---
title: 'Convert GIF Images to TIFF, PDF, PNG, JPG, or BMP using C#'
seoTitle: ""
description: ""
date: Wed, 10 Jun 2020 17:45:06 +0000
draft: false
url: /2020/06/10/convert-gif-images-to-tiff-pdf-png-jpg-or-bmp-using-csharp/
author: Usman Aziz
summary: ''
tags: ['convert GIF to BMP in csharp', 'convert GIF to JPG in csharp', 'convert GIF to PDF in csharp', 'convert GIF to PNG in csharp', 'convert GIF to TIFF in csharp']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose-Imaging-for-net_100.png" alt="Convert animated GIF using C#">}}


Animated [GIF][1] (Graphics Interchange Format) contains a number of image frames in a particular order within a single file. These frames are shown in a sequence to create the animation. There could be various use cases when you need to convert animated GIFs to other multi-page or raster image formats. The multi-page formats include TIFF as well as PDF whereas raster images could be PNG, JPG, BMP and etc. In this article, I'll show you how to convert animated GIF images to TIFF, PDF, PNG. JPG, and BMP images programmatically using C#. The code samples provided in this article can easily be ported to VB.NET as well.

*   [Convert animated GIF to TIFF using C#][2]
*   [Convert animated GIF to PDF using C#][3]
*   [Extract and convert a frame of GIF to PNG using C#][4]
*   [Convert a GIF frame to JPG using C#][5]
*   [Convert a GIF frame to BMP using C#][6]

**Info**: You may want to check out the FREE [Text to GIF Converter][7] Aspose recently developed.

## C# GIF Converter API

[Aspose.Imaging for .NET][8] is a feature-rich API that supports manipulating a wide range vector or raster image formats including the animated GIFs. It allows converting animated GIF to other multi-page formats as well as raster images within the .NET application. You can install the API using [NuGet Package Manager][9] or download and reference its [DLL][10] file manually.

## Convert Animated GIF to TIFF using C# {#Convert-animated-GIF-to-TIFF-using-CSharp}

TIFF is a multi-page image format that keeps multiple images within a single file. Since the animated GIF also contains a sequence of frames, you can export all or selected frames to the TIFF format. In this conversion, each frame in GIF will be converted to a page in the TIFF image. The following are the steps to convert an animated GIF to TIFF format using Aspose.Imaging for .NET.

*   Load a GIF image into [Image][11] object using [Image.Load(String)][12] method.
*   Use the [MultiPageOptions][13] class to specify the range of frames you want to convert (optional).
*   Convert GIF to TIFF using [Image.Save(String, TiffOptions)][14] method.

The following code sample shows how to convert GIF to TIFF using C#.

{{< gist aspose-com-gists b8ed72ac8b5ad3f06e103a003c6c8e78 "gif-to-tiff.cs" >}}

## Convert Animated GIF to PDF using C# {#Convert-animated-GIF-to-PDF-using-CSharp}

In an animated GIF to PDF conversion, each frame of the GIF is converted into a separated page within the PDF. Just like GIF to TIFF, you can specify the range of frames you want to get in the converted PDF file. The following are the steps to convert an animated GIF to PDF.

*   Create an instance of [Image][15] class and load the animated GIF file.
*   Use the [MultiPageOptions][16] class to specify the range of frames (optional).
*   Save the image as PDF using [Image.Save(String, PdfOptions)][17] method.

The following code sample shows how to convert animated GIF to PDF using C#.

{{< gist aspose-com-gists b8ed72ac8b5ad3f06e103a003c6c8e78 "gif-to-pdf.cs" >}}

## Convert a GIF Frame to PNG, JPG, or BMP using C#

Since animated GIF contains a sequence of frames, you can extract the desired frame and convert it to raster images such as PNG, JPG, BMP, etc.

### Convert GIF Frame to PNG using C# {#Extract-and-convert-a-frame-of-animated-GIF-to-PNG-using-CSharp}

The following are the steps to convert a GIF frame to a PNG image.

*   Load the animated GIF image using [Image.Load(String)][18] method.
*   Convert the GIF frame to PNG using [Image.Save(String, PngOptions)][19] method by specifying the frame number.

The following code sample shows how to convert a frame of an animated GIF to PNG using C#.

{{< gist aspose-com-gists b8ed72ac8b5ad3f06e103a003c6c8e78 "gif-to-png.cs" >}}

### Convert GIF Frame to JPG using C# {#Convert-a-GIF-frame-to-JPEG-using-CSharp}

Aspose.Imaging exposes [JpegOptions][20] class to set the options while converting a GIF frame to the JPG image. The following code sample shows how to convert a frame in GIF to JPG using C#.

{{< gist aspose-com-gists b8ed72ac8b5ad3f06e103a003c6c8e78 "gif-to-jpg.cs" >}}

### Convert GIF Frame to BMP using C# {#Convert-a-GIF-frame-to-BMP-using-CSharp}

For GIF to BMP conversion, the API provides the [BmpOptions][21] class. The following code sample shows how to convert a GIF frame to BMP using C#.

{{< gist aspose-com-gists b8ed72ac8b5ad3f06e103a003c6c8e78 "gif-to-bmp.cs" >}}

## Conclusion

In this article, you have learned how to convert an animated GIF to multipage formats such as TIFF and PDF using C#. Furthermore, we have seen how to extract a particular frame from the animated GIF and convert it to the PNG, JPG, or BMP images. You can explore more about Aspose.Imaging for .NET using the [documentation][22].

## See Also

*   [Convert DICOM to JPEG, GIF, PNG, and BMP using C#][23]




[1]: https://wiki.fileformat.com/image/gif/
[2]: #Convert-animated-GIF-to-TIFF-using-CSharp
[3]: #Convert-animated-GIF-to-PDF-using-CSharp
[4]: #Extract-and-convert-a-frame-of-animated-GIF-to-PNG-using-CSharp
[5]: #Convert-a-GIF-frame-to-JPEG-using-CSharp
[6]: #Convert-a-GIF-frame-to-BMP-using-CSharp
[7]: https://products.aspose.app/slides/text-to-gif
[8]: https://products.aspose.com/imaging/net
[9]: http://nuget.org/packages/Aspose.imaging
[10]: https://downloads.aspose.com/imaging/net
[11]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[12]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/canload/methods/2
[13]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/multipageoptions
[14]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[15]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[16]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/multipageoptions
[17]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[18]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/canload/methods/2
[19]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[20]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/jpegoptions
[21]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/bmpoptions
[22]: https://docs.aspose.com/display/imagingnet/Introduction
[23]: https://blog.aspose.com/2020/04/01/convert-dicom-to-jpeg-gif-png-bmp-images-in-csharp-net/





