---
title: 'Convert Visio Diagram to SVG with Quality Control using C# and Java'
date: Tue, 05 Sep 2017 05:03:35 +0000
draft: false
url: /2017/09/05/control-svg-quality-and-connect-shapes-using-connection-indexes-with-aspose.diagram-17.8/
author: Imran Rafique
summary: ''
tags: ['Convert Visio diagrams to SVG in csharp', 'Convert Visio diagrams to SVG in java']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose-Diagram-for-net_100.png" alt="Aspose.Diagram for .NET logo">}}


We are pleased to announce that the new version 17.8 of Aspose.Diagram API is now live. The new version of the API adds features to control the image quality while exporting a Visio drawing to SVG format, and using connecting indexes to connect shapes with dynamic connectors. We recommend our client to incorporate the latest upgrade of Aspose.Diagram API to take benefit of improved functionality and bug fixes. Please use the following links for downloading Aspose.Diagram for .NET and Java assemblies.

*   [Aspose.Diagram for .NET 17.8][1]
*   [Aspose.Diagram for Java 17.8][2]

## Convert Visio Drawing to SVG

Aspose.Diagram API has support of exporting Visio drawings to SVG format and based on the customer request, we have added a Quality member to SVGSaveOptions class. We use SVGSaveOptions class to define SVG export settings and now developers can control SVG image quality. Developers can use the following code example to control the quality of SVG image:

### Convert Visio to SVG in C#```
string dataDir = @"c:\temp\";
// Load an existing drawing
Diagram diagram = new Diagram(dataDir + "Drawing1.vsdx");
// specify SVG export settings
SVGSaveOptions options = new SVGSaveOptions();
// set image quality
options.Quality = 100;
// save drawing in the SVG format
diagram.Save(dataDir + "UseSVGSaveOptions_out.svg", options);
```

### Convert Visio to SVG in Java```
String dataDir = "c:\\temp\\";
// Load an existing drawing
Diagram diagram = new Diagram(dataDir + "Drawing1.vsdx");
// specify SVG export settings
SVGSaveOptions options = new SVGSaveOptions();
// set image quality
options.setQuality(100);
// save drawing in the SVG format
diagram.save(dataDir + "UseSVGSaveOptions_out.svg", options);
```

Developers can find more details of exporting a Visio drawing to SVG. Please refer to this help topic: [Convert Visio drawing to SVG][3]

## Connect Visio Shapes with Connection Indexes

The previous versions of Aspose.Diagram API can connect shapes from the top, bottom, center, left, and right connection points. Developers were able to add new connection points to a shape, but there were limited ways to connect shapes. We have enhanced the way of connecting shapes, and developers can connect Visio shapes with the help of connection indexes. We have added ConnectShapesViaConnectorIndex methods in the Page class. Developers can use the following code to retrieve two shapes from an existing Visio drawing, and connect shapes with the help of connection indexes:

**C#**

```
string dataDir = @"c:\temp\";
// Load an existing drawing
Diagram diagram = new Diagram(dataDir + "Drawing1.vsdx");
// get shapes by ID
Aspose.Diagram.Shape shape1 = diagram.Pages[0].Shapes.GetShape(1);
Aspose.Diagram.Shape shape2 = diagram.Pages[0].Shapes.GetShape(2);
// add connector shapes
Aspose.Diagram.Shape connector1 = new Aspose.Diagram.Shape();
long connecter1Id = diagram.AddShape(connector1, "Dynamic connector", 0);
// connect shapes by index of conneecting points
diagram.Pages[0].ConnectShapesViaConnectorIndex(shape1.ID, 6, shape2.ID, 3, connecter1Id);
// save drawing
diagram.Save(dataDir + "UseSVGSaveOptions_out.vsdx", SaveFileFormat.VSDX);
```

**Java**

```
String dataDir = "c:\\temp\\";
// Load an existing drawing
Diagram diagram = new Diagram(dataDir + "Drawing1.vsdx");
// get shapes by ID
Shape shape1 = diagram.getPages().get(0).getShapes().getShape(1);
Shape shape2 = diagram.getPages().get(0).getShapes().getShape(2);
// add connector shapes
Shape connector1 = new Shape();
long connecter1Id = diagram.addShape(connector1, "Dynamic connector", 0);
// connect shapes by index of conneecting points
diagram.getPages().get(0).connectShapesViaConnectorIndex(
                shape1.getID(), 6, shape2.getID(), 3, connecter1Id);
// save drawing
diagram.save(dataDir + "UseSVGSaveOptions_out.vsdx", SaveFileFormat.VSDX);
```

Besides this, we have incorporated a number of regular bug fixes and enhancements. 

## Public .NET Diagram API Changes

The following API changes in the new version are worth noticing:

*   A quality member is added in the SVGSaveOptions class. It helps to control the quality of the generated image.
*   ConnectShapesViaConnectorIndex members are added in the Page class. It helps to connect shapes through connection indexes.

## Aspose.Diagram for .NET Resources

The following resources will help you work with Aspose.Diagram for .NET:

*   [Home page for Aspose.Diagram API][4].
*   [Aspose.Diagram API wiki docs][5]\- Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][6]\- Post your technical questions, queries and any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][7]\- Do not limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for .NET Examples][8]– We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.
*   [Aspose.Diagram for Java Examples][9] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/diagram/net/new-releases/aspose.diagram-for-.net-17.8/
[2]: https://downloads.aspose.com/diagram/java/new-releases/aspose.diagram-for-java-17.8/
[3]: https://docs.aspose.com/display/diagramnet/Save+a+Visio+Drawing#SaveaVisioDrawing-SVGSO
[4]: http://www.aspose.com/products/diagram
[5]: https://docs.aspose.com/display/diagramproductfamily/Home
[6]: https://forum.aspose.com/c/diagram
[7]: https://blog.aspose.com/category/aspose-products/aspose-diagram-product-family/
[8]: https://github.com/asposediagram/Aspose_diagram_NET
[9]: https://github.com/asposediagram/Aspose_Diagram_Java




