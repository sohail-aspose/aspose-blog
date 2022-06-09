---
title: 'Add Watermark to Images using C#'
seoTitle: "Add Watermark to Images using C# | PNG, JPEG, BMP, and Others"
description: "Use .NET image processing API to add watermark to images using C#. Add watermark to PNG, JPEG, BMP and other popular image formats in C#."
date: Mon, 08 Mar 2021 11:50:00 +0000
draft: false
url: /2021/03/08/add-watermark-to-images-in-csharp/
author: Usman Aziz
summary: "Watermarks in images are usually used to claim ownership of the content. On the other hand, images are watermarked to avoid unauthorized usage or counterfeiting. In various cases, you may need to automate watermarking feature within your web or desktop applications. For such scenarios, this article covers **how to add watermark to images programmatically using C#**. This could also be useful when you need to watermark a batch of images in one go. So let's begin."
tags: ['Add Diagonal Watermark to images in Csharp', 'Add Watermark to an Image in Csharp', 'Csharp API to Add Watermark to Images']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/Add-Watermark-to-Images.jpg" alt="add watermark to images C#">}}


Watermarks in images are usually used to claim ownership of the content. On the other hand, images are watermarked to avoid unauthorized usage or counterfeiting. In various cases, you may need to automate watermarking feature within your web or desktop applications. For such scenarios, this article covers **how to add watermark to images programmatically using C#**. This could also be useful when you need to watermark a batch of images in one go. So let's begin.

*   [C# API to Add Watermark to Images][1]
*   [Add Watermark to an Image in C#][2]
*   [Add Diagonal Watermark to images in C#][3]
*   [Get Free API License][4]

## C# API to Add Watermark to Images {#API-to-Add-Watermark-to-Images}

In order to add watermarks to images, we'll use [Aspose.Imaging for .NET][5]. It is a powerful image processing API that supports a wide range of image formats. Furthermore, the API makes it easier for you to manipulate the images. You can either [download][6] binaries of the API or get it installed using [NuGet][7].

```
PM> Install-Package Aspose.Imaging
```

## Add Watermark to an Image in C# {#Add-Watermark-to-an-Image-in-csharp}

The following are the steps to add a watermark to an image using C#.

*   Load the image using [Image][8] class.
*   Create an instance of [Graphics][9] class and initialize it with [Image][10] object.
*   Set font family, size, and face using [Font][11] class.
*   Create an instance of [SolidBrush][12] class and set its properties such as color etc.
*   Instantiate [StringFormat][13] class to set text alignment.
*   Add watermark to the image using [Graphics.DrawString(String, Font, SolidBrush, 0, 0, StringFormat)][14] method.
*   Save the image using [Image.Save(String)][15] method.

The following code sample shows how to add watermark to an image in C#.

{{< gist aspose-com-gists 940c35e16a1b6065fafce68838d36c63 "add-watermark-to-image.cs" >}}



{{< figure align=center src="images/watermarked.jpg" alt="Add watermark to image C#">}}


## Add Diagonal Watermark to images in C# {#Add-Diagonal-Watermark-to-images-in-csharp}

In various cases, watermarks are applied to the images diagonally. For this, Aspose.Imaging for .NET allows you to transform the watermark text on a certain angle. The following are the steps to add a diagonal watermark to an image.

*   Load the image using [Image][16] class.
*   Create an instance of [Graphics][17] class and initialize it with [Image][18] object.
*   Set font family, size, and face using [Font][19] class.
*   Create an instance of [SolidBrush][20] class and set its properties such as color etc.
*   Instantiate [StringFormat][21] class to set text alignment.
*   Create an instance of [Matrix][22] class and set transformation angle.
*   Assign Matrix object to [Graphics.Transform][23] property.
*   Add watermark using [Graphics.DrawString(String, Font, SolidBrush, 0, 0, StringFormat)][24] method.
*   Save the image using [Image.Save(String)][25] method.

The following code sample shows how to add a diagonal watermark to images using C#.

{{< gist aspose-com-gists 940c35e16a1b6065fafce68838d36c63 "add-diagonal-watermark-to-image.cs" >}}



{{< figure align=center src="images/watermark_diagonal.jpg" alt="Add diagonal watermark to image C#">}}


## Get a Free API License {#Get-a-Free-API-License}

In case you want to try the API without evaluation limitations, you can [get a free temporary license][26].

## Conclusion

In this article, you have learned how to add watermark to images using C#. Furthermore, you have seen how to transform watermark text to a particular angle. You can explore more about C# image processing API using [documentation][27]. In case you would have any questions or queries, contact us via our [forum][28].

## See Also

*   [Compress PNG, JPEG, and TIFF Images using C#][29]




[1]: #API-to-Add-Watermark-to-Images
[2]: #Add-Watermark-to-an-Image-in-csharp
[3]: #Add-Diagonal-Watermark-to-images-in-csharp
[4]: https://blog.aspose.com/2021/01/27/Add-Watermark-to-Images-using-Java/#Get-a-Free-License
[5]: https://products.aspose.com/imaging/net
[6]: https://downloads.aspose.com/imaging/net
[7]: https://www.nuget.org/packages/Aspose.Imaging
[8]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[9]: https://apireference.aspose.com/imaging/net/aspose.imaging/graphics
[10]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[11]: https://apireference.aspose.com/imaging/net/aspose.imaging/font
[12]: https://apireference.aspose.com/imaging/net/aspose.imaging.brushes/solidbrush
[13]: https://apireference.aspose.com/imaging/net/aspose.imaging/stringformat
[14]: https://apireference.aspose.com/imaging/net/aspose.imaging.graphics/drawstring/methods/5
[15]: https://apireference.aspose.com/imaging/net/aspose.imaging.datastreamsupporter/save/methods/2
[16]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[17]: https://apireference.aspose.com/imaging/net/aspose.imaging/graphics
[18]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[19]: https://apireference.aspose.com/imaging/net/aspose.imaging/font
[20]: https://apireference.aspose.com/imaging/net/aspose.imaging.brushes/solidbrush
[21]: https://apireference.aspose.com/imaging/net/aspose.imaging/stringformat
[22]: https://apireference.aspose.com/imaging/net/aspose.imaging/matrix
[23]: https://apireference.aspose.com/imaging/net/aspose.imaging/graphics/properties/transform
[24]: https://apireference.aspose.com/imaging/net/aspose.imaging.graphics/drawstring/methods/5
[25]: https://apireference.aspose.com/imaging/net/aspose.imaging.datastreamsupporter/save/methods/2
[26]: https://purchase.aspose.com/temporary-license
[27]: https://docs.aspose.com/imaging/net/getting-started/
[28]: https://forum.aspose.com/
[29]: https://blog.aspose.com/2020/11/27/compress-png-jpeg-and-tiff-images-using-csharp/





