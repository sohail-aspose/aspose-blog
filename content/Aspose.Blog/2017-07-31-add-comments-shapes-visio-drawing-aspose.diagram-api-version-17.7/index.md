---
title: 'Add Comments to Shapes in Visio Drawings using C# and Java'
date: Mon, 31 Jul 2017 03:57:07 +0000
draft: false
url: /2017/07/31/add-comments-shapes-visio-drawing-aspose.diagram-api-version-17.7/
author: Imran Rafique
summary: ''
tags: ['add comments to Visio Shapes']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose-Diagram-for-net_100.png" alt="Aspose.Diagram for .NET logo">}}


We are pleased to announce that the new version 17.7 of Aspose.Diagram API is now live. The new version of the API adds a feature to add comments to the Visio shapes and also includes regular bug fixes and enhancements. Please use the following links for downloading Aspose.Diagram for .NET and Java assemblies.

*   [Aspose.Diagram for .NET 17.7][1]
*   [Aspose.Diagram for Java 17.7][2]

## Add Comments to a Visio Shape using C# and Java

The recent version 17.7 of Aspose.Diagram API allows to [add comments to any Visio shape in the drawing][3] and the shape-level comments will stay with the shape even if it is moved around. In order to read a comment, click the comment icon beside the shape and the comment will open. In order to close the comment, click on a blank area of the page. Developers can use the following code example to add comments to a Visio shape:

**C#**

```
// load diagram  
Diagram diagram = new Diagram(@"c:\\temp\\Drawing1.vsdx");  
// retrieve page by name  
Aspose.Diagram.Page page = diagram.Pages.GetPage("Page-1");  
// retrieve shape by ID  
Aspose.Diagram.Shape shape = page.Shapes.GetShape(12);  
page.AddComment(shape, "Hello");  
// save diagram  
diagram.Save(@"c:\\temp\\Drawing1.vsdx", SaveFileFormat.VSDX);
```

**Java**

```
// load diagram  
Diagram diagram = new Diagram("c:\\\\temp\\\\Drawing1.vsdx");  
// retrieve page by name  
Page page = diagram.getPages().getPage("Page-1");  
// retrieve shape by ID  
Shape shape = page.getShapes().getShape(12);  
page.addComment(shape, "Hello");  
// save diagram  
diagram.save("c:\\\\temp\\\\Drawing1.vsdx", SaveFileFormat.VSDX);
```

Besides this, the mechanism of retrieving SolutionXML elements and page information from the Visio drawing has been improved. The recent version also comprises a series of bug fixes.  In general, it improves the export of Visio drawings to SVG, VSDX, and image formats as well as preserves the page-level comments on the Visio drawings.

## Public API Changes

The following API change in the new version is worth noticing:

*   AddComment(shapeinstance, "comment string") method is added in the Shape class. It helps to add comments to a shape.

## Aspose.Diagram for .NET Resources

The following resources will help you work with Aspose.Diagram for .NET:

*   [Home page for Aspose.Diagram API][4].
*   [Aspose.Diagram API wiki docs][5]\- Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][6]\- Post your technical questions, queries and any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][7]\- Do not limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for .NET Examples][8]– We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.
*   [Aspose.Diagram for Java Examples][9] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/diagram/net/new-releases/aspose.diagram-for-.net-17.7/
[2]: https://downloads.aspose.com/diagram/java/new-releases/aspose.diagram-for-java-17.7/
[3]: https://docs.aspose.com/display/diagramnet/Working+with+Comments#WorkingwithComments-AddaShape-LevelCommentinVisioDrawing
[4]: http://www.aspose.com/products/diagram
[5]: https://docs.aspose.com/display/diagramproductfamily/Home
[6]: https://forum.aspose.com/c/diagram
[7]: https://blog.aspose.com/category/aspose-products/aspose-diagram-product-family/
[8]: https://github.com/asposediagram/Aspose_diagram_NET
[9]: https://github.com/asposediagram/Aspose_Diagram_Java




