---
title: 'Create Thumbnails and Crop Images Programmatically using C#'
date: Wed, 02 Apr 2014 19:12:06 +0000
draft: false
url: /2014/04/02/thumbnail-creation-support-for-image-cropping-in-aspose.imaging-for-.net-2.3.0/
author: Babar Raza
summary: ''
tags: ['Aspose.Imaging', 'AutoCAD Drawings', 'AutoCAD Layouts', 'Babar Raza', 'DXF Drawings', 'DXF Layout', 'DXF to PDF', 'Image Cropping', 'Imaging Library', 'JPEG EXIF', 'JPG Thumbnail', 'Raster Crop', 'Rectangle Cropping', 'Shift Cropping', 'Thumbnails']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose-Imaging-for-net_100.png" alt="">}}


Aspose.Imaging 2.3.0 has been released and we are pleased to announce that this month’s release contains many useful improvements and features. You can download the latest release of Aspose.Imaging from the [download section][1].

Here is a look at a few of the biggest features in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the link above.

## Create Thumbnails for JPEG Images using C#

A thumbnail is a small copy of an image mostly used for recognition purposes when more images are stored in a library. Usually, when the image is shot with a digital camera, the thumbnail information is stored in the image metadata and can be retrieved through imaging libraries such as Aspose.Imaging for .NET API. With this release, Aspose.Imaging has provided a convenient mechanism to [extract the thumbnail information from the image metadata][2].

## Crop Images using C#

Aspose.Imaging now provides the long-awaited feature of [image cropping][3] for the RasterImage class by introducing the Crop method. There are two overload versions of the Crop method available based on two different approaches as discussed below,

*   **Shift Mode**: One of the overloads accepts 4 integer parameters denotes as Left, Right, Top and Bottom. Based on these values, the Crop method shrinks the image boundaries toward the center of the image while discarding everything outside the boundaries.
*   **Rectangle Mode**: As the name suggests, this mechanism can be used to highlight a particular area by cutting it out of the image. The area should be defined using an instance of the Rectangle class and passed to the other overload of the Crop method.

## Export Specific Layout in DXF Drawing to PDF

This feature has been migrated to [Aspose.CAD for .NET][4] and the API facilitates [exporting a specific layer of the AutoCAD DXF drawing to PDF format][5]. Furthermore, it adds another exciting feature that allows you to [select a layout from a DXF drawing, and export it to PDF][6].

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][7] for a chat.




[1]: https://downloads.aspose.com/imaging/net
[2]: https://docs.aspose.com/display/imagingnet/Manipulating+JPEG+Images#ManipulatingJPEGImages-CreatingThumbnailsfromJPEGImages
[3]: https://docs.aspose.com/display/imagingnet/Crop%2C+Rotate+and+Resize+Images#Crop,RotateandResizeImages-CroppingImages
[4]: https://products.aspose.com/cad/net
[5]: https://docs.aspose.com/display/cadnet/DXF+Drawings#DXFDrawings-ExportingSpecificLayerofDXFDrawingstoPDF
[6]: https://docs.aspose.com/display/cadnet/DXF+Drawings#DXFDrawings-ExportingSpecificLayerofDXFDrawingstoImage
[7]: http://forum.aspose.com




