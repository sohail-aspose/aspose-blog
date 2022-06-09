---
title: 'Compress PNG, JPEG, and TIFF Images using C#'
seoTitle: ""
description: ""
date: Fri, 27 Nov 2020 04:53:55 +0000
draft: false
url: /2020/11/27/compress-png-jpeg-and-tiff-images-using-csharp/
author: Usman Aziz
summary: '[Image compression][1] is a popular way of reducing the size of the images. It lets you minimize the space and time required to store and transmit images respectively. Various compression techniques are available that compress images in such a way that the quality of the images is not degraded. In accordance with that, this post provides you with some simple ways of **how to compress PNG, JPEG, and TIFF images programmatically using C#**.'
tags: ['compress images csharp', 'compress jpeg csharp', 'compress png csharp', 'compress tiff csharp']
categories: ['Aspose.Imaging Product Family']
---

[Image compression][2] is a popular way of reducing the size of the images. It lets you minimize the space and time required to store and transmit images respectively. Various compression techniques are available that compress images in such a way that the quality of the images is not degraded. In accordance with that, this post provides you with some simple ways of **how to compress [PNG][3], [JPEG][4], and [TIFF][5] images programmatically using C#**.

*   [C# Image Compression API - Free Download][6]
*   [Compress PNG Images in C#][7]
*   [Compress JPEG Images in C#][8]
*   [Apply Compression to TIFF Images in C#][9]

## C# Image Compression API - Free Download {#CSharp-Image-Compression-API-Free-Download}

[Aspose.Imaging for .NET][10] is a powerful image processing API that lets you manipulate popular image formats from within your .NET applications. In addition, the API allows you to apply different types of compression to images including PNG, JPEG, and TIFF. In order to use the API, you can either [download][11] its DLL or install it using [NuGet][12].

```
Install-Package Aspose.Imaging
```

## Compress PNG Images in C# {#Compress-PNG-Images-in-CSharp}

For PNG images, you can set the compression level from 0 to 9 where 9 is the maximum compression and 0 is store mode. The following are the steps to compress a PNG image using Aspose.Imaging for .NET.

*   Load the image using [Image][13] class.
*   Create an object of [PngOptions][14] class.
*   Set the compression level using [PngOptions.CompressionLevel][15] property.
*   Save the image using [Image.Save(String, PngOptions)][16] method.

The following code sample shows how to compress PNG images using C#.

{{< gist aspose-imaging b93073a27bcdd4fefc2821e113f0cb3a "Examples-CSharp-ModifyingAndConvertingImages-PNG-CompressingFiles-CompressingFiles.cs" >}}

## Compress JPEG Images in C# {#Compress-JPG-Images-in-CSharp}

In order to deal with JPEG images, Aspose.Imaging for .NET provides [JpegOptions][17] class which offers the following compression types for JPEG images.

*   Baseline
*   Progressive
*   Lossless
*   JpegLs

The following are the steps to compress JPEG images using one of the above-mentioned compression types.

*   Load the JPEG image using [Image][18] class.
*   Create an object of [JpegOptions][19] class.
*   Set the color mode using [JpegOptions.ColorType][20] property.
*   Set compression type using [JpegOptions.CompressionType][21] property.
*   Save the image using [Image.Save(String, JpegOptions)][22] method.

The following code sample shows how to compress a JPEG image using C#.

{{< gist aspose-imaging b93073a27bcdd4fefc2821e113f0cb3a "Examples-CSharp-ModifyingAndConvertingImages-JPEG-ColorTypeAndCompressionType-ColorTypeAndCompressionType.cs" >}}

## Apply Compression on TIFF Images in C# {#Apply-Compression-on-TIFF-Images-in-CSharp}

Aspose.Imaging for .NET provides a [wide range][23] of compression types for TIFF images including LZW, Packbits, CCIT Fax 3 & 4 and etc. You can select the appropriate type as per your requirements. The following are the steps to compress a TIFF image.

*   Load the TIFF image using [Image][24] class.
*   Create an object of [TiffOptions][25] and initialize it with [TiffExpectedFormat.Default][26] enum value.
*   Set [BitsPerSample][27], [Compression][28], [Photometric][29] mode, and [Palette][30] for the Tiff image.
*   Save the image using [Image.Save(String, TiffOptions)][31] method.

The following code sample shows how to compress TIFF images using C#.

{{< gist aspose-imaging b93073a27bcdd4fefc2821e113f0cb3a "Examples-CSharp-ModifyingAndConvertingImages-CompressingTIFFImagesWithLZWAlgorithm-CompressingTIFFImagesWithLZWAlgorithm.cs" >}}

**Info**: Using Aspose [JPG to PPT][32] or [PNG to PPT][33] converter, you can generate PowerPoint presentations from simple images.

## Conclusion

In this post, you have learned how to compress PNG, JPEG, and TIFF images using C#. Various supported compression techniques have also been listed for JPEG and TIFF images. You can explore more about the .NET image processing API using [documentation][34].

## See Also

*   [Convert DICOM to JPEG, GIF, PNG, and BMP Images in C#][35]




[1]: https://en.wikipedia.org/wiki/Image_compression
[2]: https://en.wikipedia.org/wiki/Image_compression
[3]: https://docs.fileformat.com/image/png/
[4]: https://docs.fileformat.com/image/jpeg/
[5]: https://docs.fileformat.com/image/tiff/
[6]: #CSharp-Image-Compression-API-Free-Download
[7]: #Compress-PNG-Images-in-CSharp
[8]: #Compress-JPG-Images-in-CSharp
[9]: #Apply-Compression-on-TIFF-Images-in-CSharp
[10]: https://products.aspose.com/imaging
[11]: https://downloads.aspose.com/imaging
[12]: https://www.nuget.org/packages/Aspose.Imaging
[13]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[14]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/pngoptions
[15]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/pngoptions/properties/compressionlevel
[16]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[17]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/jpegoptions
[18]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[19]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/jpegoptions
[20]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/jpegoptions/properties/colortype
[21]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/jpegoptions/properties/compressiontype
[22]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[23]: https://apireference.aspose.com/imaging/net/aspose.imaging.fileformats.tiff.enums/tiffcompressions
[24]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[25]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/tiffoptions
[26]: https://apireference.aspose.com/imaging/net/aspose.imaging.fileformats.tiff.enums/tiffexpectedformat
[27]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/tiffoptions/properties/bitspersample
[28]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/tiffoptions/properties/compression
[29]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/tiffoptions/properties/photometric
[30]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/tiffoptions/properties/palette
[31]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[32]: https://products.aspose.app/slides/import/jpg-to-ppt
[33]: https://products.aspose.app/slides/import/png-to-ppt
[34]: https://docs.aspose.com/imaging/net/getting-started/
[35]: https://blog.aspose.com/2020/04/01/convert-dicom-to-jpeg-gif-png-bmp-images-in-csharp-net/





