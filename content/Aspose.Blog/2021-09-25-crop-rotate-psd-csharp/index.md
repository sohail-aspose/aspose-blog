---
title: 'Rotate or Crop PSD Image using C#'
seoTitle: "Crop or Rotate a PSD file Programmatically with C#"
description: "Crop or rotate a PSD image file using C# in your .NET application. Crop by shift, crop by rectangle or rotate PSD at any angle."
date: Sat, 25 Sep 2021 09:27:00 +0000
draft: false
url: /2021/09/25/crop-rotate-psd-csharp/
author: Farhan Raza
summary: 'PSD images are frequently used to design graphics and visuals. In some cases, you might want to crop or rotate a PSD image for different aesthetic requirements. In this article, you will learn how to crop or rotate a PSD image using C#. Please go through the following headings for more information.'
tags: ['Crop PSD', 'Crop PSD in csharp', 'Rotate PSD', 'Rotate PSD in csharp']
categories: ['Aspose.PSD Product Family']
---



{{< figure align=center src="images/Crop-Resize-PSD.jpg" alt="Crop Rotate PSD">}}


[PSD][1] images are frequently used to design graphics and visuals. In some cases, you might want to crop or rotate a PSD image for different aesthetic requirements. In this article, you will learn how to crop or rotate a PSD image using C#. Please go through the following headings for more information:

*   [Rotate or Crop a PSD Image – C# .NET API Installation][2]
*   [Crop a PSD Image with Shift Approach using C#][3]
*   [Crop a PSD Image with Rectangular Coordinates in C#][4]
*   [Rotate a PSD Image at any Angle using C#][5]

## Rotate or Crop a PSD Image – C# .NET API Installation {#section1}

[Aspose.PSD for .NET][6] API supports creating, editing, and manipulating PSD and many other Photoshop file formats. You can easily set up the API by downloading the DLL file from the [New Releases][7], or with the following [NuGet][8] installation command in Microsoft Visual Studio:

```
PM> Install-Package Aspose.PSD
```

## Crop a PSD Image with Shift Approach using C# {#section2}

You can crop a PSD image by moving the contents towards the center of the image. The following steps show how to crop a PSD image while shifting contents:

1.  Load the input PSD image using the [RasterImage][9] class instance.
2.  Cache the PSD image with [CacheData][10] method.
3.  Specify the shift values and call the [Crop][11] method.
4.  Save the output cropped image.

The code snippet explains how to crop a PSD image programmatically in C#:

{{< gist aspose-com-gists f93a3760be357b8f0ccd2f984f236816 "Crop-PSD-Shift.cs" >}}

## Crop a PSD Image with Rectangular Coordinates in C# {#section3}

You can crop any portion of a PSD image by using rectangular coordinates. Please follow the steps below in order to crop the PSD image with Rectangular coordinates:

1.  Load the input PSD file with [RasterImage][12] class.
2.  Cache the input image for enhanced performance.
3.  Initialize a [Rectangle][13] class object with the desired coordinates.
4.  Crop the PSD image and save the output file.

The following code snippet demonstrates how to crop a PSD image using rectangular coordinates in C#:

{{< gist aspose-com-gists f93a3760be357b8f0ccd2f984f236816 "Crop-PSD-Rectangle.cs" >}}

## Rotate a PSD Image at any Angle using C# {#section4}

You can rotate a PSD image at any angle with the following steps:

1.  Load the input PSD image with [RasterImage][14] class.
2.  Cache the image improved performance.
3.  Set the angle of rotation in the [Rotate][15] method.
4.  Save the rotated output PSD file.

The code snippet below explains how to rotate a PSD image programmatically in C#:

{{< gist aspose-com-gists f93a3760be357b8f0ccd2f984f236816 "Rotate-PSD.cs" >}}

## Get Free Evaluation License

You can request a [free evaluation license][16] to test the API in its full capacity.

## Conclusion

In conclusion, you have learned how to crop or rotate a PSD image programmatically with C#. You can integrate the feature into your .NET-based applications. Please visit the [documentation][17] section for further details and feel free to write to us at the [free support forum][18], in case of any inquiries.

## See Also

[Convert PSB to PDF, JPG, or PSD Programmatically using C#][19]




[1]: https://docs.fileformat.com/image/psd/
[2]: #section1
[3]: #section2
[4]: #section3
[5]: #section4
[6]: https://products.aspose.com/psd/net
[7]: https://downloads.aspose.com/psd/net
[8]: https://www.nuget.org/packages/Aspose.PSD/
[9]: https://apireference.aspose.com/psd/net/aspose.psd/rasterimage
[10]: https://apireference.aspose.com/psd/net/aspose.psd/datastreamsupporter/methods/cachedata
[11]: https://apireference.aspose.com/psd/net/aspose.psd/rasterimage/methods/crop/index
[12]: https://apireference.aspose.com/psd/net/aspose.psd/rasterimage
[13]: https://apireference.aspose.com/psd/net/aspose.psd/rectangle
[14]: https://apireference.aspose.com/psd/net/aspose.psd/rasterimage
[15]: https://apireference.aspose.com/psd/net/aspose.psd/rasterimage/methods/rotate/index
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/display/psdnet/Home
[18]: https://forum.aspose.com/c/psd
[19]: https://blog.aspose.com/2021/07/16/convert-psb-to-pdf-jpg-or-psd-programmatically-using-csharp/




