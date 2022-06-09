---
title: 'Inspect, Extract, or Navigate SVG Image Elements Programmatically in C#'
seoTitle: "Inspect, Extract, or Navigate SVG Image Elements Programmatically in C#"
description: "You can inspect, extract, or navigate SVG image file nodes programmatically using C#. It lets you process SVG nodes using XPath Query."
date: Fri, 19 Feb 2021 20:45:00 +0000
draft: false
url: /2021/02/19/inspect-extract-navigate-svg-csharp/
author: Farhan Raza
summary: 'SVG images are popularly used over the web, especially where scalability and quality of images are important. You can inspect, extract, or navigate SVG image elements programmatically with C#.'
tags: ['SVG file and XPath Query', 'SVG file in csharp', 'inspect svg file', 'navigate svg file']
categories: ['Aspose.SVG Product Family']
---



{{< figure align=center src="images/inspect-navigate-svg.png" alt="inspect navigate svg">}}


[SVG][1] images are popularly used over the web, especially where scalability and quality of images are important. You can inspect, extract, or navigate SVG image elements programmatically with C#. Let us explore the following sections for further details:

*   [SVG Inspection or Navigation in C# - API Installation][2]
*   [Inspect SVG Document and its Elements][3]
*   [Extract Information About Specific SVG Elements][4]
*   [Navigate SVG using XPath Query][5]

## SVG Inspection or Navigation in C# - API Installation {#section1}

[Aspose.SVG for .NET][6] API supports creating, editing, or converting SVG files. You can download the DLL file as ZIP from [Downloads][7] section. You can also configure it via NuGet Package Manager in Microsoft Visual Studio. Following NuGet installation command can be used to configure it:

```
PM> Install-Package Aspose.SVG
```

## Inspect SVG Document and its Elements {#section2}

Several methods in Aspose.SVG for .NET API are based on Element Traversal Specifications as per W3C. You can inspect an SVG file in detail with the following steps:

1.  Load the input SVG file.
2.  Load different elements with [DocumentElement][8] object.
3.  Access the value of any property.

The code below explains how to inspect SVG documents and its different elements programmatically using C#:

{{< gist aspose-com-gists 32cf16c0f8fd21b90ab8f787c6af0395 "inspect-SVG.cs" >}}

## Extract Information About Specific SVG Elements {#section3}

An SVG image file consists of several elements under a root element. [SVGDocument][9] class exposes different methods to extract information about specific SVG elements, for instance, [ParentElement][10] and [GetElementsByClassName][11]. Let us follow the steps below for extracting information about specific SVG elements:

1.  Load input SVG image.
2.  Access the [DocumentElement][12] attribute.
3.  Read Any Specific Element.

The following code shows how to extract information about a specific SVG element programmatically using C#:

{{< gist aspose-com-gists 32cf16c0f8fd21b90ab8f787c6af0395 "extract-svg-info.cs" >}}

For this demonstration, we have considered working with [shapes.svg][13] file.

## Navigate SVG using XPath Query {#section4}

XPath query language is used to select nodes from XML based documents. The following steps elaborate how to navigate SVG image file nodes with XPath Query:

*   Load source SVG file.
*   [Evaluate][14] XPath expression.
*   Evaluate and get the next node.

The code below demonstrates how these steps let you navigate SVG nodes programmatically using C# language:

{{< gist aspose-com-gists 32cf16c0f8fd21b90ab8f787c6af0395 "navigate-svg-xpath.cs" >}}

## Conclusion

In this article, we have explored how to inspect the SVG file and its elements. Likewise, extracting information from SVG files and navigating SVG nodes using XPath Query is also discussed. Furthermore, you can learn more by reading the [Documentation][15]. Feel free to reach out at [Free Support Forum][16]. We will be glad to help and guide you!

## See Also

[Load, Save or Merge SVG Images Programmatically in C#][17]




[1]: https://docs.fileformat.com/page-description-language/svg/
[2]: #section1
[3]: #section2
[4]: #section3
[5]: #section4
[6]: https://products.aspose.com/svg/net
[7]: https://releases.aspose.com/
[8]: https://apireference.aspose.com/svg/net/aspose.svg.dom/document/properties/documentelement
[9]: https://apireference.aspose.com/svg/net/aspose.svg/svgdocument
[10]: https://apireference.aspose.com/svg/net/aspose.svg.dom/node/properties/parentelement
[11]: https://apireference.aspose.com/svg/net/aspose.svg.dom/document/methods/getelementsbyclassname
[12]: https://apireference.aspose.com/svg/net/aspose.svg.dom/document/properties/documentelement
[13]: https://www.dropbox.com/s/wku2b7u10pnptod/shapes.svg?dl=0
[14]: https://apireference.aspose.com/svg/net/aspose.svg.dom/document/methods/evaluate
[15]: https://docs.aspose.com/svg/net/
[16]: https://forum.aspose.com/c/svg/42
[17]: https://blog.aspose.com/2021/02/10/load-save-merge-svg-pdf-xps-csharp/





