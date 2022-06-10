---
title: 'Retrieve Char Elements of Master Inherited by the Visio Shape in C#'
date: Sun, 25 Feb 2018 18:40:25 +0000
draft: false
url: /2018/02/25/retrieve-char-elements-of-master-inherited-by-the-shape-with-aspose.diagram-18.2-api/
author: Imran Rafique
summary: ''
tags: []
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose-Diagram-for-net_100.png" alt="Aspose.Diagram for .NET logo">}}


We are pleased to announce that the new version 18.1 of Aspose.Diagram API is now live. The recent version 18.2 has added support of retrieving Char elements of Master with the Shape instance. The Shape is an extended form of Master and developers can retrieve text formatting using Char elements of the Master with a Shape instance. The recent version 18.2 also covers enhancements and regular bug fixes. We recommend our client to incorporate the latest upgrade of Aspose.Diagram API to take benefit of improved functionality and bug fixes. Please use the following links for downloading Aspose.Diagram for .NET and Java assemblies.

*   [Aspose.Diagram for .NET 18.2][1]
*   [Aspose.Diagram for Java 18.2][2]

## Retrieve a collection of inherited Char elements

The Char elements define the formatting of the shape's text, and a Shape instance has a collection of Char elements inherited from the Master. Developers can retrieve these inherited Char elements with InheritChars member of the Shape class as follows:  
**C#**

```
// shape is the instance of Aspose.Diagram.Shape classCharCollection charCollection = shape.InheritChars;
```

**Java**

```
// shape is the instance of com.aspose.diagram.Shape classCharCollection charCollection = shape.getInheritChars();
```

## Aspose.Diagram for .NET and Java Resources

The following resources will help you work with Aspose.Diagram for .NET:

*   [Home page for Aspose.Diagram API][3].
*   [Aspose.Diagram API wiki docs][4]\- Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][5]\- Post your technical questions, queries and any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][6]\- Do not limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for .NET Examples][7]– We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.
*   [Aspose.Diagram for Java Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   Release Notes ([.NET][9] and [Java][10] – For details on API fixes, please check Release Notes having a complete list of the new features.




[1]: https://www.nuget.org/packages/Aspose.Diagram/18.2.0
[2]: http://maven.aspose.com/artifactory/simple/ext-release-local/com/aspose/aspose-diagram/18.2/
[3]: http://www.aspose.com/products/diagram
[4]: https://docs.aspose.com/display/diagramproductfamily/Home
[5]: https://forum.aspose.com/c/diagram
[6]: https://blog.aspose.com/category/aspose-products/aspose-diagram-product-family/
[7]: https://github.com/asposediagram/Aspose_diagram_NET
[8]: https://github.com/asposediagram/Aspose_Diagram_Java
[9]: https://docs.aspose.com/display/diagramnet/Aspose.Diagram+for+.NET+18.2+Release+Notes
[10]: https://docs.aspose.com/display/diagramjava/Aspose.Diagram+for+Java+18.2+Release+Notes)




