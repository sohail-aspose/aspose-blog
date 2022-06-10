---
title: 'Identify Glued or Connected Visio Shapes using C# or VB.NET'
date: Thu, 28 Jan 2016 11:44:05 +0000
draft: false
url: /2016/01/28/identify-glued-or-connected-visio-shapes-read-vssx-stencil-and-export-shapes-with-shadow-using-aspose.diagram-for-.net-6.0.0/
author: Imran Rafique
summary: ''
tags: ['Aspose APIs', 'Convert Visio', 'Glue Visio shape', 'Imran.Rafique', 'VSSX masters', 'open VSSX', 'shape geometry', 'shape shadow', 'shape style']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose-Diagram-for-net_100.png" alt="Aspose.Diagram for .NET logo">}}


We're pleased to announce the new version 6.0.0 of the Aspose.Diagram for .NET API. This version contains new methods that let developers know about shape connections beforehand. They could now get the information, whether two shapes are connected or glued prior to any other manipulation of the Visio shapes, which can result in greater programmer productivity and more concise readable code. The reading capacity of VSSX stencils and preserving shadows of shapes during the export operation have also been enhanced. It helps in making Visio diagram look both professional and beautiful. This also includes a large number of bug fixes along with several new enhancements, and performance improvements.

## Check Whether Visio Shapes are Glued or Connected

Two Visio shapes could be glued or connected with each other. Using Aspose.Diagram API, developers could now determine whether shapes are connected or glued. It offers IsGlued and IsConnected methods in the Shape class. Both these methods take a destination shape object as a parameter and return resultant true or false. This help topic shows how developers can check whether two shapes are glued or connected: Verify Whether Two Visio Shapes are Connected or Glued.

{{< gist aspose-diagram cce69e51f567ea17ef24bc35fef0f689 "Examples-CSharp-Working-Shapes-VerifyConnectedOrGluedShapes-VerifyConnectedOrGluedShapes.cs" >}}

## Reading Improvements of VSSX Stencil

Aspose.Diagram API has already supported reading VSSX stencils and we received some use cases from our clients where it was not properly loading VSSX stencil. It was due to the internal elements of conflict. Using this version, developers can now even load their complex stencil files.

## Visio Export Preserves Shadow of the Shapes

Microsoft Office Visio allows to apply shadows to the shapes in the drawing and easily change the color, style, pattern, size, position, and angle of those shadows. Using this version, the shadows of the shapes are also being exported when converting a Visio to any supported file format.

This release also covers many other recent defects, e.g. white spots in the resultant PDF, misplaced shapes, in correct geometry, incorrect shape ids of the connected shapes and partial rendering of the Visio shapes. Please check a list of fixed defects:

*   Fixed: VSD to PDF export, empty PDF having white spot is generated.
*   Fixed: VSD to VDX conversion, curve dynamic connectors turn into the straight.
*   Fixed: VSD to HTML conversion, the text shape is misplaced.
*   Fixed: VSD to PDF conversion, the text "Iloprost" is added in the header of all pages.
*   Fixed: VSD to PDF conversion, the list items are misplaced.
*   Fixed: VSD to HTML conversion, the text "Iloprost" is added in the header of all pages.
*   Fixed: Can't detect incoming nodes of the connected shapes.
*   Fixed: Geometry of the connector shapes is incorrect.
*   Fixed: Geometry of the connector shapes is incorrect.
*   Fixed: Output format HTML\] - Can't place a group shape from another Visio diagram.
*   Fixed: Copying a Visio diagram page operation does not preserve the style of the shapes.
*   Fixed: Copying a Visio diagram page does not preserve shapes completely.
*   Fixed: Copying a Visio diagram page does not preserve shapes completely.
*   Fixed: VDX to VDX export, shape's text is not bold.
*   Fixed: Source VSD - ConnectCollection class returns additional connect and incorrect shape ids.
*   Fixed: Shape.connectedShapes method returns incorrect shape ids.
*   Fixed: Shape.connectedShapes method detects the incorrect direction of the shape connectors.
*   Fixed: Diagram.Save method call also closes the resultant stream.
*   Fixed: \[output VSDX\] - A missing parts error occurred.

## Public API Changes

The following API changes in the new version are also worth noting:

*   IsGlued method has been added in the Shape class.
*   IsConnected method has been added in the Shape class.

## Aspose.Diagram for .NET Resources

The following resources will help you work with Aspose.Diagram for .NET:

*   [Home page for Aspose.Diagram for .NET API][1].
*   [Download Aspose.Diagram for .NET][2]
*   Aspose.Diagram for .NET wiki docs - Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][3] - Post your technical questions and queries, or any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][4] - Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for .NET Examples][5] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   How to Migrate from Earlier Versions of Aspose.Diagram API - We keep track of Aspose.Diagram API change version by version. So we recommend to get help from this section while upgrading to the latest API version or if Aspose.Diagram API code is broken at some stage.

We hope you’ll enjoy this new release that saves time and efforts. The API is quite simple and developers can use it in application easily.




[1]: https://products.aspose.com/diagram
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.diagram-for-.net/default.aspx
[3]: http://www.aspose.com/community/forums/aspose.diagram-product-family/489/showforum.aspx
[4]: https://blog.aspose.com/
[5]: https://github.com/asposediagram/Aspose_diagram_NET




