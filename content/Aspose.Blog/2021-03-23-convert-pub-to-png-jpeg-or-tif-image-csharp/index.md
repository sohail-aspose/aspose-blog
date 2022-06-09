---
title: 'Convert PUB to PNG, JPEG, or TIF Image using C#'
seoTitle: "C# Convert PUB to PNG, JPEG, or TIF Image Programmatically in .NET"
description: "Convert Microsoft Publisher PUB file to Image like PNG, JPEG, TIFF Programmaticaly using C#. Export or change .PUB file to picture or graphic in .NET."
date: Tue, 23 Mar 2021 11:41:00 +0000
draft: false
url: /2021/03/23/convert-pub-to-png-jpeg-or-tif-image-csharp/
author: Farhan Raza
summary: 'Publisher (PUB) files are used for publishing content on large scale. However, limited applications support this file format so you may need an image or thumbnail of the PUB file for a quick preview. You can convert PUB to PNG, JPEG, or TIF image programmatically using C#.'
tags: ['Convert PUB to Image', 'PUB to JPEG in C#', 'PUB to PNG in C#', 'PUB to TIF in C#']
categories: ['Aspose.PUB Product Family']
---



{{< figure align=center src="images/PUB-to-PNG-JPG-TIF-Image.png" alt="PUB to PNG JPEG TIF Image">}}


Microsoft Publisher files are used for publishing content on large scale. However, limited applications support this file format so you might need an image or thumbnail of the PUB file for a quick preview. You can convert [PUB][1] to [PNG][2], [JPEG][3], or [TIF][4] image programmatically using C#. Please check out the following use cases for details:

*   [PUB to Image Conversion – C# APIs Installation][5]
*   [Convert PUB to PNG Image Programmatically with C#][6]
*   [Convert PUB to JPEG Image Programmatically using C#][7]
*   [PUB to TIF Image Conversion Programmatically with C#][8]
*   [Get a Free API License][9]

## PUB to Image Conversion – C# APIs Installation {#section1}

You can convert the PUB files to Image formats like PNG, JPEG, and TIF files. Basically, it is a two-step conversion where you need to convert PUB to PDF and then render it to image formats. Therefore, you need to install [Aspose.PUB for .NET][10] as well as [Aspose.PDF for .NET][11] API in your environment. You can download the DLL files from the [New Releases][12] section, or run the following installation commands to configure APIs from NuGet gallery:

```
PM> Install-Package Aspose.Pdf
PM> Install-Package Aspose.PUB
```

## Convert PUB to PNG Image Programmatically with C# {#section2}

You can convert a PUB file to PNG image with the following steps:

1.  Initialize the [MemoryStream][13] object to hold the PDF file.
2.  Convert PUB to PDF file with [ConvertToPdf()][14] method.
3.  Get page dimensions from the input PDF document.
4.  Create a PNG device using the [PngDevice][15] class object.
5.  Convert PUB to an output PNG image.

The code below explains how to convert PUB file to PNG image programmatically using C#:

{{< gist aspose-com-gists 8e6da8edec616d56815994bc277f389e "convert-pub-to-png.cs" >}}

## Convert PUB to JPEG Image Programmatically using C# {#section3}

Please follow the steps below for converting PUB file to JPEG format with C#:

1.  Declare [MemoryStream][16] class object.
2.  Parse input PUB file with [Parse()][17] method.
3.  Convert PUB to PDF file with [IPdfConverter.ConvertToPdf()][18] method.
4.  Create a Jpeg device with specified Width, Height, and Resolution.
5.  Convert the PUB file and save the output JPEG image.

The following code snippet shows how to convert PUB file to JPEG image programmatically using C#:

{{< gist aspose-com-gists 8e6da8edec616d56815994bc277f389e "convert-pub-to-jpg.cs" >}}

## PUB to TIF Image Conversion Programmatically with C# {#section4}

You can convert PUB file to TIF image format by following the steps below:

1.  Parse input PUB file with [IPubParser.Parse()][19] method.
2.  Convert PUB to PDF file using [IPdfConverter][20] interface.
3.  Create [Resolution][21] object.
4.  Initialize the [TiffDevice][22] class object.
5.  Convert the PUB file to the output TIF image.

The code below demonstrates how to convert PUB file to a TIF image programmatically using C#:

{{< gist aspose-com-gists 8e6da8edec616d56815994bc277f389e "convert-pub-to-tif.cs" >}}

## Get a Free API License {#section0}

You can evaluate the APIs in their full capacity by requesting a free [temporary license][23].

## Conclusion

In this article, you have learned how to convert PUB files to PNG, JPEG, or TIF image formats programmatically using C# language. You may visit the [Documentation][24] for more details and write to us at [Free Support Forum][25], in case of any queries.

## See Also

[Convert PUB to PDF Programmatically in C#][26]




[1]: https://en.wikipedia.org/wiki/PUB_(file_type)
[2]: https://docs.fileformat.com/image/png/
[3]: https://docs.fileformat.com/image/jpeg/
[4]: https://docs.fileformat.com/image/tiff/
[5]: #section1
[6]: #section2
[7]: #section3
[8]: #section4
[9]: #section0
[10]: https://products.aspose.com/pub/net
[11]: https://products.aspose.com/pdf/net
[12]: https://releases.aspose.com/
[13]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream
[14]: https://apireference.aspose.com/pub/net/aspose.pub/ipdfconverter/methods/converttopdf/index
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf.devices/pngdevice
[16]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream
[17]: https://apireference.aspose.com/pub/net/aspose.pub/ipubparser/methods/parse
[18]: https://apireference.aspose.com/pub/net/aspose.pub/ipdfconverter/methods/converttopdf/index
[19]: https://apireference.aspose.com/pub/net/aspose.pub/ipubparser/methods/parse
[20]: https://apireference.aspose.com/pub/net/aspose.pub/ipdfconverter
[21]: https://apireference.aspose.com/pdf/net/aspose.pdf.devices/resolution
[22]: https://apireference.aspose.com/pdf/net/aspose.pdf.devices/tiffdevice
[23]: https://purchase.aspose.com/temporary-license
[24]: https://docs.aspose.com/pdf/net/converting/
[25]: https://forum.aspose.com/c/pub
[26]: https://blog.aspose.com/2021/01/13/convert-pub-pdf-csharp/





