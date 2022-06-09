---
title: 'Convert EPS to PNG or PDF using C#'
seoTitle: ""
description: ""
date: Mon, 21 Sep 2020 16:49:28 +0000
draft: false
url: /2020/09/21/convert-eps-to-png-or-pdf-using-csharp/
author: Usman Aziz
summary: 'EPS (Encapsulated PostScript) is a graphics file format that is used to describe images or drawings. In various scenarios, EPS images are also used to be placed within another PostScript document. EPS contains an encapsulated low-resolution preview, however, you may come across the need of converting EPS images to a format that could easily be displayed without any dependency. For such cases, this article covers how to convert EPS to PNG or PDF using C#.'
tags: ['EPS Converter API', 'convert EPS to PDF csharp', 'convert EPS to PNG csharp']
categories: ['Aspose.Imaging Product Family']
---

[EPS][1] (Encapsulated PostScript) is a graphics file format that is used to describe images or drawings. In various scenarios, EPS images are also used to be placed within another PostScript document. EPS contains an encapsulated low-resolution preview, however, you may come across the need of converting EPS images to a format that could easily be displayed without any dependency. For such cases, this article covers **how to convert EPS to [PNG][2] or [PDF][3] using C#**.

*   [C# EPS to PNG or PDF Converter API][4]
*   [EPS to PNG Conversion using C#][5]
*   [EPS to PDF Conversion using C#][6]

## C# EPS to PNG or PDF Converter API {#CSharp-EPS-to-PNG-or-PDF-Converter-API}

[Aspose.Imaging for .NET][7] is an image processing and manipulation API that lets you work with EPS images within your .NET applications. It provides easy to use methods to convert EPS files to PNG images or PDF documents seamlessly. You can either [download][8] API's DLL or install it using [NuGet][9].

```
PM> Install-Package Aspose.Imaging
```

## EPS to PNG C# Conversion {#EPS-to-PNG-Conversion-using-CSharp}

Aspose.Imaging for .NET provides [PngOptions][10] class that allows you to control EPS to PNG conversion with different options. The following are the steps to convert an EPS image to PNG.

*   Load the EPS file using [Image.Load(String)][11] method.
*   Create an object of [PngOptions][12] class and set its options such as image's height and width.
*   Convert EPS to PNG using [Image.Save(String, ImageOptionsBase)][13] method.

The following code sample shows how to convert an EPS file to PNG using C#.

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "Examples-Convert-Eps-To-Png.cs" >}}

### EPS to PNG



{{< figure align=center src="images/EpsToPng-1024x542.png" alt="EPS to PNG">}}


## EPS to PDF C# Conversion {#EPS-to-PDF-Conversion-using-CSharp}

Similar to the PngOptions, Aspose.Imaging provides PdfOptions class for controlling EPS to PDF conversion. The following are the steps to convert an EPS image to a PDF.

*   Load the EPS file using [Image.Load(String)][14] method.
*   Create an object of [PdfOptions][15] class and set its options such as PDF compliance version.
*   Convert EPS to PDF using [Image.Save(String, ImageOptionsBase)][16] method.

The following code sample shows how to convert EPS to PDF using C#.

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "Examples-Convert-Eps-To-Pdf.cs" >}}

### EPS to PDF



{{< figure align=center src="images/EpsToPdf-1024x547.png" alt="EPS to PDF">}}


## Conclusion

In this article, you have learned how to convert EPS images to PNG or PDF format using C#. The step by step guide and code samples also showed how to customize EPS to PNG/PDF conversion using Aspose.Imaging for .NET. You can explore more about the API using the [documentation][17].

## See Also

*   [Create Clipping Path in TIFF Images using C#][18]




[1]: https://docs.fileformat.com/page-description-language/eps/
[2]: https://docs.fileformat.com/image/png/
[3]: https://docs.fileformat.com/pdf/
[4]: #CSharp-EPS-to-PNG-or-PDF-Converter-API
[5]: #EPS-to-PNG-Conversion-using-CSharp
[6]: #EPS-to-PDF-Conversion-using-CSharp
[7]: https://products.aspose.com/imaging/net
[8]: https://downloads.aspose.com/imaging/net
[9]: https://www.nuget.org/packages/Aspose.Imaging
[10]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/pngoptions
[11]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/load/methods/2
[12]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/pngoptions
[13]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[14]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/load/methods/2
[15]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/pdfoptions
[16]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[17]: https://docs.aspose.com/imaging/net/getting-started/
[18]: https://blog.aspose.com/2020/08/31/create-clipping-path-in-tiff-images-using-csharp/





