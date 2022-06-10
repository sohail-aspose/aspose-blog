---
title: 'Move Page Position in Visio Drawing using C# and Java'
date: Mon, 26 Mar 2018 07:15:10 +0000
draft: false
url: /2018/03/26/move-page-position-in-visio-drawing-using-csharp-and-java/
author: Imran Rafique
summary: ''
tags: []
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose-Diagram-for-net_100.png" alt="Aspose.Diagram for .NET logo">}}


We are pleased to announce that the new version 18.3 of [Aspose.Diagram][1] API is now live. The recent version 18.3 has added support of changing the position of Page in Visio drawings, and the export of the VSD to XPS has been improved. The recent version 18.3 also covers enhancements and regular bug fixes. We recommend our client to incorporate the latest upgrade of Aspose.Diagram API to take benefit of improved functionality and bug fixes. Please use the following links for downloading Aspose.Diagram for .NET and Java assemblies.

*   [Aspose.Diagram for .NET 18.3][2]
*   [Aspose.Diagram for Java 18.3][3]

## Move Page Position in Visio Diagrams

Developers can add a new page to the target page index, and they can also change the position of an existing page in the Visio drawing. Developers can change the position of the Page with MoveTo member of the Page class as follows:

### C#```
// import diagram Diagram diagram = new Diagram(dataDir + "Drawing1.vsdx"); Page newPage = new Page(1); // move page in the diagram 
newPage.MoveTo(2); diagram.Save(dataDir + "Drawing1.vsdx", SaveFileFormat.VSDX);
```

### Java```
// import diagramDiagram diagram = new Diagram(dataDir + "Drawing1.vsdx");
Page newPage = new Page(1);// move page in the diagram
newPage.moveTo(2);
diagram.save(dataDir + "Drawing1.vsdx", SaveFileFormat.VSDX);
```

## Aspose.Diagram for .NET and Java Resources

The following resources will help you work with Aspose.Diagram for .NET:

*   [Home page for Aspose.Diagram API][4].
*   [Aspose.Diagram API wiki docs][5]\- Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][6]\- Post your technical questions, queries and any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][7]\- Do not limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for .NET Examples][8]– We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.
*   [Aspose.Diagram for Java Examples][9] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   Release Notes ([.NET][10] and [Java][11] – For details on API fixes, please check Release Notes having a complete list of the new features.




[1]: https://products.aspose.com/diagram
[2]: https://www.nuget.org/packages/Aspose.Diagram/18.3.0
[3]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-diagram/18.3/
[4]: http://www.aspose.com/products/diagram
[5]: https://docs.aspose.com/display/diagramproductfamily/Home
[6]: https://forum.aspose.com/c/diagram
[7]: https://blog.aspose.com/category/aspose-products/aspose-diagram-product-family/
[8]: https://github.com/asposediagram/Aspose_diagram_NET
[9]: https://github.com/asposediagram/Aspose_Diagram_Java
[10]: https://docs.aspose.com/display/diagramnet/Aspose.Diagram+for+.NET+18.3+Release+Notes
[11]: https://docs.aspose.com/display/diagramjava/Aspose.Diagram+for+Java+18.3+Release+Notes)




