---
title: 'Create SVG Image File Programmatically using C#'
seoTitle: "Create SVG Image File Programmatically using C# | Embedded HTML"
description: "Create SVG Image File Programmatically using C#. You can also embed HTML content in a SVG file as foreignobject. Create SVG from scratch."
date: Tue, 29 Jun 2021 07:37:00 +0000
draft: false
url: /2021/06/29/create-svg-image-file-programmatically-caharp/
author: Farhan Raza
summary: 'Scalable Vector Graphics (SVG) images are popular for their scalability. They are frequently used over the web for displaying visual information. In this article, you will learn how to create an SVG image file programmatically using C#. The following sections cover different use cases.'
tags: ['create SVG']
categories: ['Aspose.SVG Product Family']
---



{{< figure align=center src="images/create-svg.png" alt="">}}


Scalable Vector Graphics ([SVG][1] images are popular for their scalability. They are frequently used over the web for displaying visual information. In this article, you will learn how to create an SVG image file programmatically using C#. The following sections cover different use cases:

*   [C# SVG Image Creator – API Installation][2]
*   [Create SVG Image File Programmatically with C#][3]
*   [Create SVG Image with Embedded HTML Programmatically using C#][4]

## C# SVG Image Creator – API Installation {#section1}

[Aspose.SVG for .NET][5] API can be used to create, edit, and manipulate SVG image files. You can iterate different nodes or convert the file to supported file formats. Please download the DLL files from the [New Releases][6] section, or use the following NuGet installation commands:

```
PM> Install-Package Aspose.SVG
```

After configuring the API successfully, you can learn how to create a simple and basic SVG image and later you will explore further with the help of an advanced example.

## Create SVG Image File Programmatically with C# {#section2}

1.  You can create an SVG image file with the following steps:
2.  Specify SVG content as a string.
3.  Initialize an object of [SVGDocument][7] class from the string content.
4.  Save the document to a file with the [Save][8] method.

The following code explains how to create an SVG image file programmatically using C#:

\[gist id="43e53ea52673b2211d6023a13b3a3dde" file="create-svg.cs"\]

## Create SVG Image with Embedded HTML Programmatically using C# {#section3}

SVG is consistent with all XML-based languages for describing and rendering of embedded content. You can use <foreignObject> element to include HTML content in an SVG file. Please follow the following steps to create SVG image with embedded HTML:

1.  Specify SVG content with embedded HTML.
2.  Specify the XHTML namespace from which the foreign object originates.
3.  Initialize an SVG document using [SVGDocument][9].
4.  Save the document to a file with [SVGSaveFormat][10] enumeration.

The code below explains how to create an SVG image with embedded HTML content programmatically using C#:

\[gist id="43e53ea52673b2211d6023a13b3a3dde" file="create-SVG-html.cs"\]

## Get Free API License

You can evaluate Aspose APIs without any limitations by requesting a [Free Temporary License][11].

## Conclusion

In this article, you have learned how to create SVG image files from scratch programmatically using C#. You have explored creating a simple SVG image as well as an advanced SVG image with embedded HTML content. You can further explore the API by taking a look at API [Documentation][12]. Moreover, in case of any queries, please feel free to contact us at the [Free Support Forum][13].

## See Also

[Convert SVG to PDF or XPS Programmatically using C# VB.NET][14]



[1]: https://docs.fileformat.com/page-description-language/svg/)
[2]: #section1
[3]: #section2
[4]: #section3
[5]: https://products.aspose.com/svg/net
[6]: https://releases.aspose.com/
[7]: https://apireference.aspose.com/svg/net/aspose.svg/svgdocument
[8]: https://apireference.aspose.com/svg/net/aspose.svg/svgdocument/methods/save/index
[9]: https://apireference.aspose.com/svg/net/aspose.svg/svgdocument
[10]: https://apireference.aspose.com/svg/net/aspose.svg.saving/svgsaveformat
[11]: https://purchase.aspose.com/temporary-license
[12]: https://docs.aspose.com/svg/net/
[13]: https://forum.aspose.com/c/svg/42
[14]: https://blog.aspose.com/2020/12/04/convert-svg-pdf-xps-chsarp-vb-net/





