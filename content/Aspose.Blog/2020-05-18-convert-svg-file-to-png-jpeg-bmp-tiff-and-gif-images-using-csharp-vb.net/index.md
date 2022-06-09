---
title: 'Convert SVG Files to PNG, JPEG, BMP, TIFF, and GIF Images using C#'
seoTitle: ""
description: ""
date: Mon, 18 May 2020 18:25:55 +0000
draft: false
url: /2020/05/18/convert-svg-file-to-png-jpeg-bmp-tiff-and-gif-images-using-csharp-vb.net/
author: Usman Aziz
summary: ''
tags: ['Convert SVG to BMP', 'Convert SVG to GIF', 'Convert SVG to JPEG', 'Convert SVG to PNG', 'Convert SVG to TIFF']
categories: ['Aspose.SVG Product Family']
---



{{< figure align=center src="images/Convert-SVG-to-Image.jpg" alt="Convert SVG to Image">}}


In this article, I am going to show you how to convert SVG files to PNG, JPEG, TIFF, and other popular raster image formats using C# with Aspose's [.NET SVG API][1].

[Aspose.SVG for .NET][2] is a powerful API for processing SVG files using C# or VB.NET. It allows you to load, parse, and convert the SVG files to various other file formats. In this article, we'll leverage the capabilities of the converter API of Aspose.SVG for .NET and learn how to perform the following SVG conversions:

*   [Convert SVG to PNG using C#][3]
*   [SVG to JPEG conversion using C#][4]
*   [Convert SVG to BMP using C#][5]
*   [Save SVG as TIFF Image using C#][6]
*   [Convert SVG to GIF using C#][7]

## C# SVG to Image Converter - Installation

Aspose.SVG for .NET is hosted on [NuGet][8] and can easily be installed using the NuGet Package Manager. Alternatively, you can download the API's DLL from the [Downloads][9] section.

## Convert SVG to PNG using C# {#Convert-SVG-to-PNG-using-CSharp}

PNG is a popular image format because of its lossless compression. You can opt to convert SVG to PNG in case you want high-resolution images without losing the quality. The following are the steps to perform SVG to PNG conversion using Aspose.SVG for .NET.

*   Load the SVG image using the [SVGDocument][10] class.
*   Create an instance of [ImageDevice][11] class for specifying output image format and file's path.
*   Render SVG to PNG using [SVGDocument.RenderTo(ImageDevice)][12] method.

The following code sample shows how to convert SVG to PNG using C#.

{{< gist aspose-com-gists 0420a5530f73658aebea7f98ea4d705f "Examples-CSharp-LoadSaveConvert-ConvertSVGToImage-ConvertSVGToPNG.cs" >}}

## Convert SVG to JPEG Image using C# {#SVG-to-JPEG-conversion-using-CSharp}

Conversion of SVG to JPEG format is useful when you need to compress the image to reduce the file's size. JPEG supports lossy compression which leads you to compromise the quality of the image. Here, the higher compression means a lower image quality. The following are the steps to export the SVG file to a JPEG image.

*   Create an instance of [SVGDocument][13] and load the SVG file.
*   Create and initialize the [ImageDevice][14] object for the output JPEG image.
*   Save SVG as JPEG using [SVGDocument.RenderTo(ImageDevice)][15] method.

The following code sample converts an SVG file to the JPEG image in C#.

{{< gist aspose-com-gists 0420a5530f73658aebea7f98ea4d705f "Examples-CSharp-LoadSaveConvert-ConvertSVGToImage-ConvertSVGToJPEG.cs" >}}

## Convert SVG to BMP using C# {#Convert-SVG-to-BMP-using-CSharp}

BMP format is in the business since long for digital representation of the images. BMP is known as a device-independent format which can be opened on multiple platforms such as Windows, Mac, etc. The following are the steps to perform SVG to BMP conversion using Aspose.SVG for .NET.

*   Use [SVGDocument][16] to load the SVG file you want to convert.
*   Use the [ImageDevice][17] class to specify the output format and file's path.
*   Render SVG as BMP using [SVGDocument.RenderTo(ImageDevice)][18] method.

The following code sample shows how to save an SVG as BMP using C#.

{{< gist aspose-com-gists 0420a5530f73658aebea7f98ea4d705f "Examples-CSharp-LoadSaveConvert-ConvertSVGToImage-ConvertSVGToBMP.cs" >}}

## Convert SVG to TIFF using C# {#Save-SVG-as-TIFF-Image-using-CSharp}

TIFF is another popular format for digital images that supports both lossy and lossless compression. It is more popular among graphic artists, industries as well as the photographer for producing the high resolution/quality images. The following are the steps for SVG to TIFF conversion.

*   Load SVG file using the [SVGDocument][19] class.
*   Create and initialize the [ImageDevice][20] object for the output TIFF image.
*   Save SVG as TIFF using [SVGDocument.RenderTo(ImageDevice)][21] method.

The following code sample shows how to render an SVG file as a TIFF image using C#.

{{< gist aspose-com-gists 0420a5530f73658aebea7f98ea4d705f "Examples-CSharp-LoadSaveConvert-ConvertSVGToImage-ConvertSVGToTIFF.cs" >}}

**Tip**: You may want to check out Aspose [Text to GIF][22] service that allows you to create beautiful animations just by typing.

## Convert SVG to GIF using C# {#Convert-SVG-to-GIF-using-CSharp}

GIF is another raster image format that also supports high compression features. One of the popular use cases of GIF images is displaying the animations that are produced by combining multiple images into a single GIF file. The following are the steps to convert an SVG file to a GIF image.

*   Create an instance of the [SVGDocument][23] class for loading the source SVG file.
*   Use the [ImageDevice][24] class to specify the output image's format and its path.
*   Save SVG as GIF using [SVGDocument.RenderTo(ImageDevice)][25] method.

The following code sample demonstrates SVG to GIF conversion using C#.

{{< gist aspose-com-gists 0420a5530f73658aebea7f98ea4d705f "Examples-CSharp-LoadSaveConvert-ConvertSVGToImage-ConvertSVGToGIF.cs" >}}

## Conclusion

In this article, you have learned how to export SVG files to popular image formats using C#. The step by step guide and code samples demonstrate how to convert SVG to PNG, JPEG, BMP, TIFF, and GIF images. You can learn more about the C# SVG library using the [documentation][26].

## See Also

*   [Create, Edit, and Read SVG Files using C#][27]




[1]: http://products.aspose.com/svg/net
[2]: http://products.aspose.com/svg/net
[3]: #Convert-SVG-to-PNG-using-CSharp
[4]: #SVG-to-JPEG-conversion-using-CSharp
[5]: #Convert-SVG-to-BMP-using-CSharp
[6]: #Save-SVG-as-TIFF-Image-using-CSharp
[7]: #Convert-SVG-to-GIF-using-CSharp
[8]: http://nuget.org/packages/Aspose.SVG
[9]: https://downloads.aspose.com/svg/net
[10]: https://apireference.aspose.com/svg/net/aspose.svg/svgdocument
[11]: https://apireference.aspose.com/svg/net/aspose.svg.rendering.image/imagedevice
[12]: https://apireference.aspose.com/svg/net/aspose.svg/svgdocument/methods/renderto
[13]: https://apireference.aspose.com/svg/net/aspose.svg/svgdocument
[14]: https://apireference.aspose.com/svg/net/aspose.svg.rendering.image/imagedevice
[15]: https://apireference.aspose.com/svg/net/aspose.svg/svgdocument/methods/renderto
[16]: https://apireference.aspose.com/svg/net/aspose.svg/svgdocument
[17]: https://apireference.aspose.com/svg/net/aspose.svg.rendering.image/imagedevice
[18]: https://apireference.aspose.com/svg/net/aspose.svg/svgdocument/methods/renderto
[19]: https://apireference.aspose.com/svg/net/aspose.svg/svgdocument
[20]: https://apireference.aspose.com/svg/net/aspose.svg.rendering.image/imagedevice
[21]: https://apireference.aspose.com/svg/net/aspose.svg/svgdocument/methods/renderto
[22]: https://products.aspose.app/slides/text-to-gif
[23]: https://apireference.aspose.com/svg/net/aspose.svg/svgdocument
[24]: https://apireference.aspose.com/svg/net/aspose.svg.rendering.image/imagedevice
[25]: https://apireference.aspose.com/svg/net/aspose.svg/svgdocument/methods/renderto
[26]: https://docs.aspose.com/display/svgnet/Product+Overview
[27]: https://blog.aspose.com/2020/02/13/create-edit-read-and-convert-svg-files-using-c-aspose.svg-for-.net/





