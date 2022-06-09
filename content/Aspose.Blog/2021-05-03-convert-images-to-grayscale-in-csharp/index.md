---
title: 'Convert Images to Grayscale in C#'
seoTitle: "Convert Images to Grayscale in C# | C# Binarization and Grayscaling"
description: "Use .NET image processing API to convert images to grayscale using C#. Use binarization methods to convert colored images to black and white."
date: Mon, 03 May 2021 23:40:06 +0000
draft: false
url: /2021/05/03/convert-images-to-grayscale-in-csharp/
author: Usman Aziz
summary: 'In various cases, you may need to convert the color images to grayscale or black and white, such as, in image processing, etc. In this article, you will learn **how to convert color images to grayscale using C#**. Furthermore, the article will cover grayscaling and binarization of the images explicitly.'
tags: ['Binarization with Fixed Threshold Csharp', 'Binarization with Otsu Threshold Csharp', 'Convert Images to Black and White with Binarization', 'Convert Images to Grayscale in Csharp']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/Convert-Image-to-Grayscale.jpg" alt="convert image to grayscale C#">}}


In various cases, you may need to convert the color images to grayscale or black and white, such as, in image processing, etc. Therefore, in this article, you will learn **how to convert an image to grayscale using C#**. Furthermore, the article will cover grayscaling and binarization of the [images][1] explicitly.

*   [C# API for Converting Images to Grayscale][2]
*   [Convert Images to Grayscale in C#][3]
*   [Convert Images to Black and White with Binarization][4]
    *   [Binarization with Fixed Threshold][5]
    *   [Binarization with Otsu Threshold][6]
*   [Get a Free API License][7]

## C# API to Convert Image to Grayscale {#C-API-for-Converting-Image-to-Grayscale}

In order to convert RGB color images to grayscale, we'll use [Aspose.Imaging for .NET][8]. It is a powerful image processing API that lets you manipulate popular image formats seamlessly. You can either [download][9] the API or install it using [NuGet][10].

```
PM> Install-Package Aspose.Imaging
```

## Convert an Image to Grayscale in C# {#Convert-Image-to-Grayscale-in-C}

The following are the steps to convert a color image to grayscale in C#.

*   First, load the image using the [Image][11] class.
*   Cast the image into a [RasterCachedImage][12] object.
*   Cache the image using [RasterCachedImage.CacheData()][13] method.
*   Convert image to grayscale using [RasterCachedImage.Grayscale()][14] method.
*   Finally, save the image using [RasterCachedImage.Save(String)][15] method.

The following code sample shows how to convert an image to grayscale using C#.

{{< gist aspose-com-gists 99b57925041963022726fdc48b5e2170 "convert-image-to-grayscale.cs" >}}

### Input Image

The following is a sample image used in this article.



{{< figure align=center src="images/aspose.jpg" alt="image to grayscale C#">}}


### Converted to Grayscale

The following is the image after conversion to grayscale.



{{< figure align=center src="images/Grayscaling_out.png" alt="grayscale image">}}


## Convert Image to Black and White with Binarization {#Convert-Image-to-Grayscale-with-Binarization}

In binarization, each pixel in an image can have only two possible values; 0 or 1. Here, 0 denotes the absence and 1 denotes the presence of the color. Aspose.Imaging supports two binarization methods i.e. binarization with fixed and binarization with Otsu threshold.

### Binarization with Fixed Threshold in C# {#Binarization-with-Fixed-Threshold}

The following are the steps to perform binarization on an image using fixed threshold.

*   First, load the image using the [Image][16] class.
*   Cast the image into a [RasterCachedImage][17] object.
*   Cache the image using [RasterCachedImage.CacheData()][18] method.
*   Convert image to black and white using [RasterCachedImage.BinarizeFixed()][19] method.
*   Finally, save the image using [RasterCachedImage.Save(String)][20] method.

The following C# code applies binarization to an image and converts it to black and white.

{{< gist aspose-com-gists 99b57925041963022726fdc48b5e2170 "convert-image-to-binary-fixed.cs" >}}

### Binarization with Otsu Threshold in C# {#Binarization-with-Otsu-Threshold}

The following are the step to convert an image to black and white with Otsu threshold.

*   First, load the image using the [Image][21] class.
*   Cast the image into a [RasterCachedImage][22] object.
*   Cache the image using [RasterCachedImage.CacheData()][23] method.
*   Convert image to black and white using [RasterCachedImage.BinarizeOtsu()][24] method.
*   Finally, save the image using [RasterCachedImage.Save(String)][25] method.

The following code sample shows how to convert an image to black and white with Otsu threshold using C#.

{{< gist aspose-com-gists 99b57925041963022726fdc48b5e2170 "convert-image-to-binary-otsu.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [get a free temporary license][26] in order to use the API without evaluation limitations.

## Conclusion

In this article, you have learned how to convert an image to grayscale and black and white using C#. Moreover, you have seen how to apply binarization to the images with fixed or Otsu threshold. Furthermore, you can explore more about the C# image processing API using [documentation][27]. Also, you can share your queries with us via our [forum][28].

## See Also

*   [Add Watermark to Images using C#][29]
*   [Compress PNG, JPEG, and TIFF Images using C#][30]




[1]: https://docs.fileformat.com/image/
[2]: #C-API-for-Converting-Image-to-Grayscale
[3]: #Convert-Image-to-Grayscale-in-C
[4]: #Convert-Image-to-Grayscale-with-Binarization
[5]: #Binarization-with-Fixed-Threshold
[6]: #Binarization-with-Otsu-Threshold
[7]: #Get-a-Free-API-License
[8]: https://products.aspose.com/imaging/net
[9]: https://downloads.aspose.com/imaging/net
[10]: https://nuget.org/packages/Aspose.Imaging
[11]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[12]: https://apireference.aspose.com/imaging/net/aspose.imaging/rastercachedimage
[13]: https://apireference.aspose.com/imaging/net/aspose.imaging/rastercachedimage/methods/cachedata
[14]: https://apireference.aspose.com/imaging/net/aspose.imaging/rastercachedimage/methods/grayscale
[15]: https://apireference.aspose.com/imaging/net/aspose.imaging.datastreamsupporter/save/methods/2
[16]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[17]: https://apireference.aspose.com/imaging/net/aspose.imaging/rastercachedimage
[18]: https://apireference.aspose.com/imaging/net/aspose.imaging/rastercachedimage/methods/cachedata
[19]: https://apireference.aspose.com/imaging/net/aspose.imaging/rastercachedimage/methods/binarizefixed
[20]: https://apireference.aspose.com/imaging/net/aspose.imaging.datastreamsupporter/save/methods/2
[21]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[22]: https://apireference.aspose.com/imaging/net/aspose.imaging/rastercachedimage
[23]: https://apireference.aspose.com/imaging/net/aspose.imaging/rastercachedimage/methods/cachedata
[24]: https://apireference.aspose.com/imaging/net/aspose.imaging/rastercachedimage/methods/binarizeotsu
[25]: https://apireference.aspose.com/imaging/net/aspose.imaging.datastreamsupporter/save/methods/2
[26]: https://purchase.aspose.com/temporary-license
[27]: https://docs.aspose.com/imaging/net/getting-started/
[28]: https://forum.aspose.com/
[29]: https://blog.aspose.com/2021/03/08/add-watermark-to-images-in-csharp/
[30]: https://blog.aspose.com/2020/11/27/compress-png-jpeg-and-tiff-images-using-csharp/





