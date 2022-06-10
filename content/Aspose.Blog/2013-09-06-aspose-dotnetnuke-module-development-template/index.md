---
title: 'Aspose DotNetNuke Module Development Template Released'
date: Fri, 06 Sep 2013 14:27:44 +0000
draft: false
url: /2013/09/06/aspose-dotnetnuke-module-development-template/
author: Zaheer Tariq
summary: ''
tags: ['DotNetNuke', 'News Release', 'automatic download', 'module development template']
categories: ['Aspose.Total Product Family']
---

Aspose DotNetNuke Module Development Template provides a quick and easy way to use a module development template for DotNetNuke 7+ that can automatically download Aspose components and seamlessly add them to your DotNetNuke module project.

Aspose DotNetNuke Module Development Template includes the following features:

*   Supports Visual Studio 2010 and Visual Studio 2012.
*   Create DotNetNuke modules for C# or VB.NET.
*   Create DotNetNuke modules with the new DAL2 data access layer available in DotNetNuke 7 for C# or VB.NET.
*   Select one or more Aspose components during module creation.
*   The latest version of the selected Aspose components is automatically downloaded and referenced.

## How to Install the Aspose DotNetNuke Project Templates

Installing Aspose DotNetNuke project templates is pretty easy. There are multiple ways to install: choose one of these options below.

### Install manually by downloading the VSIX file from the DNN Store

1.  Visit the DNN Store – Aspose DotNetNuke Module Development Template page
2.  Click ‘Add to Cart’ and then proceed to checkout to download the VSIX file
3.  Double click on the downloaded file to install the templates.

### Install manually by downloading from Codeplex

1.  Download the VSIX file from Codeplex
2.  Double click on the downloaded file to install the templates.

**Note:** Please make sure to restart Visual Studio for the changes to take effect.

## Creating a DotNetNuke Module using the Templates

Once you’ve installed the templates, you can set up a project based on them. To do so you should follow the steps below. Before you can use them, you should have installed Visual Studio 2010 or 2012, and Aspose DotNetNuke Project Templates (described above).

1.  Set up the DotNetNuke Development environment following the steps in the Wiki (the templates assume you have your development environment set up at http://dnndev.me/). Development Environment
2.  Run Visual Studio 2010 or Visual Studio 2012 as an Administrator (right-click  the desk-top shortcut to do so)
3.  From the **File** menu, select **New Project**.
4.  Choose either C# or VB.Net from the Languages section of the new project dialog.Aspose DotNetNuke create project
5.  Select the DotNetNuke Folder under your preferred language (C# or Visual Basic).
6.  Choose either the **Aspose DotNetNuke C# Compiled Module** or **Aspose DotNetNuke 7 C# DAL2 Compiled Module** template for your project template (or the VB.NET versions).
7.  For the new project creation screen using the following settings
    1.  Name: ModuleName  
        Something unique here, example DNNTaskManager
    2.  Location: c:\\websites\\dnndev.me\\desktopmodules\\  
        This assumes you set up your development environment as instructed in step 1.
    3.  Solution: Create new solution
    4.  Create directory for solution : **Unchecked**  
        If checked, this option will cause path problems. The templates assume that the SLN is in the same folder as the project file.
    5.  Click **OK**.A screen is shown containing all Aspose components (screenshot below).
8.  Select one or more components from the list.  
    Each component’s common uses is shown upon selection.
9.  Click **Next** to continue once done.Aspose DotNetNuke create project select componentsThe Next screen shows the download progress for each selected component.Aspose DotNetNuke create project component downloadOnce the downloading is completed the module is created with the selection components automatically reference.Aspose DotNetNuke created moduleThis creates a folder under c:\\websites\\dnndev.me\\desktopmodules\\ModuleName which should contain all the files necessary for your module, including the solution.

There are a couple of final steps just to finalize the process, documented in the **Documentation\\Documentation.html** file, which should open up automatically in Visual Studio after the project is created. Follow the steps to configure the final project properties and then you are ready to build/deploy a module. You can delete the documentation folder once you have completed those steps.








