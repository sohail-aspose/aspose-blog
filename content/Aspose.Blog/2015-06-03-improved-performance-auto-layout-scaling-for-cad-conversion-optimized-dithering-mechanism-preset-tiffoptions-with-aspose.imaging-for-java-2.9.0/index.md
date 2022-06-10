---
title: 'Improved Performance, Auto Layout Scaling for CAD Conversion, Optimized Dithering Mechanism &amp; Preset TiffOptions with Aspose.Imaging for Java 2.9.0'
date: Wed, 03 Jun 2015 07:22:34 +0000
draft: false
url: /2015/06/03/improved-performance-auto-layout-scaling-for-cad-conversion-optimized-dithering-mechanism-preset-tiffoptions-with-aspose.imaging-for-java-2.9.0/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.Imaging Product Family']
---

[![Aspose.Imaging for Java logo][1]](http://www.aspose.com/java/imaging-component.aspx "Aspose.Imaging for Java API")We are pleased to announce the release of Aspose.Imaging for Java 2.9.0. This month's release contains many useful improvements & features from Aspose.Imaging for .NET 2.8.0 & 2.9.0, where the most worth mentioning enhancement is the new improved imaging core. Please refer to the release notes of [Aspose.Imaging for Java 2.9.0][2] for a full list of bug fixes and improvements along with sample code snippets to the newly added features. If you are planning to upgrade the Aspose.Imaging for Java API to the latest revision, we strongly suggest you to check the Public API Change section to know what has been changed in the API since your current version.

While you are downloading the latest revision, here is a look at just a few of the showcased features of this release.

## Improved Imaging Core

Aspose.Imaging for Java API has improved the imaging core for performance considerations by converting the internal structure to utilize the byte array instead of the com.aspose.imaging.Color array. With these changes in place, the latest revision of the Aspose.Imaging for Java 2.9.0 is less resource consuming and more efficient as compared to any of its predecessors.

Previously, the imaging core used the com.aspose.imaging.Color array to store the pixel information due to which each pixel had to occupy 24 bytes in the memory. This schema proved to be the performance bottleneck in scenarios where images having huge dimensions have to be processed because image required more memory to process and hence more time to flush the data.

## Setting Auto Layout Scaling

Most of the CAD drawings have more than one layouts stored in a single file, and each layout could have different dimensions. While rendering such CAD drawings to PDF, each page of the PDF could have different scaling according to the layout size. In order to make the rendering homogeneous, the Aspose.Imaging APIs have exposed the CadRasterizationOptions.AutomaticLayoutsScaling property. Its default value is false but when set to true, the API will try to search for a corresponding scale for each separate layout and draw them in corresponding manner by performing automatic re-size operation according to page size. Please check the article on Customizing CAD Conversion for more details and source code snippets for this feature.

## Optimized Dithering Mechanism

The dithering process is now more optimized and predictable. All you need to do is use the newly exposed RasterImage.Dither method instead of creating & setting DitheringSettings and RawDitheringMethod properties as we used to do with previous revisions of Aspose.Imaging for Java API. Upon calling the RasterImage.dither method the dithering is performed right in-place and you can then review the dithered results by loading pixels or raw data.

## Preset TiffOptions

In order to facilitate the users and to avoid the miss-configuration of the TiffOptions instance, the Aspose.Imaging for Java API has exposed another constructor for that TiffOptions class that accepts a parameter of type TiffExpectedFormat. Based on the selected value from the TiffExpectedFormat enumeration, the API auto configures all the mandatory properties for the TiffOptions instance in order to produce the desired results. Please check the possible values of TiffExpectedFormat parameter and their details at TiffOptions' Configurations.

## Auto-Rotate Jpeg Images

This is a long awaited feature that will surely ease the developer's life who wish to auto-rotate the Jpeg images to correct the orientation. Most digital cameras stores the orientation information along with the image data as EXIF tags of the JEPG images. Aspose.Imaging APIs use this information to perform the auto rotation on the Jpeg images to correct the orientation.

## Setting BitDepth for PNG Image Format

Bit depth in imaging is the number of bits used to indicate the color of a single pixel in a bitmap image. Like all other bitmap formats, PNG color depth is also represented in bits such as 1-bit (2 colors), 2-bit (4 colors), 4-bit (16 colors) and 8-bit (256 colors).

Aspose.Imaging for .NET API has exposed a very easy to use mechanism to set the BitDepth for existing as well as new PNG images. With the release of version 2.9.0, the API has provided the BitDepth property for the PngOptions class that can be used to set the BitDepth as 1, 2, 4 or 8 bits for grayscale and indexed color types, whereas, for all other color types only 8 bits are supported at the moment.

## Other Enhancements & Fixes

Aspose.Imaging for Java 2.9.0 has also made the following worth mentioning improvements.

*   Enhanced the image loading & saving mechanism of JPEG, BMP & GIF file formats.
*   Improved the CAD loading mechanism for head-less CAD drawing files.
*   Provided support for TIFF files having PackBits compression.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][3] for a chat.




[1]: https://docs.aspose.com/display/emailproductfamily/Home "Aspose.Imaging for Java logo"
[2]: http://www.aspose.com/community/files/72/java-components/aspose.imaging-for-java/entry631409.aspx "Download Aspose.Imaging for Java 2.9.0"
[3]: http://www.aspose.com/community/forums/aspose.imaging-product-family/498/showforum.aspx




