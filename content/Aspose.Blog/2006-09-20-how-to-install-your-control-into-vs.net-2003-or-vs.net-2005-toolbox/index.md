---
title: 'How to Install Your Control Into VS.NET 2003 or VS.NET 2005 Toolbox'
date: Wed, 20 Sep 2006 15:21:00 +0000
draft: false
url: /2006/09/20/how-to-install-your-control-into-vs.net-2003-or-vs.net-2005-toolbox/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

We needed to make sure some of the Aspose components are installed into the Toolbox in VS.NET during installation. We sifted through many discussions about this on the net.

It is a trivial task, but looks like a lack of thought from Microsoft made it very complex. It is especially problematic because a reasonable way of installing the control to Toolbox in VS.NET 2003 does not work in VS.NET 2005.

I pulled ideas from several resources to come up with my own version of how to do it. It is now used in some of Aspose installers.

Essentially, it uses automation to instantiate VS.NET DTE (I guess it is another name for IDE?). Then it creates a tab with a name that you specify and adds all controls that are found in a specified assembly to that tab. When uninstalling, it removes the complete tab, not individual controls. It works for VS.NET 2003 and VS.NET 2005.

We invoke **ToolboxInstaller.InstallControls** from an installer class. The installer class is run by a custom action during the setup process.

This installer project is compiled in VS.NET 2003 for .NET 1.1. Apart from referncing EnvDTE.dll, it is interesting to note that it references EnvDTE80.dll (which must be a primary interop assembly for VS.NET 2005). I have both VS.NET 2003 and 2005 installed on my machine and I reference these dlls in C:\\Program Files\\Microsoft Visual Studio 8\\Common7\\IDE\\PublicAssemblies\\.

When I add the installer project to the setup project, it adds EnvDTE.dll and EnvDTE80.dll along with a few other files to the setup project, which I personally don't think is nice, but okay to live with it.

I have the following custom actions in my setup project:

**Install**

*   Name: AddToToolbox2003  
    CustomActionData: /Cmd=AddToToolbox /AssemblyName="\[TARGETDIR\]bin\\Aspose.Editor.dll" /Version=VS2003
*   Name:AddToToolbox2005  
    CustomActionData: /Cmd=AddToToolbox /AssemblyName="\[TARGETDIR\]bin\\Aspose.Editor.dll" /Version=VS2005

**Uninstall**

*   Name: RemoveFromToolbox2003  
    CustomActionData: /Cmd=RemoveFromToolbox /AssemblyName="\[TARGETDIR\]bin\\Aspose.Editor.dll" /Version=VS2003
*   Name: RemoveFromToolbox2005  
    CustomActionData: /Cmd=RemoveFromToolbox /AssemblyName="\[TARGETDIR\]bin\\Aspose.Editor.dll" /Version=VS2005

Inside the installer class, I check the Cmd parameter and take an appropriate action. For simplicity, I use the name of the assembly (without path and without extension) for the tab name.

```
string cmd = Context.Parameters[“Cmd”];

if (cmd == “AddToToolbox”)

{

          InstallControls(true);

}

else if (cmd == “RemoveFromToolbox”)

{

          InstallControls(false);

}

 

…

 

/// <summary>

/// Installs or uninstalls controls to toolbox.

///

/// Context needs to have these parameters:

/// /AssemblyName should be full path to the assembly that contains controls.

/// /Version could be VS2003 or VS2005

/// </summary>

private void InstallControls(bool isInstall)

{

          string assemblyName = Context.Parameters[“AssemblyName”];

          string tabName = Path.GetFileNameWithoutExtension(assemblyName);

          DteVersion version = StringToDteVersion(Context.Parameters[“Version”]);

          ToolboxInstaller.InstallControls(tabName, assemblyName, version, isInstall);

}

 

private DteVersion StringToDteVersion(string value)

{

          switch (value)

          {

                   case “VS2003”: return DteVersion.VS2003;

                   case “VS2005”: return DteVersion.VS2005;

                   default: throw new Exception(“Unknown DTE version.”);

          }

}

 

 

ToolboxInstaller.cs code below

 

//20/9/06 by Roman Korchagin

using System;

using System.IO;

using System.Runtime.InteropServices;

using EnvDTE;

using EnvDTE80;

 

namespace Aspose.Installer

{

          public enum DteVersion

          {

                   VS2003,

                   VS2005

          }

 

          /// <summary>

          /// Installs and uninstalls controls to the VS.NET ToolBox.

          /// Took ideas from these sources:

          /// http://dev.devbiz.com/blogs/workingsmart/archive/2005/07/27/adding_controls_to_vs_net_toolbox.aspx

          /// http://blogs.msdn.com/chetanc/archive/2006/01/19/515016.aspx

          /// </summary>

          public class ToolboxInstaller

          {

                   /// <summary>

                   /// When isInstall = true, creates tab group with specified name in control toolbox in

                   /// VS.NET 2003 or 2005 and adds a controls from specified assembly to it.

                   /// When isInstall = false, deletes the tab from the toolbox.

                   /// </summary>

                   internal static void InstallControls(string tabName, string assemblyName, DteVersion dteVersion, bool isInstall)

                   {

                             Type type = System.Type.GetTypeFromProgID(GetProgId(dteVersion));

                             DTE dte = (DTE)System.Activator.CreateInstance(type);

                             try

                             {

                                      if (isInstall)

                                      {

                                                if (dteVersion == DteVersion.VS2005)

                                                {

                                                          // create a temporary winform project;

                                                          // RK: I guess this is needed to overcome the extensibility issue in VS.NET 2005.

                                                          // If you attempt to add controls to the toolbox without a project open, it does not work.

                                                          string tmpFile = Path.GetFileNameWithoutExtension(Path.GetTempFileName());

                                                          string tmpDir = string.Format(“{0}{1}”,Path.GetTempPath(),tmpFile);

                                                          Solution2 solution = dte.Solution as Solution2;

                                                          string templatePath = solution.GetProjectTemplate(“WindowsApplication.zip”, “CSharp”);

                                                          solution.AddFromTemplate(templatePath, tmpDir, “dummyproj”, false);

                                                }

 

                                                ToolBoxTabs tabs = GetTabs(dte);

                                                ToolBoxTab tab = GetToolBoxTab(tabs, tabName);

                                                if (tab == null)

                                                          tab = tabs.Add(tabName);

 

                                                tab.Activate();

                                                tab.ToolBoxItems.Item(1).Select();

                                                tab.ToolBoxItems.Add(“MyControls”, assemblyName, vsToolBoxItemFormat.vsToolBoxItemFormatDotNETComponent);

                                      }

                                      else

                                      {

                                                // We remove the tab completely, not individual controls.

                                                ToolBoxTabs tabs = GetTabs(dte);

                                                ToolBoxTab tab = GetToolBoxTab(tabs, tabName);

                                                if (tab != null)

                                                          tab.Delete();

                                      }

                             }

                             finally

                             {

                                      dte.Solution.Close(false);

                                      dte.Quit();

                                      Marshal.ReleaseComObject(dte);

 

                                      // to ensure the dte object is actually released, and the devenv.exe process terminates.

                                      // RK: I’m not sure, but lets keep it.

                                      GC.Collect();

                                      GC.WaitForPendingFinalizers();

                             }

                   }

 

                   /// <summary>

                   /// Gets the toolbox tabs collection.

                   /// Uses a simplistic approach with retries to waits for the IDE to become available.

                   /// </summary>

                   private static ToolBoxTabs GetTabs(DTE dte)

                   {

                             const int MaxRetries = 10;

                             const int DelayBetweenRetries = 5000;

 

                             for (int retryCount = 0; retryCount < MaxRetries; retryCount++)

                             {

                                      try

                                      {

                                                Window toolbox = dte.Windows.Item(Constants.vsWindowKindToolbox);

                                                ToolBoxTabs tabs = ((ToolBox)toolbox.Object).ToolBoxTabs;

                                                dte.ExecuteCommand(“View.PropertiesWindow”, “”);

                                                return tabs;

                                      }

                                      catch (Exception)

                                      {

                                                // Most likely this is the “The message filter indicated that the application is busy.” exception.

                                                // Lets wait a little and retry.

                                                System.Threading.Thread.Sleep(DelayBetweenRetries);

                                      }

                             }

 

                             throw new Exception(“Cannot obtain toolbox from the IDE.”);

                   }

 

                   private static ToolBoxTab GetToolBoxTab(ToolBoxTabs tabs, string tabName)

                   {

                             foreach (ToolBoxTab tab in tabs)

                             {

                                      if (string.Compare(tab.Name, tabName, true) == 0)

                                                return tab;

                             }

                             return null;

                   }

 

                   private static string GetProgId(DteVersion dteVersion)

                   {

                             switch (dteVersion)

                             {

                                      case DteVersion.VS2003: return “VisualStudio.DTE.7.1”;

                                      case DteVersion.VS2005: return “VisualStudio.DTE.8.0”;

                                      default: throw new Exception(“Unknown DTE version.”);

                             }

                   }

          }

}
```

Here is how the installed control looks in the IDEs (still using a default icon):  



{{< figure align=center src="images/vs2003.jpg" alt="">}}








