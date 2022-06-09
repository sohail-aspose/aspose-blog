---
title: 'Convert JPG Images to PNG in C#'
seoTitle: "Convert JPG Images to PNG in C# .NET | JPG to PNG Converter Library"
description: "Use .NET image processing API to convert JPG images to PNG format in C#. Perform high quality conversion of JPG images to PNG programmatically in .NET apps."
date: Mon, 15 Nov 2021 03:09:00 +0000
draft: false
url: /2021/11/15/convert-jpg-to-png-in-csharp/
author: Usman Aziz
summary: '[JPG][1] is one of the most popular and widely used image formats. However, JPG images lose quality each time they are saved. Therefore, you may need to convert them into a lossless format such as [PNG][2]. To perform this conversion programmatically from within the .NET applications, this article shows **how to convert a JPG image to PNG in C#**.'
tags: ['convert jpg to png in csharp', 'dotnet image converter library', 'dotnet jpg to png converter', 'jpg to png converter in csharp']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/convert-jpg-to-png.jpg" alt="convert jpg images to png format in c#">}}


[JPG][3] is one of the most popular and widely used image formats. However, JPG images lose quality each time they are saved. Therefore, you may need to convert them into a lossless format such as [PNG][4]. To perform this conversion programmatically from within the .NET applications, this article shows **how to convert a JPG image to PNG in C#**.

*   [.NET API for JPG to PNG Conversion][5]
*   [Converting a JPG Image to PNG][6]

## C# .NET API for JPG to PNG Conversion {#API-for-JPG-to-PNG-Conversion}

[Aspose.Imaging for .NET][7] is a feature-rich image processing API to manipulate a multitude of image formats. Moreover, it provides a powerful converter that lets you convert images from one format to another with high fidelity. In this article, we will use this API to convert our JPG images to PNG format. You can either [download][8] the API's DLL or install it directly from [NuGet][9].

```
PM> Install-Package Aspose.Imaging
```

## Convert a JPG Image to PNG in C# {#Converting-a-PNG-Image-to-JPG}

It is quite straightforward to convert a JPG image to PNG format using Aspose.Imaging for .NET. You only need to load the JPG file and save it as a PNG image. The following are the steps to convert a JPG image to PNG in C#.

*   Load the JPG file using [Image][10] class.
*   Create an instance of [PngOptions][11] class.
*   Set [PngOptions.ColorType][12] property to [FileFormats.Png.PngColorType.TruecolorWithAlpha][13].
*   Convert JPG image to PNG using [Image.Save(string, PngOptions)][14] method.

The following code sample shows how to convert a JPG image to PNG format in .NET applications.

{{< gist aspose-com-gists 043a4cdac69552bf48360e07520ee206 "jpg-to-png.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [get a free temporary license][15] to use Aspose.Imaging for .NET without evaluation limitations.

## Conclusion

JPG to PNG conversion is often performed to convert images to a lossless format. In this article, you have learned how to convert JPG images to PNG format programmatically in C#. Thus, you can easily embed JPG to PNG conversion into your .NET applications. In addition, you can explore more about the .NET image processing API using [documentation][16]. Also, you can post your queries on our [forum][17].

## See Also

*   [Convert Images to Grayscale in C#][18]
*   [Add Watermark to Images using C#][19]
*   [Compress PNG, JPEG, and TIFF Images using C#][20]




[1]: https://docs.fileformat.com/image/jpeg/
[2]: https://docs.fileformat.com/image/png/
[3]: https://docs.fileformat.com/image/jpeg/
[4]: https://docs.fileformat.com/image/png/
[5]: #API-for-JPG-to-PNG-Conversion
[6]: #Converting-a-PNG-Image-to-JPG
[7]: https://products.aspose.com/imaging/net/
[8]: https://downloads.aspose.com/imaging/net/
[9]: https://nuget.org/packages/Aspose.Imaging
[10]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[11]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/pngoptions
[12]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/pngoptions/properties/colortype
[13]: https://apireference.aspose.com/imaging/net/aspose.imaging.fileformats.png/pngcolortype
[14]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/4
[15]: https://purchase.aspose.com/temporary-license
[16]: https://docs.aspose.com/imaging/net/
[17]: https://forum.aspose.com/
[18]: https://blog.aspose.com/2021/05/03/convert-images-to-grayscale-in-csharp/
[19]: https://blog.aspose.com/2021/03/08/add-watermark-to-images-in-csharp/
[20]: https://blog.aspose.com/2020/11/27/compress-png-jpeg-and-tiff-images-using-csharp/




