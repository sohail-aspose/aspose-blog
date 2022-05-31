---
title: 'Insert Text or Image in XPS using C#'
date: Fri, 15 Apr 2022 20:05:00 +0000
draft: false
url: /2022/04/15/insert-image-text-xps-csharp/
author: 'Farhan Raza'
summary: 'XPS files contain fixed page layout information including the layout, appearance, and printing information for a document. You can **insert some text or image into an XPS file programmatically in C#**.'
tags: ['Insert Image in XPS csharp', 'Insert Picture in XPS csharp', 'Insert Text in XPS csharp']
categories: ['Aspose.Page Product Family']
---



{{< figure align=center src="images/Image-Text-XPS-1024x536.jpg" alt="Insert Text Image XPS C#">}}


[XPS](https://docs.fileformat.com/page-description-language/xps/) files contain fixed page layout information including the layout, appearance, and printing information for a document. You can insert some text or image into an XPS file programmatically in C#.

*   [Insert Text or Image in an XPS Document – C# API Installation](#section0)
*   [Add Text in XPS File using C#](#section1)
*   [Add Text in XPS File using Unicode String in C#](#section2)
*   [Insert Image in XPS Document using C#](#section3)
*   [Place Tiled Image in XPS File using C#](#section4)

## Insert Text or Image in an XPS Document – C# API Installation {#section0}

You can insert text or image in an XPS file without needing to install any word processor or other user-interface application. Simply configure [Aspose.Page for .NET](https://products.aspose.com/page/net) by downloading the DLL files from the [Downloads](https://downloads.aspose.com/page/net) section or using the [NuGet](https://www.nuget.org/packages/Aspose.Page/) installation command below:

```
PM> Install-Package Aspose.Page
```

## Add Text in XPS File using C# {#section1}

You can add any text in an XPS file by following the steps below:

1.  Initialize an object of the [XPSDocument](https://apireference.aspose.com/page/net/aspose.page.xps/xpsdocument) class.
2.  Create a brush of any color and add the glyph.
3.  Save output XPS document.

The following code snippet explains how to add text in an XPS file programmatically in C#:

\[gist id="147ba05f72385c3d1a7b8c795627f369" file="Add Text XPS.cs"\]

## Add Text in XPS File using Unicode String in C# {#section2}

You can also add a Unicode string to the XPS document by following the steps below:

1.  Create an instance of the [XPSDocument](https://apireference.aspose.com/page/net/aspose.page.xps/xpsdocument) class.
2.  Add the Unicode string.
3.  Save the output XPS document.

The following code is based on these steps, which shows how to add text in an XPS file using a Unicode string in C# language:

\[gist id="147ba05f72385c3d1a7b8c795627f369" file="Add Text Unicode XPS.cs"\]

## Insert Image in XPS Document using C# {#section3}

You can insert an image in the XPS document with the following steps:

1.  Create a new XPS Document.
2.  Load input Image.
3.  Create a Matrix and [ImageBrush](https://apireference.aspose.com/page/net/aspose.page.xps/xpsdocument/methods/createimagebrush/index).
4.  Finally, save the output XPS file.

The code example below shows how to insert an image in an XPS document with C#:

\[gist id="147ba05f72385c3d1a7b8c795627f369" file="Insert Image XPS.cs"\]

## Insert Tiled Image in XPS File using C# {#section4}

You can insert the tiled image in the XPS file using C# by following the steps below:

1.  Create a new XPS Document.
2.  Add an [ImageBrush](https://apireference.aspose.com/page/net/aspose.page.xps/xpsdocument/methods/createimagebrush/index)\-filled rectangle and add a tiled image.
3.  Save output XPS document.

The code snippet below elaborates on how to add the tiled image in an XPS file using C#:

\[gist id="147ba05f72385c3d1a7b8c795627f369" file="Insert Tiled Image XPS csharp.cs"\]

## Conclusion

In this article, you have explored how to insert text or images in an XPS document using C#. You can add text as a simple string or a Unicode string as per your requirements. Likewise, an image can be inserted as usual or as a tiled image. Please feel free to visit the [documentation](https://docs.aspose.com/page/net/) section to learn other features of the API. In case of any concerns, please write to us at the [forum](https://forum.aspose.com/c/page).

## See Also

[Convert XPS or OXPS to Word DOCX/DOC in C#](https://blog.aspose.com/2022/02/07/convert-xps-oxps-word-csharp/)



