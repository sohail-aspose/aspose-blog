---
title: 'Adjust Image Contrast, Brightness, and Gamma in C#'
seoTitle: "C#: Adjust Image Contrast, Brightness and Gamma | C# .NET Image Editor"
description: "Use .NET image processing API to adjust contrast, brightness, and gamma of images in C#. Implement image editing features in your .NET applications."
date: Fri, 24 Dec 2021 13:31:03 +0000
draft: false
url: /2021/12/24/adjust-image-contrast-brightness-gamma-csharp/
author: Usman Aziz
summary: '[Contrast][1], [brightness][2], and [gamma][3] are popular attributes that are used to tune images. Different values of these attributes are set to control and enhance appearance of the images. In this article, we will show you **how to adjust the contrast, brightness, and gamma of an image programmatically in C#**. You can utilize this to implement image editing capabilities from within your .NET applications.'
tags: ['Adjust Brightness of an Image in Csharp', 'Adjust Contrast of an Image in Csharp', 'Csharp Image Editing API', 'Modify Gamma of an Image in Csharp']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/Adjust-Image-Contrast-Brightness-Gamma-2.png" alt="Adjust Image Contrast, Brightness, and Gamma in C#">}}


[Contrast][4], [brightness][5], and [gamma][6] are popular attributes that are used to tune images. Different values of these attributes are set to control and enhance appearance of the images. In this article, we will show you **how to adjust the contrast, brightness, and gamma of an image programmatically in C#**. You can utilize this to implement image editing capabilities from within your .NET applications.

*   [C# Image Editing API][7]
*   [Adjust Contrast of an Image in C#][8]
*   [Adjust Brightness of an Image in C#][9]
*   [Modify Gamma of an Image in C#][10]

## C# API to Adjust Image Contrast, Brightness, and Gamma {#Image-Editing-API}

[Aspose.Imaging for .NET][11] is a powerful and feature-rich image processing API for .NET/.NET Standard platforms. It supports the manipulation of a wide range of image formats without writing complex code. We will use this API to adjust the contrast, brightness, and gamma of images in C#. You can [download][12] the API or install it into your .NET applications using [NuGet][13].

```
PM> Install-Package Aspose.Imaging
```

## Adjust Contrast of an Image in C# {#Adjust-Contrast-of-an-Image}

The contrast is defined as the difference in pixel intensity. Its value is adjusted to make the objects in an image more visible and distinguishable. With high contrast, every object in the image looks very clear just like the photographs taken in the sunlight. Whereas, with low contrast, you hardly distinguish the objects just like in the foggy weather.

Let's check out how to adjust the contrast of an image in C# using Aspose.Imaging for .NET.

*   First, load the image using [Image][14] class.
*   Then, cast object to [RasterImage][15] type.
*   Cache image if it isn't using [RasterImage.CacheData()][16] method.
*   Adjust contrast in range \[-100, 100\] using [RasterImage.AdjustContrast(float)][17] method.
*   Finally, save the resultant image using [RasterImage.Save(string)][18] method.

The following code sample shows how to adjust the contrast of an image in C#.

{{< gist aspose-com-gists 3a5e8e91b8f8a8f90f46a3557c434317 "adjust-image-contrast.cs" >}}

The following is the comparison of input and output images after increasing contrast value.



{{< figure align=center src="images/Adjust-Image-Contrast.png" alt="Adjust Contrast of Images in C#" caption="Adjust Image Contrast">}}


## Adjust Brightness of an Image in C# {#Adjust-Brightness-of-an-Image}

The brightness attribute usually controls the visibility of the objects in an image. Its value is adjusted to increase or decrease the darkness. The following are the steps to modify the brightness of an image in C#.

*   First, load the image using [Image][19] class.
*   Cast object to [RasterImage][20] type.
*   Cache image if it isn't using [RasterImage.CacheData()][21] method.
*   Adjust brightness of the image using [RasterImage.AdjustBrightness(float)][22] method.
*   Finally, save the resultant image using [RasterImage.Save(string)][23] method.

The following code sample shows how to adjust the brightness of an image in C#.

{{< gist aspose-com-gists 3a5e8e91b8f8a8f90f46a3557c434317 "adjust-image-brightness.cs" >}}

The following is the comparison of input and output images after adjusting brightness.



{{< figure align=center src="images/Adjust-Image-Brightness.png" alt="Adjust Brightness of Images in C#" caption="Adjust Image Brightness">}}


## Modify Gamma of an Image in C# {#Modify-Gamma-of-an-Image}

The gamma attribute is used to modify the ratio of red, green, and blue colors in an image. Moreover, it also modifies the brightness of the image. The following are the steps to change the gamma value of an image in C#.

*   First, load the image using [Image][24] class.
*   Cast object to [RasterImage][25] type.
*   Cache image if it isn't using [RasterImage.CacheData()][26] method.
*   Change gamma of the image using [RasterImage.AdjustGamma(float, float, float)][27] method.
*   Finally, save the resultant image using [RasterImage.Save(string)][28] method.

The following code sample shows how to adjust the gamma of an image in C#.

{{< gist aspose-com-gists 3a5e8e91b8f8a8f90f46a3557c434317 "adjust-image-gamma.cs" >}}

The following is the comparison of input and output images after adjusting gamma value.



{{< figure align=center src="images/Adjust-Image-Gamma.png" alt="Adjust Gamma of Images in C#" caption="Adjust Image Gamma">}}


## Get a Free API License {#Get-a-Free-API-License}

You can [get a free temporary license][29] to use Aspose.Imaging for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to adjust the contrast, brightness, and gamma of images in C#. Furthermore, the code samples have demonstrated how an image looks after modifying the contrast, brightness, and gamma. In case you want to explore more about .NET image processing API, visit [documentation][30]. Also, download the complete source code samples of the API from [GitHub][31]. If you would have any questions or queries, reach us at our [forum][32].

## See Also

*   [Resize Images using C#][33]
*   [Convert Images to Grayscale in C#][34]
*   [Add Watermark to Images using C#][35]
*   [Compress PNG, JPEG, and TIFF Images using C#][36]




[1]: https://en.wikipedia.org/wiki/Contrast_(vision)
[2]: https://en.wikipedia.org/wiki/Brightness
[3]: https://en.wikipedia.org/wiki/Gamma_correction
[4]: https://en.wikipedia.org/wiki/Contrast_(vision)
[5]: https://en.wikipedia.org/wiki/Brightness
[6]: https://en.wikipedia.org/wiki/Gamma_correction
[7]: #Image-Editing-API
[8]: #Adjust-Contrast-of-an-Image
[9]: #Adjust-Brightness-of-an-Image
[10]: #Modify-Gamma-of-an-Image
[11]: https://products.aspose.com/imaging/net/
[12]: https://downloads.aspose.com/imaging/net/
[13]: https://nuget.org/packages/Aspose.Imaging
[14]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[15]: https://apireference.aspose.com/imaging/net/aspose.imaging/rasterimage
[16]: https://apireference.aspose.com/imaging/net/aspose.imaging/datastreamsupporter/methods/cachedata
[17]: https://apireference.aspose.com/imaging/net/aspose.imaging/rasterimage/methods/adjustcontrast
[18]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[19]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[20]: https://apireference.aspose.com/imaging/net/aspose.imaging/rasterimage
[21]: https://apireference.aspose.com/imaging/net/aspose.imaging/datastreamsupporter/methods/cachedata
[22]: https://apireference.aspose.com/imaging/net/aspose.imaging/rasterimage/methods/adjustbrightness
[23]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[24]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[25]: https://apireference.aspose.com/imaging/net/aspose.imaging/rasterimage
[26]: https://apireference.aspose.com/imaging/net/aspose.imaging/datastreamsupporter/methods/cachedata
[27]: https://apireference.aspose.com/imaging/net/aspose.imaging.rasterimage/adjustgamma/methods/1
[28]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[29]: https://purchase.aspose.com/temporary-license
[30]: https://docs.aspose.com/imaging/net/
[31]: https://github.com/aspose-imaging/Aspose.Imaging-for-.NET
[32]: https://forum.aspose.com/
[33]: https://blog.aspose.com/2021/12/20/resize-images-in-csharp/
[34]: https://blog.aspose.com/2021/05/03/convert-images-to-grayscale-in-csharp/
[35]: https://blog.aspose.com/2021/03/08/add-watermark-to-images-in-csharp/
[36]: https://blog.aspose.com/2020/11/27/compress-png-jpeg-and-tiff-images-using-csharp/




