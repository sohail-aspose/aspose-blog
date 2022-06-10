---
title: 'Load and Save Macro Enabled Visio Files and Modify VBA Project Code in Visio Diagram using Aspose.Diagram for .NET 6.6.0'
date: Wed, 20 Jul 2016 12:08:31 +0000
draft: false
url: /2016/07/20/load-and-save-macro-enabled-visio-files-modify-vba-project-code-and-manipulate-the-embedded-ole-objects-in-visio-diagram-using-aspose.diagram-for-.net-6.6.0/
author: Imran Rafique
summary: ''
tags: ['Embedded OLE Objects in Visio', 'OLE object icon', 'VBA Macros in Visio Files', 'VBA Project', 'VSDM', 'VSSM', 'VSTM', 'export macro-enabled Visio', 'import macro-enabled Visio', 'macro-enabled Visio files']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose-Diagram-for-net_100.png" alt="Aspose.Diagram for .NET logo">}}


We're pleased to announce that the [new version 6.6.0 of Aspose.Diagram for .NET API][1] is now live. This new version offers new APIs to incorporate new features. These APIs allow developers to retrieve VBA project and modify the source code of modules as well as import and export macro-enabled Visio files. Developers may also retrieve an OLE object to modify it, and then save back in the Visio diagram. Developers can install an Aspose.Diagram Nuget package in their .NET applications because we publish each version as [a NuGet package on the NuGet gallery][2]. We recommend our clients upgrade the old version of Aspose.Diagram API to this latest one. For details on API fixes, please check [Release Notes][3] having a complete list of the features, enhancements and bug fixes.

## Load and Save VSDM, VSSM and VSTM Files

Microsoft Office Visio has the support of macro-enabled Visio formats. We have added support of reading and writing macro-enabled Visio files, since developers can load and save VSDM (Visio macro-enabled drawing), VSSM (Visio macro-enabled stencil) and VSTM (Visio macro-enabled template) files same as the native VSDX format. They can also access internal elements for manipulation purposes.

## Modify Code Modules in VBA Project of Visio

A VBA (Visual Basic Application) project is the part of a Visio diagram. Users may create custom functions or subprocedures to refer in the calculations, and then run from a module. Using Aspose.Diagram API, developers can programmatically access VBA project, iterate through the modules, retrieve code for modification purposes and save back in the VBA project module. 

{{< gist aspose-diagram cce69e51f567ea17ef24bc35fef0f689 "Examples-CSharp-Working-Diagrams-ModifyVBAModule-ModifyVBAModule.cs" >}}

This help topic shows how developers can do so: [Modify VBA Module Code in Visio Diagram][4]

## Manipulate the Embedded OLE Objects in Visio

Object linking and embedding (OLE) is a Microsoft technology that facilitates the sharing of application data and objects written in different formats from multiple sources. Linking part establishes a connection between two objects, and embedding part facilitates application data insertion. OLE is used for compound document management, as well as an application data transfer. Aspose.Diagram API allows developers to manipulate with an existing OLE object in the Visio diagram. For example, developers may retrieve a Word document, modify it using Aspose.Words API and then save back in the Visio diagram.

{{< gist aspose-diagram cce69e51f567ea17ef24bc35fef0f689 "Examples-CSharp-OLE-Objects-ManipulateObjects-ManipulateObjects.cs" >}}

This help topic shows how developers can achieve this: [Manipulate the Embedded OLE Objects in Visio Diagram][5]

## Change the Icon of an OLE Object

Using Aspose.Diagram API, developers can also change the icon of an OLE object. ForeignData class offers an ImageData property which helps in retrieving an icon of the OLE object or change it with another one. Below is code to retrieve the icon of an OLE object.

**Sample Code: C#, .NET**

```
// set directory path
string dataDir = @"c:\temp\";
// load a Visio diagram
Diagram diagram = new Diagram(dataDir + "Drawing1.vsdx");
// get page of the Visio diagram by name
Page page = diagram.Pages.GetPage("Page-1");
// get OLE shape of the Visio diagram by ID
Shape OLE_Shape = page.Shapes.GetShape(2);

// filter shapes by type Foreign
if (OLE_Shape.Type == Aspose.Diagram.TypeValue.Foreign)
{
  if (OLE_Shape.ForeignData.ForeignType == ForeignType.Object)
  {
    using (MemoryStream stream = new MemoryStream(OLE_Shape.ForeignData.ImageData))
    {
      // load memory stream into bitmap object
      System.Drawing.Bitmap bitmap = new System.Drawing.Bitmap(stream);
      // save as png format
      bitmap.Save(dataDir + "OleIcon_Out.bmp", System.Drawing.Imaging.ImageFormat.Bmp);
    }
  }
} 
```

## Public API Changes

The following API changes in the new version are also worth noting:

*   VSDM, VSSM and VSTM options are added to the LoadFileFormat Class.
*   VSDM, VSSM and VSTM options are added to the SaveFileFormat Class.
*   VbaModule, VbaModuleCollection, VbaProject, VbaProjectReference and VbaProjectReferenceCollection classes are added.
*   An ImageData property is added to the ForeignData class

This version also addresses the issues of changing color of shapes, missing text items, the alignment problem of the shapes, additional circular shapes and accuracy in size of the shapes. These enhancements and bug fixes improve overall performance of Aspose.Diagram API. Please check a list of the resolved defects:

*   Fixed: VSDX to PDF export - the shape's boundary color overlaps the internal structure.
*   Fixed: Diagram exception occurred while loading a VSDX file.
*   Fixed: The text items are missing on converting a VSD to PDF, PNG and JPG.
*   Fixed: The transparent background of images turns into white color on converting VSD to PDF and JPG.
*   Fixed: Diagram exception occurred on saving VDX, VSX and VTX files.
*   Fixed: Properties of the diagram are not preserved during open and save.
*   Fixed: The appearance of the process shape is changed on converting a VSD to PDF and HTML.
*   Fixed: Text alignment problem on Converting a VSDX to PDF.
*   Fixed: An image is not being preserved on converting a VSD to PDF.
*   Fixed: Incorrect formatting of the shape on converting a VSD to PDF.
*   Fixed: Extra circles are added while converting a VSD to PDF.
*   Fixed: Shapes are misplaced on converting a VSD to PDF.
*   Fixed: Size of shapes is changed on converting a VSD to PDF.

## Aspose.Diagram for .NET Resources

The following resources will help you work with Aspose.Diagram for .NET:

*   [Home page for Aspose.Diagram for .NET API][6].
*   [Download Aspose.Diagram for .NET][7]
*   [Aspose.Diagram for .NET wiki docs][8] - Help documentation and API reference documents.
*   [Aspose.Diagram product][9] [](http://forum.aspose.com) [family forum][10] - Post your technical questions, queries and any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][11] - Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for .NET Examples][12] – We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.
*   [Migrate from Earlier Versions of Aspose.Diagram API][13] - We keep track of Aspose.Diagram API change version by version. So we recommend to get help from this section while upgrading to the latest API version or if Aspose.Diagram API code is broken at some stage.

We hope you’ll enjoy this new release that saves time and efforts. The API is quite simple and developers can use it in application easily.




[1]: https://downloads.aspose.com/diagram/net
[2]: https://www.nuget.org/packages/Aspose.Diagram
[3]: http://docs.aspose.com/display/diagramnet/Aspose.Diagram+for+.NET+6.6.0+Release+Notes
[4]: http://docs.aspose.com/display/diagramnet/Create%2C+Update%2C+Layout+and+Auto-Fit+Shapes#Create%2CUpdate%2CLayoutandAuto-FitShapes-ModifyVBAModuleCodeinVisioDiagram
[5]: http://docs.aspose.com/display/diagramnet/Manipulate+the+Embedded+OLE+Objects+in+Visio+Diagram
[6]: https://products.aspose.com/diagram/net
[7]: https://downloads.aspose.com/diagram/net
[8]: http://docs.aspose.com/display/diagramnet/Home
[9]: http://www.aspose.com/community/forums/aspose.diagram-product-family/489/showforum.aspx
[10]: http://www.aspose.com/community/forums/aspose.diagram-product-family/489/showforum.aspx
[11]: https://blog.aspose.com/
[12]: https://github.com/asposediagram/Aspose_diagram_NET
[13]: http://docs.aspose.com/display/diagramnet/Migrating+from+Earlier+Versions+of+Aspose.Diagram




