---
title: 'Refresh Data of Shapes in Visio Drawing in C# or Java'
date: Mon, 03 Jul 2017 15:49:33 +0000
draft: false
url: /2017/07/03/refresh-data-shapes-visio-drawing-aspose.diagram-api-version-17.6/
author: Imran Rafique
summary: ''
tags: ['Refresh data of connected shapes in Visio in CSharp', 'Refresh data of connected shapes in Visio in Java', 'recalculate connected shapes']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose-Diagram-for-net_100.png" alt="Aspose.Diagram for .NET logo">}}


We are pleased to announce that the new version 17.6 of [Aspose.Diagram][1] API is now live. The new version of the API adds a feature to refresh the data of shapes in the Visio drawing and developers can call this feature after modifying the position or size of shapes in a connected drawing. Please use the following links for downloading Aspose.Diagram for .NET and Java assemblies.

*   [Aspose.Diagram for .NET 17.6][2]
*   [Aspose.Diagram for Java 17.6][3]

## Refresh Data of Connected Visio Shapes

The recent version 17.6 of Aspose.Diagram API allows refreshing the data of shapes, including XForm, TextXForm, Connection, and Geoms after changing the text or position of the connected shapes. When there are many changes to the ShapeSheet data and developers want to recalculate the connected shapes in a drawing. They can call the RefreshData method of each shape instance as below:

### C#```
// load diagram
Diagram diagram = new Diagram(@"c:\temp\Drawing1.vsdx");
// retrieve page by name
Aspose.Diagram.Page page = diagram.Pages.GetPage("Page-1");
// retrieve shape by ID
Shape shape = page.Shapes.GetShape(12);
shape.RefreshData();
// save diagram
diagram.Save(@"c:\temp\Drawing1.vsdx", SaveFileFormat.VSDX);
```

### Java```
// load diagram
Diagram diagram = new Diagram("c:\\temp\\Drawing1.vsdx");
// retrieve page by name
com.aspose.diagram.Page page = diagram.getPages().getPage("Page-1");
// retrieve shape by ID
Shape shape = page.getShapes().getShape(12);
shape.refreshData();
// save diagram
diagram.save("c:\\temp\\Drawing1.vsdx", SaveFileFormat.VSDX);
```

Besides this, the mechanism of storing and retrieving text elements in the Visio drawings has been improved. The recent version also comprises a series of bug fixes.  In general, it improves the export of Visio drawings to SVG and image formats as well as preserves formulas in the shapesheet.

## Public API Changes

The following API changes in the new version are also worth noticing:

*   RefreshData() method is added in the Shape class. It helps in recalculating the entire data of the Shape.

## Aspose.Diagram for .NET Resources

The following resources will help you work with Aspose.Diagram for .NET:

*   [Home page for Aspose.Diagram API][4].
*   [Aspose.Diagram API wiki docs][5] - Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][6] - Post your technical questions, queries, and any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][7] - Do not limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.
*   [Aspose.Diagram for Java Examples][9] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://products.aspose.com/diagram
[2]: https://downloads.aspose.com/diagram/net/new-releases/aspose.diagram-for-.net-17.6/
[3]: https://downloads.aspose.com/diagram/java/new-releases/aspose.diagram-for-java-17.6/
[4]: https://products.aspose.com/diagram
[5]: https://docs.aspose.com/display/diagramproductfamily/Home
[6]: https://forum.aspose.com/c/diagram
[7]: https://blog.aspose.com/category/aspose-products/aspose-diagram-product-family/
[8]: https://github.com/asposediagram/Aspose_diagram_NET
[9]: https://github.com/asposediagram/Aspose_Diagram_Java




