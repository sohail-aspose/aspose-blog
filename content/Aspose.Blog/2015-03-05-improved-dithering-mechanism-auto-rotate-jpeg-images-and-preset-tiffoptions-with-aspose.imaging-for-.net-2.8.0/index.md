---
title: 'Improved Dithering Mechanism, Auto-Rotate Jpeg Images and Preset TiffOptions with Aspose.Imaging for .NET 2.8.0'
date: Thu, 05 Mar 2015 17:09:10 +0000
draft: false
url: /2015/03/05/improved-dithering-mechanism-auto-rotate-jpeg-images-and-preset-tiffoptions-with-aspose.imaging-for-.net-2.8.0/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.Imaging Product Family']
---

![](https://blog.aspose.com/wp-content/uploads/sites/2/2013/09/aspose-Imaging-for-net_100.png "aspose-Imaging-for-net_100")We are pleased to announce the monthly release of Aspose.Imaging for .NET, version 2.8.0. You can start exploring the newly added features & enhancements immediately, but before you head to the [download section][1], here is a look at just a few of the biggest features in this month’s release. For a full list of bug fixes and improvements please refer to the download page in the link above. In case you are planning to upgrade the API from any previous release, we strongly suggest you to go through the Public API Changes section to know what has been changed since your current version of the API.

## Optimized Dithering Mechanism

The dithering process is now more optimized and predictable. All you need to do is use the newly exposed RasterImage.Dither method instead of creating & setting DitheringSettings and RawDitheringMethod properties as we used to do with previous revisions of Aspose.Imaging for .NET API. Upon calling the RasterImage.Dither method the dithering is performed right in-place and you can then review the dithered results by loading pixels or raw data.

The RasterImage.Dither method accepts two parameters where first parameter is of type DitheringMethod with two possible options, that are; FloydSteinbergDithering and ThresholdDithering. The second parameter to RasterImageDither method is the BitCount in integer. BitCount defines the sampling size for the dithering result. The allowed values are 1, 4, 8 generating palettes with 2, 4 and 256 colors respectively.

Optimized code for dithering is as follow.

```
 //Create an instance of JpegImage and load an image as of JpegImage
using (JpegImage image = (JpegImage)Image.Load(sourcePath))
{
    //Peform Floyd Steinberg dithering on the current image
    image.Dither(DitheringMethod.ThresholdDithering, 4);
    //Save the resultant image
    image.Save(destinationPath);
} 
```

## Preset TiffOptions

In order to facilitate the users and to avoid the miss-configuration of the TiffOptions instance, the Aspose.Imaging for .NET API has exposed another constructor for that TiffOptions class that accepts a parameter of type TiffExpectedFormat. Based on the selected value from the TiffExpectedFormat enumeration, the API auto configures all the mandatory properties for the TiffOptions instance in order to produce the desired results. Please check the possible values of TiffExpectedFormat parameter and their details at TiffOptions' Configurations.

## Auto-Rotate Jpeg Images

This is a long awaited feature that will surely ease the developer's life who wish to auto-rotate the Jpeg images to correct the orientation. Most digital cameras stores the orientation information along with the image data as EXIF tags of the JEPG images. Aspose.Imaging APIs use this information to perform the auto rotation on the Jpeg images to correct the orientation.

With this release, Aspose.Imaging for .NET has exposed the JpegImage.AutoRotate method. Here is how you can use the aforesaid method.

```
 //Load a Jpeg image from file path location or stream
using (JpegImage image = (JpegImage)Image.Load(sourcePath))
{
    //Perform the automatic rotation on the image 
    //depending on the orientation data stored in the EXIF
    image.AutoRotate();
    //Save the result on disc or stream
    image.Save(destinationPath);
} 
```

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][2] for a chat.




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.imaging-for-.net/entry610200.aspx "Download Aspose.Imaging for .NET 2.8.0"
[2]: http://www.aspose.com/community/forums/aspose.imaging-product-family/498/showforum.aspx




