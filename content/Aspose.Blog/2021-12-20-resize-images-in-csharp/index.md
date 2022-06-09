---
title: 'Resize Images Programmatically in C# .NET'
seoTitle: "Resize Images using C# .NET | Resize PNG, JPEG, SVG, GIF in C#"
description: "Use .NET image processing API to resize images in C# or VB.NET. Resize raster or vector images such as PNG, JPEG, GIF, SVG programmatically."
date: Mon, 20 Dec 2021 17:46:58 +0000
draft: false
url: /2021/12/20/resize-images-in-csharp/
author: Usman Aziz
summary: "We often get images with the size that doesn't meet our requirements, therefore, we have to resize them accordingly. In this article, you will learn **how to resize images using C# from within your .NET applications**. Moreover, you will learn how to resize raster images and vector images explicitly."
tags: ['Resizing Vector Images in csharp', 'dotnet image resizer library', 'image resize code csharp', 'resize images using csharp', 'resize raster images in csharp']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/Resize-images.jpg" alt="resize images in c#">}}


We often get images with the size that doesn't meet our requirements, therefore, we have to resize them accordingly. In this article, you will learn **how to resize images using C# from within your .NET applications**. Moreover, you will learn how to resize raster images and vector images explicitly.

*   [.NET API to Resize Images][1]
*   [Resize Raster Images][2]
    *   [Simple Resizing of an Image][3]
    *   [Resize an Image using Resize Type][4]
*   [Resize Image Proportionally][5]
*   [Resizing Vector Images][6]

## .NET API to Resize Images {#API-to-Resize-Images}

To resize images. we will use [Aspose.Imaging for .NET][7]. It is a powerful image processing API to manipulate various types of raster and vector images. You can [download][8] the API's DLL or install it via [NuGet][9].

```
PM> Install-Package Aspose.Imaging
```

## Resize Raster Images using C# {#Reszie-Raster-Images}

There are two methods to resize raster images (PNG, GIF, JPEG, etc.): simple resizing and resizing using a resize type. In simple resizing, the images are resized by providing the height and width. Whereas, the second method uses different resizing techniques. The following sections demonstrate how to resize an image using each of the above-mentioned methods.

### Simple Resizing of an Image {#Simple-Resizing-of-an-Image}

The following are the steps to resize an image in C#.

*   First, load the image file using [Image][10] class.
*   Then, resize image by calling [Image.Resize(Int32, Int32)][11] method.
*   Finally, save resized image using [Image.Save(string)][12] method.

The following code sample shows how to resize an image in .NET applications.

{{< gist aspose-com-gists 5690a325b2be179883a03f7179c471f0 "resize-image.cs" >}}

### Resize Image using a Resize Type {#Resize-an-Image-using-ResizeType-Enum}

The [ResizeType][13] enum is used to specify resizing techniques that you can use as per your requirements. The complete list of supported resizing types is available [here][14]. The following are the steps to resize an image using a particular resize technique.

*   First, load the image using [Image][15] class.
*   Then, resize image by calling [Image.Resize(Int32, Int32, ResizeType)][16] method.
*   Finally, save resized image using [Image.Save(string)][17] method.

The following code sample resizes the image using a particular resize technique.

{{< gist aspose-com-gists 5690a325b2be179883a03f7179c471f0 "resize-image-type.cs" >}}

## Resize Image Proportionally {#Resize-Image-Proportionally}

Resizing images by specifying height and width may result in a shrunk or scaled image. Therefore, you have to calculate the aspect ratio manually. However, any miscalculation in aspect ratio may lead to a stretched image. To avoid such issues, you can use proportional resizing. The following are the steps to achieve this.

*   First, load the image file using [Image][18] class.
*   Then, cache image data using [Image.CacheData()][19] method.
*   Specify new height and width of the image.
*   Calculate the proportion values using [Image.ResizeWidthProportionally(Int32)][20] and [Image.ResizeHeightProportionally(Int32)][21] method.
*   Finally, save resized image using [Image.Save(string)][22] method.

In case you want to use any particular resize type while resizing images proportionally, use the overload methods [Image.ResizeWidthProportionally(Int32, ResizeType)][23] and [Image.ResizeHeightProportionally(Int32, ResizeType)][24].

The following code sample shows how to resize an image proportionally using C#.

{{< gist aspose-com-gists 5690a325b2be179883a03f7179c471f0 "resize-image-proportionally.cs" >}}

## Resize Vector Images in C# {#Resize-Vector-Images}

Aspose.Imaging for .NET also allows you to resize the vector images and save them in a raster image format. The following code sample shows how to resize an SVG image and save the output in PNG format.

{{< gist aspose-com-gists 5690a325b2be179883a03f7179c471f0 "resize-vector-image.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [get a free temporary license][25] to use Aspose.Imaging for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to resize images programmatically using C#. Furthermore, the code samples have demonstrated how to perform simple resizing of images or resizing using a particular type. We have also covered how to avoid manual calculation of aspect ratio while resizing images. In addition, resizing of vector images is also discussed at the end. Besides, you can explore more about the .NET image processing API using [documentation][26]. Also, you can download the complete package of source code samples from [GitHub][27]. In case of any queries, you can contact us on our [forum][28].

## See Also

*   [Convert Images to Grayscale in C#][29]
*   [Add Watermark to Images using C#][30]
*   [Compress PNG, JPEG, and TIFF Images using C#][31]




[1]: #API-to-Resize-Images
[2]: #Reszie-Raster-Images
[3]: #Simple-Resizing-of-an-Image
[4]: #Resize-an-Image-using-ResizeType-Enum
[5]: #Resize-Image-Proportionally
[6]: #Resize-Vector-Images
[7]: https://products.aspose.com/imaging/net/
[8]: https://downloads.aspose.com/imaging/net/
[9]: https://nuget.org/packages/Aspose.Imaging
[10]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[11]: https://apireference.aspose.com/imaging/net/aspose.imaging/image/methods/resize
[12]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[13]: https://apireference.aspose.com/imaging/net/aspose.imaging/resizetype
[14]: https://apireference.aspose.com/imaging/net/aspose.imaging/resizetype
[15]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[16]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/resize/methods/2
[17]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[18]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[19]: https://apireference.aspose.com/imaging/net/aspose.imaging/datastreamsupporter/methods/cachedata
[20]: https://apireference.aspose.com/imaging/net/aspose.imaging/image/methods/resizewidthproportionally
[21]: https://apireference.aspose.com/imaging/net/aspose.imaging/image/methods/resizeheightproportionally
[22]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[23]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/resizewidthproportionally/methods/2
[24]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/resizeheightproportionally/methods/2
[25]: https://purchase.aspose.com/temporary-license
[26]: https://docs.aspose.com/imaging/net/
[27]: https://github.com/aspose-imaging/Aspose.Imaging-for-.NET
[28]: https://forum.aspose.com/
[29]: https://blog.aspose.com/2021/05/03/convert-images-to-grayscale-in-csharp/
[30]: https://blog.aspose.com/2021/03/08/add-watermark-to-images-in-csharp/
[31]: https://blog.aspose.com/2020/11/27/compress-png-jpeg-and-tiff-images-using-csharp/




