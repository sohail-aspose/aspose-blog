---
title: 'Rotate Image at Specified Angle using C# or VB.NET'
date: Thu, 24 Jul 2014 16:13:01 +0000
draft: false
url: /2014/07/24/rotate-an-image-to-any-angle-using-csharp-or-vb.net/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose-Imaging-for-net_100.png" alt="">}}


We are pleased to announce the monthly release of [Aspose.Imaging for .NET][1], version 2.5.0. Our team has been hard at work bringing many useful improvements to this edition of the Aspose.Imaging API. You can start exploring the newly added features & enhancements immediately, but before you head to the [download section][2], here is a look at just a few of the biggest features in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the link above. In case are going to upgrade the API, please refer to the article [Public API Changes][3] in reference to Aspose.Imaging for .NET 2.5.0.

## Rotate an Image to any Angle using C#

With this release, the RasterImage class provides a Rotate method to help users who wish to rotate an image at a specific angle. The RasterImage.Rotate method accepts three parameters as listed below.

1.  Rotation Angle: A float type parameter specifies the rotation angle on which the image has to be rotated. A positive value rotates the image clockwise whereas a negative value performs an anticlockwise rotation.
2.  Resize Proportionally: A Boolean type parameter specifies if the image size has to changed according to the rotated rectangle (corner points) projections. If set to false, the image dimensions are untouched and only the internal image contents are rotated.
3.  Background Color: A color type parameter specifies the color to be filled in the background of the rotated image.

The following code sample shows how to rotate an image to a particular angle in C#.

{{< gist aspose-imaging b93073a27bcdd4fefc2821e113f0cb3a "Examples-CSharp-ModifyingAndConvertingImages-RotatingImageOnSpecificAngle-RotatingImageOnSpecificAngle.cs" >}}

## Set Resolution for PNG Image Format in C#

With the release of 2.5.0, Aspose.Imaging for .NET supports setting the resolution for PNG image format. In order to provide this feature, the Aspose.Imaging for .NET API has exposed the ResolutionSetting class. The PngOptions class now has a property by the name ResolutionSettings that accepts an instance of the ResolutionSetting class to specify the horizontal & vertical resolution.

## Specify Transparency for PNG Images in C#

One of the advantages of saving images in PNG format is that PNG can have a transparent background. Aspose.Imaging for .NET has provided the feature to [specify the transparency for PNG images][4]. Starting from 2.5.0, Aspose.Imaging for .NET API has exposed the ResolutionSettings property for the PngOptions class that accepts an instance of the TransparentColorSetting class to specify any color that can be set as the transparent color in the output image.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][5] for a chat.




[1]: https://products.aspose.com/imaging/net
[2]: https://downloads.aspose.com/imaging/net
[3]: https://docs.aspose.com/display/imagingnet/Public+API+Changes+in+Aspose.Imaging+2.5.0
[4]: https://docs.aspose.com/display/imagingnet/Raw+Data+Processing
[5]: http://forum.aspose.com




