---
title: 'Convert PSD to PDF, JPG, PNG and Other Raster Image Formats in C#'
seoTitle: ""
description: ""
date: Fri, 27 Mar 2020 15:57:22 +0000
draft: false
url: /2020/03/27/convert-psd-to-pdf-jpg-png-tiff-gif-bmp-jp2-in-csharp-net/
author: Usman Aziz
summary: ''
tags: ['Convert PSD Files in Csharp .NET', 'PSD to BMP', 'PSD to GIF', 'PSD to JP2', 'PSD to JPG', 'PSD to PDF', 'PSD to PNG', 'PSD to TIFF']
categories: ['Aspose.PSD Product Family']
---



{{< figure align=center src="images/PSD-to-Image-C-2.png" alt="PSD to Image C# 2">}}


The **Photoshop Document** ([PSD][1] is a well-known file format used by **Adobe Photoshop** for saving the data in the form of layers. The layers are combined together to obtain the desired artwork or images. Adobe Photoshop allows the designers to export the PSD layers as a single image in the form of PNG, JPG, GIF, TIFF, and other formats.

In case you want to implement the feature of converting or exporting the PSD files to raster image formats without Photoshop, you will definitely look for some automation. For such a case, I am going to demonstrate how to **convert PSD to PDF, JPG, PNG, BMP** or other raster image formats programmatically using C#. Furthermore, you'll also learn how to convert or export the desired layer/layer group in the PSD. This article covers the following PSD conversions in C#:

*   PSD to JPG
*   PSD to PNG
*   PSD to BMP
*   PSD to TIFF
*   PSD to GIF
*   PSD to JP2
*   PSD to PDF
*   PSD layer/layer group to image

## C# PSD Converter API - Aspose.PSD for .NET

For converting PSD to PDF and image formats, we'll leverage the capabilities of [Aspose.PSD for .NET][2] which is simple and easy to use .NET API for manipulation and conversion of Photoshop files (PSD). In addition to conversion features, the API also lets you create and edit the Photoshop PSD files, update layer properties, insert watermarks, and perform various graphics-related operations on PSD files. Aspose.PSD for .NET can be installed from [NuGet][3] as well as downloaded as DLL from the [Downloads][4] section.

## Convert PSD to JPG in C#

The following are the steps to convert a PSD file to JPG image in C#:

*   Create an object of the [Image][5] class and initialize it with the PSD file's path.
*   Create an object of the [JpegOptions][6] class.
*   Convert PSD to JPG using [Image.Save(string, JpegOptions)][7] method.

The following code sample shows how to convert a PSD file to JPG in C#:

{{< gist aspose-com-gists 98c65d2d8b648bfa7db9d8213b61a31c "convert-psd-to-jpg.cs" >}}

### PSD File



{{< figure align=center src="images/PSD-File.png" alt="PSD to JPG">}}


### Converted JPG Image



{{< figure align=center src="images/PSD-to-JPG.png" alt="PSD to PNG">}}


## Convert PSD to PNG in C#

The following are the steps to convert a PSD file to PNG image in C#:

*   Create an object of the [Image][8] class and initialize it with the PSD file's path.
*   Create an object of the [PngOptions][9] class.
*   Convert PSD to PNG using [Image.Save(string, PngOptions)][10] method.

The following code sample shows how to convert a PSD file to PNG in C#:

{{< gist aspose-com-gists 98c65d2d8b648bfa7db9d8213b61a31c "convert-psd-to-png.cs" >}}

## Convert PSD to BMP in C#

The following are the steps to convert a PSD file to BMP image in C#:

*   Create an object of the [Image][11] class and initialize it with the PSD file's path.
*   Create an object of the [BmpOptions][12] class.
*   Convert PSD to BMP using [Image.Save(string, BmpOptions)][13] method.

The following code sample shows how to convert a PSD file to BMP in C#:

{{< gist aspose-com-gists 98c65d2d8b648bfa7db9d8213b61a31c "convert-psd-to-bmp.cs" >}}

## Convert PSD to TIFF in C#

The following are the steps to convert a PSD file to TIFF image in C#:

*   Create an object of the [Image][14] class and initialize it with the PSD file's path.
*   Create an object of the [TiffOptions][15] class.
*   Convert PSD to TIFF using [Image.Save(string, TiffOptions)][16] method.

The following code sample shows how to convert a PSD file to TIFF in C#:

{{< gist aspose-com-gists 98c65d2d8b648bfa7db9d8213b61a31c "convert-psd-to-tiff.cs" >}}

## Convert PSD to GIF in C#

The following are the steps to convert a PSD file to GIF image in C#:

*   Create an object of the [Image][17] class and initialize it with the PSD file's path.
*   Create an object of the [GifOptions][18] class.
*   Convert PSD to GIF using [Image.Save(string, GifOptions)][19] method.

The following code sample converts a PSD file to GIF in C#:

{{< gist aspose-com-gists 98c65d2d8b648bfa7db9d8213b61a31c "convert-psd-to-gif.cs" >}}

## Convert PSD to JP2 in C#

The following are the steps to convert a PSD file to JP2 image in C#:

*   Create an object of the [Image][20] class and initialize it with the PSD file's path.
*   Create an object of the [Jpeg2000Options][21] class.
*   Convert PSD to JP2 using [Image.Save(string, Jpeg2000Options)][22] method.

The following code sample converts a PSD file to JP2 in C#:

{{< gist aspose-com-gists 98c65d2d8b648bfa7db9d8213b61a31c "convert-psd-to-jp2.cs" >}}

## Convert PSD to PDF in C#

The following are the steps to convert a PSD file to PDF document in C#:

*   Create an object of the [Image][23] class and initialize it with the PSD file's path.
*   Create an object of the [PdfOptions][24] class.
*   Convert PSD to PDF document using [Image.Save(string, PdfOptions)][25] method.

The following code sample converts a PSD file to PDF document in C#:

{{< gist aspose-com-gists 98c65d2d8b648bfa7db9d8213b61a31c "convert-psd-to-pdf.cs" >}}

## Convert a Layer or Layer Group of PSD in C#

You can also convert a particular layer or layer group in the PSD file to raster image formats (JPG, PNG, etc.). The following are the steps to perform this operation.

*   Create an object of the [PsdImage][26] class and load the PSD file.
*   Access the layer or layer group using [PsdImage.Layers][27] array.
*   Render the layer as an image.

The following code sample shows how to convert a layer group of PSD to PNG in C#.

{{< gist aspose-com-gists 98c65d2d8b648bfa7db9d8213b61a31c "convert-psd-layer-to-image.cs" >}}

## Learn more about Aspose.PSD for .NET

You can explore more about the Aspose.PSD for .NET using the [documentation][28].

## Related Article(s)

*   [Convert PowerPoint to JPG Images in C#][29]




[1]: https://wiki.fileformat.com/image/psd/)
[2]: https://products.aspose.com/psd/net
[3]: http://nuget.org/packages/aspose.psd
[4]: https://products.aspose.com/psd/net
[5]: https://apireference.aspose.com/net/psd/aspose.psd/image
[6]: https://apireference.aspose.com/net/psd/aspose.psd.imageoptions/jpegoptions
[7]: https://apireference.aspose.com/net/psd/aspose.psd.image/save/methods/3
[8]: https://apireference.aspose.com/net/psd/aspose.psd/image
[9]: https://apireference.aspose.com/net/psd/aspose.psd.imageoptions/pngoptions
[10]: https://apireference.aspose.com/net/psd/aspose.psd.image/save/methods/3
[11]: https://apireference.aspose.com/net/psd/aspose.psd/image
[12]: https://apireference.aspose.com/net/psd/aspose.psd.imageoptions/bmpoptions
[13]: https://apireference.aspose.com/net/psd/aspose.psd.image/save/methods/3
[14]: https://apireference.aspose.com/net/psd/aspose.psd/image
[15]: https://apireference.aspose.com/net/psd/aspose.psd.imageoptions/tiffoptions
[16]: https://apireference.aspose.com/net/psd/aspose.psd.image/save/methods/3
[17]: https://apireference.aspose.com/net/psd/aspose.psd/image
[18]: https://apireference.aspose.com/net/psd/aspose.psd.imageoptions/gifoptions
[19]: https://apireference.aspose.com/net/psd/aspose.psd.image/save/methods/3
[20]: https://apireference.aspose.com/net/psd/aspose.psd/image
[21]: https://apireference.aspose.com/net/psd/aspose.psd.imageoptions/jpeg2000options
[22]: https://apireference.aspose.com/net/psd/aspose.psd.image/save/methods/3
[23]: https://apireference.aspose.com/net/psd/aspose.psd/image
[24]: https://apireference.aspose.com/net/psd/aspose.psd.imageoptions/pdfoptions
[25]: https://apireference.aspose.com/net/psd/aspose.psd.image/save/methods/3
[26]: https://apireference.aspose.com/net/psd/aspose.psd.fileformats.psd/psdimage
[27]: https://apireference.aspose.com/net/psd/aspose.psd.fileformats.psd/psdimage/properties/layers
[28]: http://docs.aspose.com/display/psdnet
[29]: https://blog.aspose.com/2020/02/07/convert-powerpoint-ppt-pptx-to-jpg-images-in-csharp-net/





