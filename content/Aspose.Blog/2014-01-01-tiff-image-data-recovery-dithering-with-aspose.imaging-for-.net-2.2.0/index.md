---
title: 'TIFF Image Data Recovery &amp; Dithering with Aspose.Imaging for .NET 2.2.0'
date: Wed, 01 Jan 2014 13:24:34 +0000
draft: false
url: /2014/01/01/tiff-image-data-recovery-dithering-with-aspose.imaging-for-.net-2.2.0/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.Imaging Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/09/aspose-Imaging-for-net_100.png)Aspose.Imaging 2.2.0 has been released and we are very pleased to announce that this month’s release contains many useful improvements and features. You can download the latest release of Aspose.Imaging from the [download section][2].

Here is a look at just a few of the biggest features in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the link above.

## Data Recovery for TIFF Image Format

The TIFF file format stores data in strips. When strips are damaged, other strips may still retain the correct information, therefore it is possible to recover the correct data strips by filling the damaged strips with a background color. The data recovery module offered by Aspose.Imaging allows the user to retrieve the correct data portions (strips) in a similar fashion. In order to assist users, Aspose.Imaging provides two data recovery modes, ConsistentRecover and MaximalRecover, which provide different results depending on the user's data recovery needs.

## Dithering Support for the RasterImage Class

Aspose.Imaging provides dithering support for the RasterImage class by introducing the DitheringSettings property. The DitheringMode class, now available in the Aspose.Imaging.Dithering namespace, specifies the dithering to be applied. The dithering feature needs to implicitly or explicitly call to the RasterImage.LoadPixels method after the RasterImage.DitheringSettings have been specified. Please check the complete detailed article on the link shared above.

## Export Specific Layer in DXF Drawing to PDF

Previously, Aspose.Imaging allowed you to convert AutoCAD DXF drawings to PDF. With this release Aspose.Imaging adds another exciting feature that allows the user to select a layer from a DXF drawing, and export it to PDF.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][3] for a chat.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/09/aspose-Imaging-for-net_100.png "aspose-Imaging-for-net_100"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.imaging-for-.net/default.aspx "Aspose.Imaging for .NET 2.2.0"
[3]: http://www.aspose.com/community/forums/aspose.imaging-product-family/498/showforum.aspx




