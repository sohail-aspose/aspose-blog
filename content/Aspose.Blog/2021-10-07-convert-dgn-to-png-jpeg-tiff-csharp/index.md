---
title: 'Convert DGN to JPEG, PNG, or TIFF Image in C#'
seoTitle: "Convert DGN to JPEG, PNG, or TIFF Image Programmatically in C#"
description: "Convert DGN file to PNG, JPEG, or TIFF image programmatically using C#. DGN Converter in .NET framework based applications."
date: Thu, 07 Oct 2021 14:23:00 +0000
draft: false
url: /2021/10/07/convert-dgn-to-png-jpeg-tiff-csharp/
author: Farhan Raza
summary: 'DGN files are two-dimensional or three-dimensional (2D/3D) drawings that are usually supported by construction CAD applications. You may need to convert it to an image for previewing it in more system environments. This article covers DGN to JPEG, PNG, or TIFF image conversion with all the important details.'
tags: ['Convert DGN file csharp', 'DGN to Image', 'DGN to Image csharp', 'DGN to JPG', 'DGN to PNG', 'DGN to TIFF']
categories: ['Aspose.CAD Product Family']
---



{{< figure align=center src="images/DGN-to-PNG-JPG-TIFF.jpg" alt="DGN to JPG, PNG, TIFF">}}


DGN files are two-dimensional or three-dimensional (2D/3D) drawings supported by construction CAD applications. In certain cases, you may need to convert a DGN file to an image for previewing it in different system environments. This article covers how to convert [DGN][1] to [JPEG][2], [PNG][3], or [TIFF][4] image with all the important details:

*   [DGN to JPEG, PNG, or TIFF Image Converter – C# API Installation][5]
*   [Convert DGN File to JPEG Image Programmatically with C#][6]
*   [Convert DGN to PNG Image Programmatically using C#][7]
*   [DGN to TIFF Image Conversion Programmatically in C#][8]

## DGN to JPEG, PNG, or TIFF Image Converter – C# API Installation {#section1}

[Aspose.CAD for .NET][9] API supports creating, editing, and manipulating DGN files and [several other][10] file formats. You can configure the API by downloading the DLL file from the [New Releases][11], or using the following [NuGet][12] installation command:

```
PM> Install-Package Aspose.CAD
```

## Convert DGN File to JPEG Image Programmatically with C# {#section2}

You can convert a DGN file to a JPEG image with the following steps:

1.  Load input DGN file using the [Image][13] class.
2.  Initialize an object of [CadRasterizationOptions][14] class.
3.  Create an instance of [JpegOptions][15] class.
4.  Convert the DGN to a JPG image with the [Save][16] method.

The following code snippet shows how to convert a DGN file to a JPEG image programmatically using C#:

{{< gist aspose-com-gists 412be21b594854e6ab040987c3c498b2 "DGN-to-JPG.cs" >}}

## Convert DGN to PNG Image Programmatically using C# {#section3}

You can convert a DGN file to a PNG image with the steps below:

1.  Load input DGN file with the [Image][17] class.
2.  Create an instance of [CadRasterizationOptions][18] and set image height & width.
3.  Create an instance of [PngOptions][19] and set [VectorRasterizationOptions][20].
4.  Convert the DGN to a PNG Image using [Image.Save][21] method.

The code sample below explains how to convert a DGN file to a PNG image programmatically with C#:

{{< gist aspose-com-gists 412be21b594854e6ab040987c3c498b2 "DGN-to-PNG.cs" >}}

## DGN to TIFF Image Conversion Programmatically in C# {#section4}

You can convert a DGN file to a TIFF image with the below steps:

1.  Load input DGN file using the [Image][22] class.
2.  Initialize an object of [CadRasterizationOptions][23] class.
3.  Create an instance of [TiffOptions][24] type.
4.  Set the [VectorRasterizationOptions][25] property.
5.  Convert the DGN to a TIFF image with the [Save][26] method.

The following code snippet shows how to convert a DGN file to a TIFF image programmatically in C#:

{{< gist aspose-com-gists 412be21b594854e6ab040987c3c498b2 "DGN-to-TIFF.cs" >}}

## Get Free Temporary License

You can evaluate the API without any limitations by requesting a [Free Temporary License][27].

## Conclusion

In this article, you have learned how to convert a DGN file to different image formats like JPEG, PNG, or TIFF programmatically using C#. You can take a look at several other features of the API by visiting the [Documentation][28]. In case of any queries, please get in touch with us at the [Free Support Forum][29].

## See Also

[Convert IGS IGES File to PDF Programmatically using C#][30]

[Convert STL to PDF or PNG Image Programmatically in C#][31]




[1]: https://docs.fileformat.com/cad/dgn/
[2]: https://docs.fileformat.com/image/jpeg/
[3]: https://docs.fileformat.com/image/png/
[4]: https://docs.fileformat.com/image/tiff/
[5]: #section1
[6]: #section2
[7]: #section3
[8]: #section4
[9]: https://products.aspose.com/cad/net/
[10]: https://docs.aspose.com/cad/net/supported-file-formats/
[11]: https://releases.aspose.com/
[12]: https://www.nuget.org/packages/Aspose.CAD/
[13]: https://apireference.aspose.com/cad/net/aspose.cad/image
[14]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/cadrasterizationoptions
[15]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/jpegoptions
[16]: https://apireference.aspose.com/cad/net/aspose.cad/image/methods/save/index
[17]: https://apireference.aspose.com/cad/net/aspose.cad/image
[18]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/cadrasterizationoptions
[19]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/pngoptions
[20]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/vectorrasterizationoptions
[21]: https://apireference.aspose.com/cad/net/aspose.cad/image/methods/save/index
[22]: https://apireference.aspose.com/cad/net/aspose.cad/image
[23]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/cadrasterizationoptions
[24]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/tiffoptions
[25]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/vectorrasterizationoptions
[26]: https://apireference.aspose.com/cad/net/aspose.cad/image/methods/save/index
[27]: https://purchase.aspose.com/temporary-license
[28]: https://docs.aspose.com/cad/net/
[29]: https://forum.aspose.com/c/cad
[30]: https://blog.aspose.com/2021/09/08/convert-igs-iges-file-to-pdf-csharp/
[31]: https://blog.aspose.com/2021/02/12/convert-stl-to-pdf-png-image-programmatically-csharp/




