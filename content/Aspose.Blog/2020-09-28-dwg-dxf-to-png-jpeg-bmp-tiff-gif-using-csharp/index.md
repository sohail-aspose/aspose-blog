---
title: 'Convert DWG/DXF to PNG, JPEG, BMP, TIFF, and GIF Image in C#'
seoTitle: "C# DWG or DXF to PNG JPEG BMP TIFF and GIF Image | C# CAD API"
description: "Use C# .NET CAD API to convert DWG or DXF files to PNG, JPEG, BMP, TIFF, and GIF Image using C# or VB.NET within your .NET applications."
date: Mon, 28 Sep 2020 21:49:00 +0000
draft: false
url: /2020/09/28/dwg-dxf-to-png-jpeg-bmp-tiff-gif-using-csharp/
author: Usman Aziz
summary: 'DWG and DXF are the popular file formats used to store data as well as metadata of the CAD designs. However, it is not possible to directly view or display CAD designs by embedding DWG and DXF files within your web or desktop applications. One of the feasible solutions is CAD to image conversion. This article aims to show you how to convert DWG/DXF files to PNG, JPEG, BMP, TIFF, and GIF images using C#.'
tags: ['DWG or DXF to JPG', 'DWG or DXF to PNG', 'DXG or DXF to BMP GIF TIFF', 'csharp DWG or DXF Converter API']
categories: ['Aspose.CAD Product Family']
---



{{< figure align=center src="images/aspose_cad-for-net.png" alt="DWG DXF to PNG, BMP, JPEG, TIFF, and GIF">}}


[DWG][1] and [DXF][2] are the popular file formats used to store data as well as metadata of the CAD designs. However, it is not possible to directly view or display CAD designs by embedding DWG and DXF files within your web or desktop applications. One of the feasible solutions is CAD to image conversion. This article aims to show you **how to convert DWG/DXF files to [PNG][3], [JPEG][4], **[BMP][5]****, **[TIFF][6], and [GIF][7] images using C#**.

*   [C# DWG or DXF Converter API][8]
*   [C# DWG or DXF to PNG Conversion][9]
*   [DWG or DXF to JPG Conversion in C#][10]
*   [Convert DXG or DXF to BMP, GIF, and TIFF in C#][11]

**Info**: Aspose [Text to GIF][12] converter allows you to create fun animations just by typing.

## C# DWG or DXF to Image Converter API {#CSharp-DWG-or-DXF-Converter-API}

[Aspose.CAD for .NET][13] is a CAD manipulation API that lets you process and convert CAD files using C# or VB.NET. The API provides easy to use methods to convert DWG/DXF designs to raster image formats within a few lines of code. You can [download][14] the API or install it within your .NET applications using [NuGet][15].

## C# DWG or DXF to PNG Conversion {#CSharp-DWG-or-DXF-to-PNG-Conversion}

The following are the steps to convert a DWG or DXF file to PNG image using Aspose.CAD for .NET.

*   Load the DWG/DXF file using [Image][16] class.
*   Create an object of [CadRasterizationOptions][17] class and set the height and width of the resultant image.
*   Create an object of [PngOptions][18] class.
*   Set [PngOptions.VectorRasterizationOptions][19] to _CadRasterizationOptions_ object.
*   Convert CAD to PNG using [Image.Save(String, ImageOptionsBase)][20] method.

The following code sample shows how to convert a DWG file to PNG using C#.

{{< gist aspose-com-gists fa9ce3c2849df7748c9043e827afecf1 "convert-dwg-dxf-to-png.cs" >}}

## DWG or DXF to JPG C# Conversion {#DWG-DXF-to-JPG-Conversion-in-CSharp}

Similar to DWG/DXF to PNG conversion, you can convert the CAD drawings to the JPEG image using Aspose.CAD for .NET. The following are the steps to perform this operation.

*   Use the [Image][21] class to load the DWG/DXF file.
*   Create an object of [CadRasterizationOptions][22] class and set the height and width of the resultant image.
*   Create an object of [JpegOptions][23] class.
*   Set [JpegOptions.VectorRasterizationOptions][24] to _CadRasterizationOptions_ object.
*   Convert CAD to JPEG using [Image.Save(String, ImageOptionsBase)][25] method.

The following code sample shows how to convert CAD DWG/DXF file to JPG using C#.

{{< gist aspose-com-gists fa9ce3c2849df7748c9043e827afecf1 "convert-dwg-dxf-to-jpg.cs" >}}

## DXG or DXF to BMP, TIFF, and GIF using C# {#Convert-DXG-DXF-to-BMP-GIF-TIFF}

In order to convert the DWG/DXF files into BMP, TIFF, or GIF images, you can follow the same steps that you have used above. The only modification would be the usage of [GifOptions][26], [TiffOptions][27], and [BmpOptions][28] classes for conversion to GIF, TIFF, and BMP images respectively. The following code sample shows how to convert a DWG or DXF file to a GIF, TIFF, and BMP image using C#.

{{< gist aspose-com-gists fa9ce3c2849df7748c9043e827afecf1 "convert-dwg-dxf-to-bmp-gif-tiff.cs" >}}

## Conclusion

In this article, you have learned how to convert CAD's DXG or DXF files to PNG, JPEG, BMP, TIFF, and GIF images using C#. Furthermore, you have seen how to set the height and width of the resultant raster image in CAD to image conversion. You can explore more about Aspose's CAD file manipulation API using the [documentation][29].

## See Also

*   [Convert DWG and DXF Files to PDF using C#][30]




[1]: https://docs.fileformat.com/cad/dwg/
[2]: https://docs.fileformat.com/cad/dxf/
[3]: https://docs.fileformat.com/image/png/
[4]: https://docs.fileformat.com/image/jpeg/
[5]: https://docs.fileformat.com/image/bmp/
[6]: https://docs.fileformat.com/image/tiff/
[7]: https://docs.fileformat.com/image/gif/
[8]: #CSharp-DWG-or-DXF-Converter-API
[9]: #CSharp-DWG-or-DXF-to-PNG-Conversion
[10]: #DWG-DXF-to-JPG-Conversion-in-CSharp
[11]: #Convert-DXG-DXF-to-BMP-GIF-TIFF
[12]: https://products.aspose.app/slides/text-to-gif
[13]: https://products.aspose.com/cad/net
[14]: https://downloads.aspose.com/cad/net
[15]: https://www.nuget.org/packages/Aspose.CAD
[16]: https://apireference.aspose.com/cad/net/aspose.cad/image
[17]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/cadrasterizationoptions
[18]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/pngoptions
[19]: https://apireference.aspose.com/cad/net/aspose.cad/imageoptionsbase/properties/vectorrasterizationoptions
[20]: https://apireference.aspose.com/cad/net/aspose.cad.image/save/methods/2
[21]: https://apireference.aspose.com/cad/net/aspose.cad/image
[22]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/cadrasterizationoptions
[23]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/jpegoptions
[24]: https://apireference.aspose.com/cad/net/aspose.cad/imageoptionsbase/properties/vectorrasterizationoptions
[25]: https://apireference.aspose.com/cad/net/aspose.cad.image/save/methods/2
[26]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/gifoptions
[27]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/tiffoptions
[28]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/bmpoptions
[29]: https://docs.aspose.com/cad/net/getting-started/
[30]: https://blog.aspose.com/2020/09/02/convert-autocad-dwg-dxf-to-pdf-using-csharp/





