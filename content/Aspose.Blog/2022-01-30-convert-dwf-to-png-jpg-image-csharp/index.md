---
title: 'Convert DWF to PNG or JPG Image in C#'
date: Sun, 30 Jan 2022 08:15:00 +0000
draft: false
url: /2022/01/30/convert-dwf-to-png-jpg-image-csharp/
author: 'Farhan Raza'
summary: 'DWF files are based on vectors that can consist of CAD drawings, text, images, etc. You may need to create a thumbnail or preview image of a DWF file. In accordance with that, the article covers how to **convert a DWF file to a JPG or PNG image programmatically in C#**.'
tags: ['Convert DWF in csharp', 'DWF to Image', 'DWF to JPG', 'DWF to PNG', 'DWF to PNG csharp']
categories: ['Aspose.CAD Product Family']
---



{{< figure align=center src="images/DWF-to-JPG-PNG.jpg" alt="DWF to PNG JPG Image C#">}}


[DWF][1] files are based on vectors that can consist of CAD drawings, text, images, etc. You may need to create a thumbnail or preview image of a DWF file. In accordance with that, the article covers how to convert a DWF file to a [JPG][2] or [PNG][3] image programmatically in C#.

*   [DWF to JPG or PNG Image Converter – C# API Installation][4]
*   [Convert DWF to JPG Image Programmatically in C#][5]
*   [Convert DWF to PNG Image Programmatically in C#][6]

## DWF to JPG or PNG Image Converter – C# API Installation {#section1}

[Aspose.CAD for .NET][7] API supports converting DWF and [several other][8] file formats. You can easily configure the API by downloading its DLL file from the [New Releases][9] section or using the following [NuGet][10] command:

```
PM> Install-Package Aspose.CAD
```

## Convert DWF to JPG Image Programmatically in C# {#section2}

You can convert a DWF file to a JPG image by following the steps:

1.  Load the input DWF with the [Image][11] class.
2.  Initialize an object of [CadRasterizationOptions][12] class.
3.  Create an instance of [JpegOptions][13] class.
4.  Set the [VectorRasterizationOptions][14] and save the output JPG image.

The following code snippet shows how to convert a DWF file to a JPG image programmatically in C#:

{{< gist aspose-com-gists 798e87ec5644ab94972f766bd61fdd79 "DWF-to-JPG.cs" >}}

## Convert DWF to PNG Image Programmatically in C# {#section3}

You can convert a DWF file to a PNG image with the steps below:

1.  Load the input DWF file using the [Image][15] class.
2.  Create an instance of [CadRasterizationOptions][16] class.
3.  Create an object of [PngOptions][17] type.
4.  Specify the [VectorRasterizationOptions][18] and write the output PNG image.

The code snippet below explains how to convert a DWF file to a PNG image programmatically in C#:

{{< gist aspose-com-gists 798e87ec5644ab94972f766bd61fdd79 "DWF-to-PNG.cs" >}}

## Get Free Temporary License

You can evaluate the API features in their full capacity by requesting a [free temporary license][19].

## Conclusion

In this article, you have explored how to convert a DWF file to image formats like PNG or JPG. It explains all the steps and code snippets to perform the conversion programmatically in C#. Moreover, please take a look at the [documentation][20] for detailed information about the features supported by the API. Please feel free to reach out to us at the [forum][21] in case of any queries.

## See Also

[Convert DWG to DXF Programmatically in C#][22]




[1]: https://docs.fileformat.com/cad/dwf/
[2]: https://docs.fileformat.com/image/jpeg/
[3]: https://docs.fileformat.com/image/png/
[4]: #section1
[5]: #section2
[6]: #section3
[7]: https://products.aspose.com/cad/net/
[8]: https://docs.aspose.com/cad/net/supported-file-formats/
[9]: https://releases.aspose.com/
[10]: https://www.nuget.org/packages/Aspose.CAD/
[11]: https://apireference.aspose.com/cad/net/aspose.cad/image
[12]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/cadrasterizationoptions
[13]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/jpegoptions
[14]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/vectorrasterizationoptions
[15]: https://apireference.aspose.com/cad/net/aspose.cad/image
[16]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/cadrasterizationoptions
[17]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/pngoptions
[18]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/vectorrasterizationoptions
[19]: https://purchase.aspose.com/temporary-license
[20]: https://docs.aspose.com/cad/net/
[21]: https://forum.aspose.com/c/cad
[22]: https://blog.aspose.com/2021/12/27/dwg-to-dxf-csharp/




