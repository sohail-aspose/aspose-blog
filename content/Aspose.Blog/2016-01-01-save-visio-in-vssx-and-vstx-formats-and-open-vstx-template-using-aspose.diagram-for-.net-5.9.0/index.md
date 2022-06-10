---
title: 'Save Visio in VSSX and VSTX Formats and Open VSTX Template using Aspose.Diagram for .NET 5.9.0'
date: Fri, 01 Jan 2016 21:54:56 +0000
draft: false
url: /2016/01/01/save-visio-in-vssx-and-vstx-formats-and-open-vstx-template-using-aspose.diagram-for-.net-5.9.0/
author: Imran Rafique
summary: ''
tags: ['Convert VSS to VSSX', 'Convert VST to VSTX', 'Convert Visio Files', 'Imran.Rafique']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose-Diagram-for-net_100.png" alt="Aspose.Diagram for .NET logo">}}


We're pleased to announce the new version 5.9.0 of the Aspose.Diagram for .NET API. We're adding support of the latest Microsoft Office Visio formats and we're almost near to complete it. It is a progressive version to accomplish the goal. From this version, developers can now read and write in VSSX stencil and VSTX template formats. Another feature of saving resultant HTML to a stream instance is added. This release also preserves missing properties of the Visio diagram and shapes. Mostly, it relates to the new supported Visio formats. We'd also like to say a special thank you to all the clients for giving effective feedbacks and sharing their common practices to further extend the API realistically.

## Convert VSS to VSSX and VST to VSTX Formats

Using Aspose.Diagram API, developers can now transform their old VSS stencils and VST templates to the new VSSX stencils and VSTX templates respectively. They just need to open and then save by calling a couple of lines of code as follows:

```
// load an old VSS stencil
Diagram diagram = new Diagram(MyDir + "MyStencil.vss");
// save it in the VSSX format.
diagram.Save(MyDir + "MyStencil.vssx", SaveFileFormat.VSSX);
```

We have already added support of reading VSSX stencil, so developers can also manipulate its elements like the old VSS format.

## Reading and Writing Support of VSTX Template

This version covers both reading and writing support of the VSTX template. Developers would be able to alter their VSTX templates and even save them in any other supported file format.

## Save Resultant HTML Directly to a Stream

Developers can now save a Visio directly to an instance of the stream because they might have the scenario to save the resultant HTML in a database or repository without storing it in the local storage. This feature also embeds other resultant resources of the HTML, e.g. fonts, CSS (containing the style information) and images. Since it saves a single HTML file into the stream instance. This help topic shows how developers can save the resultant HTML in the stream instance: [How to Convert a Visio to HTML][1]

## Copy Themes and PageSheet of an Existing Visio

We use themes and Visio page sheet properties to manage formatting and professional look of the Visio diagrams. Previously, Aspose.Diagram API users were not able to copy them from one Visio diagram to another programmatically. All this was leading to a partial import of the Visio shape. From this version, its support is added. Diagram class offers CopyTheme method and PageSheet class offers Copy method to accomplish the goal of copying a shape and other manipulation tasks. This help topic shows how developers can copy a shape from an existing Visio: [Copy Shapes from an Existing Visio][2]

## Retrieval of the Visio Properties

Aspose.Diagram API has support of retrieving various properties of the shapes and Visio diagram. However, by adding read and write support of three main latest formats (VSDX, VSTX and VSSX), we further need to fix the problems of missing properties. This release covers the defects of such missing properties. These defects are specific to the latest Visio formats.

This release also covers many aspects in the export, layout, structure, performance and quality areas. Please check a list of fixed defects:

*   Fixed: CompactTree (RightThenDown) - Connection points of each shape are incorrect.
*   Fixed: Diagram.Layout method does not change layout of all pages.
*   Fixed: Shape.gluedShapes method is not working as expected.
*   Fixed: \[Output format VDX\] - Group Shape is not displayed properly.
*   Fixed: \[Output format PDF\] - Can't place a group shape from another Visio diagram.
*   Fixed: \[Output format VDX\] - Fill style of the Shapes is not preserved.
*   Fixed: Index out of bounds error occurred while loading a VSD diagram.
*   Fixed: VSD to VDX export, connectors position is changed.
*   Fixed: Open and save VSDX, the server shapes are missing.
*   Fixed: VSD to VSDX export, CustomProp class does not return an actual value.
*   Fixed: VDX to PDF export, the resultant PDF is blank.
*   Fixed: VDX to BMP export, an argument exception occurred.
*   Fixed: VDX to JPEG export, an argument exception occurred.
*   Fixed: VSDX to SVG export, the custom properties of the shapes are not preserved.

## Public API Changes

The following API changes in the new version are also worth noting:

*   The VSSX format option has been added in the SaveFileFormat enum.
*   The VSTX format option has been added in the SaveFileFormat enum.
*   The VSTX format option has been added in the LoadFileFormat enum.
*   The CopyTheme method has been added in the Diagram class.
*   The Copy method has been added in the PageSheet class.

## Aspose.Diagram for .NET Resources

The following resources will help you work with Aspose.Diagram for .NET:

*   [Home page for Aspose.Diagram for .NET API][3].
*   [Download Aspose.Diagram for .NET][4]
*   [Aspose.Diagram for .NET wiki docs][5] - Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][6] - Post your technical questions and queries, or any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][7] - Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

We hope you’ll enjoy this new release that save time and efforts. The API is quite simple and developers can use it in application easily.




[1]: https://docs.aspose.com/display/diagramnet/Home
[2]: http://docs.aspose.com/display/diagramnet/Add%2C+Retrieve%2C+Copy+and+Read+Visio+Shape+Data#Add%2CRetrieve%2CCopyandReadVisioShapeData-CopyShapesfromanExistingVisio
[3]: https://products.aspose.com/diagram/net
[4]: https://downloads.aspose.com/diagram/net
[5]: http://docs.aspose.com/display/diagramnet/Home
[6]: https://forum.aspose.com/
[7]: https://blog.aspose.com/
[8]: https://github.com/aspose-diagram/Aspose.Diagram-for-.NET




