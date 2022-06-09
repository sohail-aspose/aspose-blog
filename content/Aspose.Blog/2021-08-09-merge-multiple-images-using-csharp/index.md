---
title: 'Merge or Combine Images Programmatically using C#'
seoTitle: "Merge Multiple Images in C# .NET | Combine Images into Single Image"
description: "Use .NET image processing API to merge multiple images into a single image using C# .NET. Merge images vertically or horizontally in .NET applications."
date: Mon, 09 Aug 2021 17:26:00 +0000
draft: false
url: /2021/08/09/merge-multiple-images-using-csharp/
author: Usman Aziz
summary: 'In this article, you will learn **how to merge or combine multiple images into a single image programmatically using C#**. The step-by-step guide and the code samples will demonstrate how to merge images horizontally or vertically.'
tags: ['combine images using csharp', 'merge images horizontally in csharp', 'merge images using csharp', 'merge images vertically in csharp', 'merge multiple images in csharp']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/Merge-Image.jpg" alt="Merge Images in C#">}}


In this article, you will learn **how to merge or combine multiple images into a single image programmatically using C#**. The step-by-step guide and the code samples will demonstrate how to merge images horizontally or vertically.

*   [C# API to Merge Images][1]
*   [Merge Multiple Images using C#][2]
    *   [Merge Images Vertically][3]
    *   [Combine Images Horizontally][4]

**INFO:** Aspose provides a [FREE Collage web app][5]. Using this online service, you can merge [JPG to JPG][6] or PNG to PNG images, create [photo grids][7], and so on.

## C# API to Merge Images {#API-to-Merge-Images}

In order to merge multiple images into a single image, we will use [Aspose.Imaging for .NET][8]. It is a powerful and feature-rich image processing API that lets you manipulate a wide range of image formats. You can either [download][9] the API or install it using [NuGet][10].

```
PM> Install-Package Aspose.Imaging
```

## Merge Multiple Images using C# {#Merge-Multiple-Images}

There are two ways to merge images into a single one: vertically and horizontally. In the former method, the images are appended to each other vertically, whereas, in the latter, images are combined one after another horizontally. In the following sections, you will learn both of the methods with code samples.

### Merge Images Vertically {#Merge-Images-Vertically}

The following are the steps to merge images vertically using C#.

*   First, specify the paths of the images in a string array.
*   Then, create a List of [Size][11] and store size of each image into it.
*   Calculate the height and width of the resultant image.
*   Create an object of [StreamSource][12] class and initialize it with a new [MemoryStream][13].
*   Create an object of [JpegOptions][14] class and set its options.
*   Instantiate [JpegImage][15] class for the new image and initialize it with _JpegOptions_ and calculated height and width.
*   Iterate through the list of images and in each iteration, load the image in a [RasterImage][16] object.
*   Create a [Rectangle][17] for each image and add it to the new image using [JpegImage.SaveArgb32Pixels()][18] method.
*   Increase the stitched height in each iteration.
*   Finally, save the new image using [JpegImage.Save(string)][19] method.

The following code sample shows how to merge images vertically.

{{< gist aspose-com-gists 9e4c397cef74dcfed71b8338f76b6aa1 "merge-images-vertically.cs" >}}

## Merge Images Horizontally {#Combine-Images-Horizontally}

The following are the steps to combine images horizontally using C#.

*   First, specify the paths of the images in a string array.
*   Then, create a List of [Size][20] and store size of each image into it.
*   Calculate the height and width of the resultant image.
*   Create a new source using [FileCreateSource(String, Boolean)][21] and initialize it with file's path.
*   Create an object of [JpegOptions][22] class and set its options.
*   Instantiate [JpegImage][23] class for the new image and initialize it with _JpegOptions_ and calculated height and width.
*   Iterate through the list of images and in each iteration, load the image in a [RasterImage][24] object.
*   Create a [Rectangle][25] for each image and add it to new image using [JpegImage.SaveArgb32Pixels()][26] method.
*   Increase the stitched width in each iteration.
*   Once done, save the new image using [JpegImage.Save(string)][27] method.

The following code sample shows how to merge multiple images horizontally.

{{< gist aspose-com-gists 9e4c397cef74dcfed71b8338f76b6aa1 "merge-images-horizontally.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [get a free temporary license][28] in order to use the API without evaluation limitations.

## Conclusion

In this article, you have learned how to merge multiple images into a single image using C#. The code samples have demonstrated how to combine the images vertically and horizontally. You can explore more about the .NET image processing API using [documentation][29]. Also, you can share your queries with us via our [forum][30].

## See Also

*   [Convert Images to Grayscale in C#][31]
*   [Add Watermark to Images using C#][32]
*   [Compress PNG, JPEG, and TIFF Images using C#][33]




[1]: #API-to-Merge-Images
[2]: #Merge-Multiple-Images
[3]: #Merge-Images-Vertically
[4]: #Combine-Images-Horizontally
[5]: https://products.aspose.app/slides/collage
[6]: https://products.aspose.app/slides/collage/jpg
[7]: https://products.aspose.app/slides/collage/photo-grid
[8]: https://products.aspose.com/imaging/net
[9]: https://downloads.aspose.com/imaging/net
[10]: http://nuget.org/packages/Aspose.Imaging
[11]: https://apireference.aspose.com/imaging/net/aspose.imaging/size
[12]: https://apireference.aspose.com/imaging/net/aspose.imaging.sources/streamsource
[13]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream
[14]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/jpegoptions
[15]: https://apireference.aspose.com/imaging/net/aspose.imaging.fileformats.jpeg/jpegimage
[16]: https://apireference.aspose.com/imaging/net/aspose.imaging/rasterimage
[17]: https://apireference.aspose.com/imaging/net/aspose.imaging/rectangle
[18]: https://apireference.aspose.com/imaging/net/aspose.imaging/rasterimage/methods/saveargb32pixels
[19]: https://apireference.aspose.com/imaging/net/aspose.imaging.datastreamsupporter/save/methods/2
[20]: https://apireference.aspose.com/imaging/net/aspose.imaging/size
[21]: https://apireference.aspose.com/imaging/net/aspose.imaging.sources/filecreatesource/constructors/1
[22]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/jpegoptions
[23]: https://apireference.aspose.com/imaging/net/aspose.imaging.fileformats.jpeg/jpegimage
[24]: https://apireference.aspose.com/imaging/net/aspose.imaging/rasterimage
[25]: https://apireference.aspose.com/imaging/net/aspose.imaging/rectangle
[26]: https://apireference.aspose.com/imaging/net/aspose.imaging/rasterimage/methods/saveargb32pixels
[27]: https://apireference.aspose.com/imaging/net/aspose.imaging.datastreamsupporter/save/methods/2
[28]: https://purchase.aspose.com/temporary-license
[29]: https://docs.aspose.com/imaging/net
[30]: https://forum.aspose.com/
[31]: https://blog.aspose.com/2021/05/03/convert-images-to-grayscale-in-csharp/
[32]: https://blog.aspose.com/2021/03/08/add-watermark-to-images-in-csharp/
[33]: https://blog.aspose.com/2020/11/27/compress-png-jpeg-and-tiff-images-using-csharp/





