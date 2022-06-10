---
title: 'Resize Images and Convert CAD Drawings to Raster Formats in C# .NET'
date: Wed, 24 Sep 2014 16:29:31 +0000
draft: false
url: /2014/09/24/resize-images-proportionally-convert-cad-drawings-to-raster-formats-much-more-with-aspose.imaging-for-.net-2.6.0/
author: Babar Raza
summary: ''
tags: ['Adjust brightness contrast and gamma in images', 'Babar Raza', 'Convert CAD to Raster Image', 'Resize images proportionally in Csharp']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose-Imaging-for-net_100.png" alt="">}}


We are pleased to announce the monthly release of Aspose.Imaging for .NET, version 2.6.0. We have been working hard to bring the useful improvements with this edition of the Aspose.Imaging API. You can start exploring the newly added features & enhancements immediately, but before you head to the [download section][1], here is a look at just a few of the biggest features in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the link above. In case you are planning to upgrade the API from any previous release, we strongly suggest you to go through the Public API Changes in reference to Aspose.Imaging for .NET 2.6.0.

## Resize Images Proportionally in C#

This is a long-awaited feature that will surely ease the developer's life who wish to resize the images while preserving the Aspect Ratio. With the release of Aspose.Imaging for .NET 2.6.0, the API has exposed the ResizeWidthProportionally and ResizeHeightProportionally methods to the base class Image. You have to use any of these methods to either pass the width or height to [resize the images proportionally][2].

{{< gist aspose-imaging b93073a27bcdd4fefc2821e113f0cb3a "Examples-CSharp-ModifyingAndConvertingImages-SimpleResizeImageProportionally-SimpleResizeImageProportionally.cs" >}}

## Convert CAD Drawings to Raster Image Formats

We had to provide this feature at some stage so why not now. With the latest enhancements to the Aspose.Imaging for .NET API, users can convert the CAD drawings such as DWG & DXF to raster image formats. In order to implement this feature, the API has exposed the CadRasterizationOptions class with properties that enable the customization of the rendering process. Users may set the page size for the resultant image, control the background and drawing color schema, shrink or expand the drawing to fit the resultant canvas and center the drawing as per application requirements.

{{< gist aspose-com-gists 88cdd0899132edaf0afff77d33d11ae5 "Src-ConvertingCAD-ConvertDrawingToRasterImage-ConvertDrawingToRasterImage.cs" >}}

## Support for Deflate and Adobe Deflate Compression

The TIFF (Tagged Image File Format) file format supports various types of compression whereas the compression type is stored as a tag (an integer value) in the file. One of such compression methods is Adobe Deflate (previously known as Deflate). Since the release of Aspose.Imaging for .NET 2.6.0, the API [supports both Deflate & Adobe Deflate compression methods for loading, converting & creating TIFF images][3].

## Conversion of Colored Images to Black n White & Grayscale

Aspose.Imaging for .NET API can be used to [convert colored images to Black n White or Grayscale format][4] for printing or archiving purposes. The API provides two Binarization algorithms (Binarization with Fixed Threshold & Binarization with Otsu Threshold) for this purpose. Whereas the conversion to grayscale images is done through the process of converting a continuous color tone to discontinues an array of gray shades.

## Adjust Brightness, Contrast & Gamma in Images

[Color adjustments][5] in reference to the digital images is one of the core features that most of the imaging libraries provide. These features are now also available with Aspose.Imaging for .NET 2.6.0. The API has exposed an easy to use mechanism by exposing AdjustBrightness, AdjustContrast and AdjustGamma methods to the RasterImage class.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][6] for a chat.




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.imaging-for-.net/entry574143.aspx
[2]: https://docs.aspose.com/display/imagingnet/Crop%2C+Rotate+and+Resize+Images#Crop,RotateandResizeImages-ResizeImageProportionally
[3]: https://docs.aspose.com/display/imagingnet/Manipulating+TIFF+Images#ManipulatingTIFFImages-SupportforDeflateandAdobeDeflateCompression
[4]: https://docs.aspose.com/display/imagingnet/Converting+Images#ConvertingImages-ConvertingImagestoBlacknWhiteandGrayscale
[5]: https://docs.aspose.com/display/imagingnet/Manipulating+DICOM+Formats
[6]: http://forum.aspose.com




