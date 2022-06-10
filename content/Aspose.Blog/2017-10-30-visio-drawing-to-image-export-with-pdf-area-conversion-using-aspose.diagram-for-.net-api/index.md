---
title: 'Convert Visio Drawing to Image using Aspose.Diagram for .NET and Java'
date: Mon, 30 Oct 2017 21:22:56 +0000
draft: false
url: /2017/10/30/visio-drawing-to-image-export-with-pdf-area-conversion-using-aspose.diagram-for-.net-api/
author: Imran Rafique
summary: ''
tags: ['Convert Visio Diagram to Image in Csharp', 'Convert Visio Diagram to Image in Java']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose-Diagram-for-net_100.png" alt="Aspose.Diagram for .NET logo">}}


We are pleased to announce that the new version 17.10 of Aspose.Diagram API is now live. The new version of the API adds a feature to export the Visio drawing to image format in the same way as the API converts a Visio drawing to PDF. The recent version covers a feature, enhancement and regular bug fixes. We recommend our client to incorporate the latest upgrade of Aspose.Diagram API to take benefit of improved functionality and bug fixes. Please use the following links for downloading Aspose.Diagram for .NET and Java assemblies.

*   [Aspose.Diagram for .NET 17.10][1]
*   [Aspose.Diagram for Java 17.10][2]

## Convert Visio Drawing to Image with PDF Export Area Option

Aspose.Diagram API has the support of converting Visio drawing to an image. With the recent version 17.10, developers can convert a drawing to image with the same conversion area as Microsoft Visio application converts a drawing to PDF. In order to achieve this, we have added the SameAsPdfConversionArea member in the ImageSaveOptions class. Please try the following code example:

**C#**

```
string dataDir = @"C:\temp\";// load a drawingDiagram diagram = new Diagram(dataDir + "Drawing1.vsdx");// specify image save optionsImageSaveOptions opts = new ImageSaveOptions(SaveFileFormat.PNG);opts.SameAsPdfConversionArea = true;
```

**Java**

```
String dataDir = "C:\\\\temp\\\\";  
// load a drawing  
Diagram diagram = new Diagram(dataDir + "Drawing1.vsdx");  
// specify image save options  
ImageSaveOptions opts = new ImageSaveOptions(SaveFileFormat.PNG);  
opts.setSameAsPdfConversionArea(true);
```

## Public Aspose.Diagram for .NET and Java API Changes

The following API changes in the new version are worth noticing:

*   SameAsPdfConversionArea member is added to the ImageSaveOptions class. It helps to specify whether to save area in the same way as the PDF.

## Aspose.Diagram for .NET and Java Resources

The following resources will help you work with Aspose.Diagram for .NET:

*   [Home page for Aspose.Diagram API][3].
*   [Aspose.Diagram API wiki docs][4]\- Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][5]\- Post your technical questions, queries and any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][6]\- Do not limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for .NET Examples][7]– We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.
*   [Aspose.Diagram for Java Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   Release Notes ([.NET][9] and [Java][10] – For details on API fixes, please check Release Notes having a complete list of the new features.




[1]: https://downloads.aspose.com/diagram/net/new-releases/aspose.diagram-for-.net-17.10/
[2]: https://downloads.aspose.com/diagram/java/new-releases/aspose.diagram-for-java-17.10/
[3]: https://products.aspose.com/diagram
[4]: https://docs.aspose.com/display/diagramproductfamily/Home
[5]: https://forum.aspose.com/c/diagram
[6]: https://blog.aspose.com/category/aspose-products/aspose-diagram-product-family/
[7]: https://github.com/asposediagram/Aspose_diagram_NET
[8]: https://github.com/asposediagram/Aspose_Diagram_Java
[9]: https://docs.aspose.com/display/diagramnet/Aspose.Diagram+for+.NET+17.10+Release+Notes
[10]: https://docs.aspose.com/display/diagramjava/Aspose.Diagram+for+Java+17.10+Release+Notes)




