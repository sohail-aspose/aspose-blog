---
title: 'Create Animated PNG Images using C# or VB.NET'
seoTitle: ""
description: ""
date: Thu, 02 Jul 2020 06:24:09 +0000
draft: false
url: /2020/07/02/create-animated-png-using-csharp-or-vb.net/
author: Usman Aziz
summary: ''
tags: ['Animated PNG to GIF in csharp', 'Tiff to APNG using csharp', 'create APNG using csharp', 'create animated PNG using csharp']
categories: ['Aspose.Imaging Product Family']
---

[Animated PNG][1] (Portable Network Graphics) is an extension to PNG format to incorporate the animations. Just like animated GIFs, the APNG format is used to present the animations. An edge of APNG over GIF is, it supports 24-bit transparency whereas GIF supports only 8-bit. Furthermore, APNG provides a smoother animation as compared to an animated GIF. In this article, I'll show you how to **create the animated PNG (APNG)** images from an image or multi-page Tiff and **export APNG to animated GIF** programmatically using C# (or VB.NET).

*   [.NET API for Animated PNG Images][2]
*   [Create animated PNG from an image][3]
*   [Create animated PNG from multi-page Tiff file][4]
*   [Export animated PNG to animated GIF][5]

## .NET API for Animated PNG Images {#NET-API-for-Animated-PNG-Images}

Aspose offers its [.NET Imaging API][6] to create or manipulate popular image formats including animated PNG using C# or VB.NET. We'll leverage the capabilities of _Aspose.Imaging for .NET_ to create or export animated PNG images. You can either [download][7] the API's DLL or install it within your .NET application using [NuGet][8].

```
PM> Install-Package Aspose.Imaging
```

## Create Animated PNG from an Image using C# {#Create-animated-PNG-from-a-PNG-image}

Aspose.Imaging for .NET lets you create an animated PNG from a single-page image such as PNG by setting the custom animation and frame duration. The following are the steps to perform this operation.

*   Load the PNG image into a [RasterImage][9] object using [Image.Load(String)][10] method.
*   Set [ApngOptions][11] properties as per your requirements.
*   Use the [ApngImage][12] class to create the animated PNG.
*   Update the gamma of each frame using [ApngFrame.AdjustGamma(Single)][13] method.
*   Create animated PNG using [ApngImage.Save()][14] method.

The following code sample shows how to create an animated PNG (APNG) from a PNG image using C#.

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "Examples-Create-APNG-animation-from-single-image.cs" >}}

### Source PNG



{{< figure align=center src="images/Static-PNG.jpg" alt="PNG to APNG in C#">}}


### Animated PNG

## Create Animated PNG from Multi-Page Tiff using C# {#Create-animated-PNG-from-multi-page-Tiff-file}

You can also use a multi-page Tiff file to create the animated PNG by setting the desired frame time. The following are the steps to create animated PNG from a Tiff file.

*   Load Tiff image within an object of [Image][15] class.
*   Save Tiff as APNG using [Image.Save(String, ImageOptionsBase)][16] method.

The following code sample shows how to create animated PNG from a Tiff file using C#.

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "Examples-Save-to-Animated-APNG-from-Multi-Page-Tiff.cs" >}}

### Source Tiff

You can download the source Tiff file from here.

### Animated PNG



{{< figure align=center src="images/Tiff-to-Animated-PNG.png" alt="TIFF to Animated PNG">}}


## Export Animated PNG to Animated GIF using C# {#Export-animated-PNG-to-animated-GIF}

You can also export an animated PNG image to an equivalent animated GIF. The following are the steps to export APNG to GIF.

*   Load the animated PNG into an [Image][17] object.
*   Export APNG to GIF using [Image.Save(String, GifOptions())][18] method.

The following code sample shows how to export animated PNG to GIF using C#.

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "Examples-Export-APNG-to-Gif.cs" >}}

### Source Animated PNG



{{< figure align=center src="images/Animated-PNG.png" alt="Animated PNG Image">}}


### Animated GIF



{{< figure align=center src="images/Animated-Gif.gif" alt="Animated PNG to GIF C#">}}


## Conclusion

In this article, you have learned how to create an animated PNG from different sources using C#. The step by step guide and code samples demonstrated how to create animated PNG from single-page PNG and multi-page Tiff as well as export animated PNG to an animated GIF using C#. You can learn more about manipulating APNG images using the documentation of the API.

## See Also

*   [Convert GIF Images to TIFF, PDF, PNG, JPG, or BMP using C#][19]




[1]: https://en.wikipedia.org/wiki/APNG
[2]: #NET-API-for-Animated-PNG-Images
[3]: #Create-animated-PNG-from-a-PNG-image
[4]: #Create-animated-PNG-from-multi-page-Tiff-file
[5]: #Export-animated-PNG-to-animated-GIF
[6]: https://products.aspose.com/imaging/net
[7]: https://downloads.aspose.com/imaging/net
[8]: http://nuget.org/packages/Aspose.imaging
[9]: https://apireference.aspose.com/imaging/net/aspose.imaging/rasterimage
[10]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/load/methods/2
[11]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/apngoptions
[12]: https://apireference.aspose.com/imaging/net/aspose.imaging.fileformats.apng/apngimage
[13]: https://apireference.aspose.com/imaging/net/aspose.imaging/rastercachedimage/methods/adjustgamma
[14]: https://apireference.aspose.com/imaging/net/aspose.imaging/image/methods/save
[15]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[16]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[17]: https://apireference.aspose.com/imaging/net/aspose.imaging/image
[18]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[19]: https://blog.aspose.com/2020/06/10/convert-gif-images-to-tiff-pdf-png-jpg-or-bmp-using-csharp/





