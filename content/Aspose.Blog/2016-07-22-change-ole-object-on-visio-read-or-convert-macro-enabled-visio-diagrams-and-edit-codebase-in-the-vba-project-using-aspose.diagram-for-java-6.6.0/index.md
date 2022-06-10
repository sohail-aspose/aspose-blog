---
title: 'Change OLE Objects in Visio and Read or Convert Macro-Enabled Visio Diagrams  in Java'
date: Fri, 22 Jul 2016 10:24:50 +0000
draft: false
url: /2016/07/22/change-ole-object-on-visio-read-or-convert-macro-enabled-visio-diagrams-and-edit-codebase-in-the-vba-project-using-aspose.diagram-for-java-6.6.0/
author: Imran Rafique
summary: ''
tags: ['Macro-Enabled Visio Diagrams', 'OLE Icons', 'VBA Project', 'VSDX', 'VSSM', 'VSTM', 'ole objects in Visio']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose_diagram-for-java-e1401178596961.png" alt="Aspose.Diagram for Java logo">}}


We’re pleased to announce that the [new version 6.6.0 of Aspose.Diagram for Java API][1] is now live. This new version adds features and provides the most notable and useful new APIs for application developers. It incorporates a way to access and modify code modules in the VBA project of Visio, read or convert macro-enabled Visio diagrams. Developers may also convert macro-enabled drawings to macro-free drawings and vice versa. Besides this, developers can manipulate OLE objects in the Visio diagram. We recommend our clients to [use Aspose powerful Java APIs directly in their Maven Projects with simple configurations][2]. For details on API fixes, please visit the product [Release Notes][3] section of this new version.

## Change an OLE Object in Visio Diagram in Java

OLE (Object Linking and Embedding) is a technology that allows applications to share data and functionality easily in a quick way. OLE allows an application to interact with another one without knowing, in advance, about the other application. Aspose.Diagram API gives developers a mechanism to programmatically retrieve OLE objects from a Visio, and then change it with its modified version.

{{< gist aspose-diagram 92a05cb833bad6d60de2968c96b40ee4 "Examples-src-main-java-com-aspose-diagram-examples-OLEObjectsinVisioDiagram-ManipulateEmbeddedOLEObjects-ManipulateEmbeddedOLEObjects.java" >}}

This help topic shows how to programmatically access an OLE object, and then change to another one: Manipulate the Embedded OLE Objects in Visio Diagram

## Read or Convert VSDM, VSSM and VSTM Files

Microsoft Office Visio has three main file types named as drawing (VSDX), stencil (VSSX) and template (VSTX). It also offers macro-enabled formats (VSDM, VSSM and VSTM) for each file type. Using Aspose.Diagram API, it is very easy for developers to transform their macro-enable diagrams to macro-free diagrams or vice versa. However, please note, only the macro-enabled files (VSDM, VSSM, VSTM) can store VBA macros.

## Edit Codebase in VBA Project of Visio

The VBA (Visual Basic Application) programs can be saved in the Microsoft Office Visio diagrams and VBA modules are the home for custom functions and subprocedures. Users may add multiple procedures in a single module manually. Using Aspose.Diagram API, developers can access and modify the source code of the whole module in the VBA project.

{{< gist aspose-diagram 92a05cb833bad6d60de2968c96b40ee4 "Examples-src-main-java-com-aspose-diagram-examples-Diagrams-ModifyVBAModuleCode-ModifyVBAModuleCode.java" >}}

This help topic shows how to dynamically modify the VBA code segments: Modify VBA Module Code in Visio Diagram

## Retrieve OLE Icons from a Visio

Users may embed documents on a Visio diagram, displayed as icons. Aspose.Diagram API allows developers to save these icons in the local storage.

```
String dirPath = "c:\\temp\\";
// load a Visio diagram
Diagram diagram = new Diagram(dirPath + "Drawing1.vsdx");
// get page of the Visio diagram by name
Page page = diagram.getPages().getPage("Page-1");
// get shape of the Visio diagram by ID
Shape OLE_Shape = page.getShapes().getShape(2);

// filter shapes by type Foreign
if (OLE_Shape.getType() == TypeValue.FOREIGN)
{
    if (OLE_Shape.getForeignData().getForeignType() == ForeignType.OBJECT)
    {
	// get byte array
    	byte[] bytes = OLE_Shape.getForeignData().getImageData();
    	// create an image file
    	FileOutputStream fos = new FileOutputStream(dirPath + "Icon_Out.png");
    	// write byte array of the image
    	fos.write(bytes);
    	// close array
    	fos.close();
    }
}
```

## Public API Changes

The following API changes in the new version are also worth noting:

*   VSDM, VSSM and VSTM options are added to the LoadFileFormat Class.
*   VSDM, VSSM and VSTM options are added to the SaveFileFormat Class.
*   VbaModule, VbaModuleCollection, VbaProject, VbaProjectReference and VbaProjectReferenceCollection classes are added.
*   An getImageData() method is added to the ForeignData class

We auto port Aspose.Diagram for .NET to Java to give developers perfectly the same features on both platforms, so this version also incorporates the bug fixes and enhancements from its equivalent .NET version. Please check a list of the resolved defects:

*   Fixed: Add support to import the macro-enabled Drawing (VSDM).
*   Fixed: Add support to import the macro-enabled template (VSTM).
*   Fixed: Add support to import the macro-enabled stencil (VSSM).
*   Fixed: Diagram exception occurred while loading a VSDX file.

## Aspose.Diagram for Java Resources

The following resources will help you work with Aspose.Diagram for Java:

*   [Homepage for Aspose.Diagram for Java API][4].
*   [Download Aspose.Diagram for Java][5].
*   [Aspose.Diagram for Java wiki docs][6] - Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][7] - Post your technical questions, queries and any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][8] - Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for Java Examples][9] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   Migrate from Earlier Versions of Aspose.Diagram API – We keep track of Aspose.Diagram API change version by version. So we recommend getting help from this section while upgrading to the latest API version or if Aspose.Diagram API code is broken at some stage.

We hope you’ll enjoy this new release that saves time and effort. The API is quite simple and developers can use it in application easily.

Intensity




[1]: https://downloads.aspose.com/diagram/java
[2]: https://blog.aspose.com/2014/08/12/aspose-for-maven-aspose-cloud-maven-repository
[3]: https://docs.aspose.com/display/diagramjava/Aspose.Diagram+for+Java+6.6.0+Release+Notes
[4]: http://products.aspose.com/diagram/java
[5]: http://downloads.aspose.com/diagram/java
[6]: http://docs.aspose.com/display/diagramjava/Home
[7]: http://forum.aspose.com
[8]: https://blog.aspose.com/
[9]: https://github.com/asposediagram/Aspose_Diagram_Java




