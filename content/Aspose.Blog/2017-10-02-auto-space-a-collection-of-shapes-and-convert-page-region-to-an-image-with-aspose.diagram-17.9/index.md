---
title: 'Auto-space a Collection of Shapes and Convert Page Region to an Image using C# and Java'
date: Mon, 02 Oct 2017 06:36:55 +0000
draft: false
url: /2017/10/02/auto-space-a-collection-of-shapes-and-convert-page-region-to-an-image-with-aspose.diagram-17.9/
author: Imran Rafique
summary: ''
tags: []
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose-Diagram-for-net_100.png" alt="Aspose.Diagram for .NET logo">}}


We are pleased to announce that the new version 17.9 of Aspose.Diagram API is now live. The new version of the API adds features to get the shape by name, retrieves the shape ID of the shape-level annotation, adds horizontal and vertical space to the collection of shapes and render a specified rectangular region of the Visio page to an image. We recommend our client to incorporate the latest upgrade of Aspose.Diagram API to take benefit of improved functionality and bug fixes. Please use the following links for downloading Aspose.Diagram for .NET and Java assemblies.

*   [Aspose.Diagram for .NET 17.9][1]
*   [Aspose.Diagram for Java 17.9][2]

## Retrieve shape ID of a shape-level Annotation

With Aspose.Diagram API, developers can retrieve page and shape level annotations from an existing Visio drawing. After annotating a shape, there was no way to retrieve information about the shape from an annotation instance. In order to retrieve the shape from an annotation instance, the ShapeID member is added in the Annotation class and Shapes member of the Page instance allows to retrieve the shape by ID. Developers can use the following code example to retrieve the shape ID from an Annotation instance:

**C#**

```
string dataDir = @"C:\temp\";
// load a drawing
Diagram diagram = new Diagram(dataDir + "Drawing1.vsdx");
// get page by name
Page page = diagram.Pages.GetPage("Page-1");
// get the annotation by index
Annotation annotation = page.PageSheet.Annotations[1];
// get shape Id
Console.WriteLine(annotation.ShapeID);
// retrieve shape instance by shape Id
Shape shape = page.Shapes.GetShape(annotation.ShapeID);
```

**Java**

```
String dataDir = "c:\\\\temp\\\\";
// load a drawing
Diagram diagram = new Diagram(dataDir + "Drawing1.vsdx");
// get page by name
Page page = diagram.getPages().getPage("Page-1");
// get the annotation by index
Annotation annotation = page.getPageSheet().getAnnotations().get(1);
// get shape Id
System.out.println(annotation.getShapeID());
// retrieve shape instance by shape Id
Shape shape = page.getShapes().getShape(annotation.getShapeID());
```

## Add Horizontal and Vertical Space to a Collection of Visio Shapes

With the recent version 17.9 of Aspose.Diagram API, developers can add horizontal and vertical distances to a collection of shapes. In order to achieve this, the Page class offers AutoSpaceShapes member which takes ShapeCollection and AutoSpaceOptions parameters. The AutoSpaceOptions class allows to set horizontal and vertical distances. Developers can use the following code example to add horizontal and vertical space to a collection of Visio shapes:

**C#**

```
string dataDir = @"c:\\temp\\";
// load a drawing
Diagram diagram = new Diagram(dataDir + "Drawing1.vsdx");
// get page by name
Page page = diagram.Pages.GetPage("Page-1");
AutoSpaceOptions options = new AutoSpaceOptions();
// set horizontal and vertical distances
options.DistanceInHorizontal = 2;
options.DistanceInVertical = 2;
// auto-space a collection of shapes
page.AutoSpaceShapes(page.Shapes, options);
// save drawing
diagram.Save(dataDir + "Drawing1.vsdx", SaveFileFormat.VSDX);
```

**Java**

```
String dataDir = "c:\\\\temp\\\\";
// load a drawing
Diagram diagram = new Diagram(dataDir + "Drawing1.vsdx");
// get page by name
Page page = diagram.getPages().getPage("Page-1");
AutoSpaceOptions options = new AutoSpaceOptions();
// set horizontal and vertical distances
options.setDistanceInHorizontal(2);
options.setDistanceInVertical(2);
// auto-space a collection of shapes
page.autoSpaceShapes(page.getShapes(), options);
// save drawing
diagram.save(dataDir + "Drawing1.vsdx", SaveFileFormat.VSDX);
```

Please refer to these help topics:

1.  [Auto-space a Collection of Shapes in the Visio Page (with Aspose.Diagram for .NET API)][3]
2.  [Auto-space a Collection of Shapes in the Visio Page (with Aspose.Diagram for Java API)][4]

## Convert Rectangle Region of a Visio Page to an Image

With the recent version 17.9 of Aspose.Diagram for .NET API, developers can define an area with XY coordinates, width and height, and then convert this rectangle area to a supported image format. Developers can use the following code example:

**C#**

```
string dataDir = @"c:\\temp\\";
// load a Visio drawing
Diagram diagram = new Diagram(dataDir + "test.vsdx");
ImageSaveOptions Options = new ImageSaveOptions(SaveFileFormat.PNG);
// specify region
Options.Area = new RectangleF(0, 0, 1, 1);
// save into the image format
diagram.Save(dataDir + "area.png", Options);
```

Besides this, developers can retrieve shape by name and we have incorporated a number of regular bug fixes and enhancements.

## Public .NET Diagram API Changes

The following API changes in the new version are worth noticing:

*   GetShape member is added to the ShapeCollection class. It helps to retrieve a shape instance with a name.
*   ShapeID member is added in the Annotation class. It helps to retrieve shape information from an instance of Annotation.
*   Area member is added in the RenderingSaveOptions class. It helps to convert a rectangular region of the page to an image.
*   AutoSpaceShapes member is added in the Page class. It helps in adding distance to a collection of shapes.
*   AutoSpaceOptions class is added. It helps to define the horizontal and vertical distances to a collection of shapes.

## Aspose.Diagram for .NET and Java Resources

The following resources will help you work with Aspose.Diagram for .NET:

*   [Home page for Aspose.Diagram API][5].
*   [Aspose.Diagram API wiki docs][6]\- Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][7]\- Post your technical questions, queries and any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][8]\- Do not limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for .NET Examples][9]– We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.
*   [Aspose.Diagram for Java Examples][10] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   Release Notes ([.NET][11] and [Java][12] – For details on API fixes, please check Release Notes having a complete list of the new features.




[1]: https://downloads.aspose.com/diagram/net/new-releases/aspose.diagram-for-.net-17.9/
[2]: https://downloads.aspose.com/diagram/java/new-releases/aspose.diagram-for-java-17.9/
[3]: https://docs.aspose.com/display/diagramnet/Auto-space+a+Collection+of+Shapes+in+the+Visio+Page
[4]: https://docs.aspose.com/display/diagramjava/Auto-space+a+Collection+of+Shapes+in+the+Visio+Page
[5]: http://www.aspose.com/products/diagram
[6]: https://docs.aspose.com/display/diagramproductfamily/Home
[7]: https://forum.aspose.com/c/diagram
[8]: https://blog.aspose.com/category/aspose-products/aspose-diagram-product-family/
[9]: https://github.com/asposediagram/Aspose_diagram_NET
[10]: https://github.com/asposediagram/Aspose_Diagram_Java
[11]: https://docs.aspose.com/display/diagramnet/Aspose.Diagram+for+.NET+17.9+Release+Notes
[12]: https://docs.aspose.com/display/diagramjava/Aspose.Diagram+for+Java+17.9+Release+Notes)




