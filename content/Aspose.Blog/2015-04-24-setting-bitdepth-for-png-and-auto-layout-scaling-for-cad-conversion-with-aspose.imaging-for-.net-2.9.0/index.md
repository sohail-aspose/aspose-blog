---
title: 'Set BitDepth for PNG and Auto Layout Scaling for CAD Conversion using C#'
date: Fri, 24 Apr 2015 12:39:24 +0000
draft: false
url: /2015/04/24/setting-bitdepth-for-png-and-auto-layout-scaling-for-cad-conversion-with-aspose.imaging-for-.net-2.9.0/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose-Imaging-for-net_100.png" alt="">}}


Aspose.Imaging for .NET 2.9.0 has been released, and we are pleased to announce that this month’s release contains many useful improvements. You can now [download][1] the latest build and start exploring the newly added features & enhancements. In case you are planning to upgrade the API from any previous revision then we would strongly recommend you to check the [Public API Change][2] section to know what has been changed since your current version of the API.

While you are waiting for the latest release to download, here is a look at a few of the worth mentioning features in this month’s release.

## Setting BitDepth for PNG Image Format

Bit depth in imaging is the number of bits used to indicate the color of a single pixel in a bitmap image. Like all other bitmap formats, PNG color depth is also represented in bits such as 1-bit (2 colors), 2-bit (4 colors), 4-bit (16 colors) and 8-bit (256 colors).

Aspose.Imaging for .NET API has exposed a very easy to use mechanism to [set the BitDepth for existing as well as new PNG images][3]. With the release of version 2.9.0, the API has provided the BitDepth property for the PngOptions class that can be used to set the BitDepth as 1, 2, 4 or 8 bits for grayscale and indexed color types, whereas, for all other color types only 8 bits are supported at the moment.

Here is the simplest code snippet that sets the bit depth of 1-BitPerPixel for an existing PNG image.

{{< gist aspose-imaging b93073a27bcdd4fefc2821e113f0cb3a "Examples-CSharp-ModifyingAndConvertingImages-PNG-SpecifyBitDepth-SpecifyBitDepth.cs" >}}

## Setting Auto Layout Scaling

Most of the CAD drawings have more than one layouts stored in a single file, and each layout could have different dimensions. While rendering such CAD drawings to PDF, each page of the PDF could have different scaling according to the layout size. In order to make the rendering homogeneous, the Aspose.Imaging APIs have exposed the CadRasterizationOptions.AutomaticLayoutsScaling property. Its default value is false but when set to true, the API will try to search for a corresponding scale for each separate layout and draw them in corresponding manner by performing automatic re-size operation according to page size.

Here is how the CadRasterizationOptions.AutomaticLayoutsScaling property works in collaboration with CadRasterizationOptions.ScaleMethod settings.

*   If ScaleMethod is set to ScaleType.ShrinkToFit or ScaleType.GrowToFit with AutomaticLayoutsScaling set to false then all layouts (including the Model) will be processed according to first option.
*   If ScaleMethod is set to ScaleType.ShrinkToFit or ScaleType.GrowToFit with AutomaticLayoutsScaling set to true then all layouts (except Model) will be processed according to their size whereas the Model will be processed according to first option.
*   If ScaleMethod is set to ScaleType.None with AutomaticLayoutsScaling set to true or false then no scaling will be performed.

## Other Enhancements & Fixes

Aspose.Imaging for .NET 2.9.0 has also made the following worth mentioning improvements.

*   Enhanced the image loading & saving mechanism of JPEG, BMP & GIF file formats.
*   Improved the CAD loading mechanism for head-less CAD drawing files.
*   Provided support for TIFF files having PackBits compression.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][4] for a chat.




[1]: https://downloads.aspose.com/imaging/net
[2]: https://docs.aspose.com/display/imagingnet/Migrating+from+Earlier+Versions+of+Aspose.Imaging
[3]: https://docs.aspose.com/display/imagingnet/Manipulating+PNG+Images#ManipulatingPNGImages-SpecifyingBitDepthforPNGImages
[4]: http://forum.aspose.com/




