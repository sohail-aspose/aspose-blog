---
title: 'Rotate and Flip Images in C# .NET'
seoTitle: "Rotate and Flip Images in C# .NET | .NET Image Editor Library"
description: "Use .NET image processing API to rotate and flip images using C# or VB.NET. Rotate image only, flip image only, or rotate and flip image at the same time."
date: Tue, 21 Dec 2021 13:21:40 +0000
draft: false
url: /2021/12/21/rotate-and-flip-images-in-csharp/
author: Usman Aziz
summary: 'While working with images, you may often need to rotate images at different angles. Moreover, horizontal and vertical flips are also used in various cases, especially in image editors. In this article, we will cover **how to rotate and flip images programmatically using C#**.'
tags: ['Csharp dotnet image editor API', 'Flip an Image in Csharp', 'Rotate an Image in Csharp', 'Rotate and Flip an Image in Csharp', 'dotnet library to Rotate and Flip Images']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/Rotate-Flip-Images-Logo.jpg" alt="Rotate or Flip images in C# .NET">}}


While working with images, you may often need to rotate them at different angles. Moreover, horizontal and vertical flips are also used in various cases. Both are considered the key features of every image editor. In this article, you will learn **how to rotate and flip images programmatically in C#**.

*   [.NET API to Rotate and Flip Images][1]
*   [Rotate and Flip an Image][2]
    *   [Rotate an Image in C#][3]
    *   [Flip an Image in C#][4]
    *   [Rotate and Flip an Image in C#][5]

## C# .NET API to Rotate and Flip Images {#API-to-Rotate-and-Flip-Images}

To rotate and flip images from within .NET applications, we will use [Aspose.Imaging for .NET][6]. It is an image processing API that provides a wide range of features to manipulate various types of images. Furthermore, it hides the complex operations and makes it quite easier for you to perform image processing. You can [download][7] the API or install it into your .NET applications using [NuGet][8].

```
PM> Install-Package Aspose.Imaging
```

## Rotate and Flip an Image in C# {#Rotate-and-Flip-an-Image}

To rotate an image, you need to specify a rotation angle. The most commonly used angles are 90, 180, and 270 degrees. In addition to that, the images are flipped horizontally or vertically. Aspose.Imaging for .NET takes care of rotation as well as flipping at the same time. For this, the API provides [RotateFlipType][9] enum to specify the rotation angle and flip type. You can perform the following flip/rotate operations on an image:

*   Rotate only
*   Flip only
*   Both rotate and flip

Let's see how to perform each of the above-mentioned operations on the following image.



{{< figure align=center src="images/lion-image.png" alt="Image for rotation and flipping">}}


### Rotate an Image in C# {#Rotate-an-Image}

First, let's have a look at how to rotate an image. The following options are used to rotate an image without flipping.

*   **Rotate180FlipNone**: 180-degree rotation without flipping
*   **Rotate270FlipNone**: 270-degree rotation without flipping
*   **Rotate90FlipNone**: 90-degree rotation without flipping

The following are the steps to perform the rotation of an image in C#.

*   First, load the image file using [Image][10] class.
*   Then, rotate image to 270 degrees using [Image.RotateFlip(RotateFlipType.Rotate270FlipNone)][11] method.
*   Finally, save updated image using [Image.Save(string)][12] method.

The following code snippet shows how to rotate an image to a particular angle.

{{< gist aspose-com-gists 7d208081e84c309d073e79ffdbd4214d "rotate-image.cs" >}}

The following is the rotated image that we get after executing this code.



{{< figure align=center src="images/Rotate-Image.png" alt="rotate an image in C#" caption="Rotate an Image">}}


### Flip an Image in C# {#Flip-an-Image}

Now, take a look at how to flip an image without rotation. For this, the following **RotateFlipType** members are used.

*   **RotateNoneFlipX**: No rotation with horizontal flipping
*   **RotateNoneFlipY**: No rotation with vertical flipping
*   **RotateNoneFlipXY**: No rotation with horizontal and vertical flipping

The following are the steps to flip an image in C#.

*   First, load the image file using [Image][13] class.
*   Then, flip the image horizontally using [Image.RotateFlip(RotateFlipType.RotateNoneFlipX)][14] method.
*   Finally, save updated image using [Image.Save(string)][15] method.

The following code sample shows how to flip an image in .NET applications.

{{< gist aspose-com-gists 7d208081e84c309d073e79ffdbd4214d "flip-image.cs" >}}

The following screenshot shows how the image is flipped using the code snippet above.



{{< figure align=center src="images/Flip-Image.png" alt="Flip an image in C#" caption="Flip an Image">}}


### Rotate and Flip an Image in C# {#Rotate-and-Flip-an-Image-at-once}

In this section, we will see how to rotate and flip the image at the same time. To achieve this, the following members of **RotateFlipType** enum are used.

*   **Rotate180FlipX**: 180-degree rotation with horizontal flipping
*   **Rotate180FlipXY**: 180-degree rotation with horizontal and vertical flipping
*   **Rotate180FlipY**: 180-degree rotation with vertical flipping
*   **Rotate270FlipX**: 270-degree rotation with horizontal flipping
*   **Rotate270FlipXY**: 270-degree rotation with horizontal and vertical flipping
*   **Rotate270FlipY**: 270-degree rotation with vertical flipping
*   **Rotate90FlipX**: 90-degree rotation with horizontal flipping
*   **Rotate90FlipXY**: 90-degree rotation with horizontal and vertical flipping
*   **Rotate90FlipY**: 90-degree rotation with vertical flipping

The following are the steps to rotate and flip an image in C#.

*   First, load the image file using [Image][16] class.
*   Then, rotate the image on 180 degree and flip it horizontally using [Image.RotateFlip(RotateFlipType.Rotate180FlipX)][17] method.
*   Finally, save updated image using [Image.Save(string)][18] method.

The following C# code snippet shows how to perform rotation and flipping at the same time.

{{< gist aspose-com-gists 7d208081e84c309d073e79ffdbd4214d "rotate-flip-image.cs" >}}

The following screenshot shows how the image looks like after we apply rotation and flipping.



{{< figure align=center src="images/Rotate-and-Flip-Image.png" alt="Rotate and flip an image in C#" caption="Rotate and Flip an Image">}}


## Get a Free API License {#Get-a-Free-API-License}

You can [get a free temporary license][19] to use Aspose.Imaging for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to rotate and flip images programmatically in C#. Furthermore, the step by step guide and code samples have demonstrated how to rotate an image, flip an image, and rotate and flip an image at the same time. Besides, you can explore more about .NET image processing API using [documentation][20]. Also, you can download the source code samples of the API from [GitHub][21]. In case of any queries, you can reach us at our [forum][22].

## See Also

*   [Resize Images using C#][23]
*   [Convert Images to Grayscale in C#][24]
*   [Add Watermark to Images using C#][25]
*   [Compress PNG, JPEG, and TIFF Images using C#][26]




[1]: #API-to-Rotate-and-Flip-Images
[2]: #Rotate-and-Flip-an-Image
[3]: #Rotate-an-Image
[4]: #Flip-an-Image
[5]: #Rotate-and-Flip-an-Image-at-once
[6]: https://products.aspose.com/imaging/net/
[7]: https://downloads.aspose.com/imaging/net/
[8]: https://nuget.org/packages/Aspose.Imaging
[9]: https://apireference.aspose.com/imaging/net/aspose.imaging/rotatefliptype
[10]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[11]: https://apireference.aspose.com/imaging/net/aspose.imaging/image/methods/rotateflip
[12]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[13]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[14]: https://apireference.aspose.com/imaging/net/aspose.imaging/image/methods/rotateflip
[15]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[16]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[17]: https://apireference.aspose.com/imaging/net/aspose.imaging/image/methods/rotateflip
[18]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[19]: https://purchase.aspose.com/temporary-license
[20]: https://docs.aspose.com/imaging/net/
[21]: https://github.com/aspose-imaging/Aspose.Imaging-for-.NET
[22]: https://forum.aspose.com/
[23]: https://blog.aspose.com/2021/12/20/resize-images-in-csharp/
[24]: https://blog.aspose.com/2021/05/03/convert-images-to-grayscale-in-csharp/
[25]: https://blog.aspose.com/2021/03/08/add-watermark-to-images-in-csharp/
[26]: https://blog.aspose.com/2020/11/27/compress-png-jpeg-and-tiff-images-using-csharp/




