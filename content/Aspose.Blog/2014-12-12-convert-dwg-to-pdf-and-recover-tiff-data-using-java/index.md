---
title: 'Convert DWG to PDF and Recover TIFF Data using Java'
date: Fri, 12 Dec 2014 17:19:06 +0000
draft: false
url: /2014/12/12/convert-dwg-to-pdf-and-recover-tiff-data-using-java/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.Imaging Product Family']
---

Aspose.Imaging for Java 2.4.0 has been released and we are pleased to announce that this release contains many useful improvements, including the long-awaited feature of AutoCAD DWG Drawings to PDF conversion. Please refer to the release notes of [Aspose.Imaging for Java 2.4.0][1] for a full list of bug fixes and improvements. If you are planning to upgrade the API from any previous version, we would suggest you to check the Public API Changes section first.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Convert DWG Drawings to PDF in Java

With the release of 2.4.0, Aspose.Imaging for Java supports loading DWG files for conversion to PDF format. Currently we support reading AutoCAD 2004 DWG (version 16.0 Release 18) format only. We will add more DWG revisions with future releases of Aspose.Imaging APIs whereas the support for DWG 2005 and 2010 are on the top of our priority list.

DWG to PDF conversion uses the PdfOptions class to specify the resultant PDF page size, and additional settings such as which Layout to render, BackgroundColor, DrawType and ScaleMethod. These properties have to be set before calling the Image.Save method for converting DWG to PDF format. Please read more about Customizing CAD to PDF Conversion.

## Data Recovery for TIFF Image Format

The TIFF file format stores data in strips. When a few strips are damaged, other strips may still retain the correct information, therefore it is possible to recover the correct data strips by filling the damaged strips with a background color. The data recovery module offered by Aspose.Imaging allows the user to retrieve the correct data portions (strips) in a similar fashion. In order to assist the users, Aspose.Imaging provides two data recovery modes, ConsistentRecover and MaximalRecover, which provide different results depending on the user's data recovery needs.

## Dithering Support for the RasterImage Class

Aspose.Imaging provides dithering support for the RasterImage class by introducing the DitheringSettings property. The DitheringMode class, now available in the com.aspose.imaging.dithering package, specifies the dithering to be applied. The dithering feature needs to implicitly or explicitly call the RasterImage.LoadPixels method after the RasterImage.DitheringSettings have been specified. Please check the complete detailed article on the link shared above.

## Raw Data Processing

Another exciting feature that is now available for public use is Raw Data Processing. Prior to 2.4.0, Aspose.Imaging used Color\[\] to internally store data. This approach had issues. First of all, an array of structs affected the performance during copy operations. Secondly, the Color struct required more memory for data storage because the API had to store additional system information together with 4 bytes of data.

With this release, we have partially switched the internal structure to use byte\[\] instead Color\[\] in order to assist developers in getting the best performance out of Aspose.Imaging API. At the moment this system has been introduced for BMP file format only, but soon all other image formats will be supported too.

## Add Thumbnails to EXIF & JFIF Segments of JPEG Images

Aspose.Imaging has exposed additional properties to add thumbnails to EXIF and JFIF data segments of JPEG images. Both types of segments can store only 65,535 bytes of data including the thumbnail image according to the JPEG specifications, therefore Aspose.Imaging API will throw appropriate exception in case the added image is bigger than the specified limit.

## Support for Image Cropping

Aspose.Imaging now provides the long awaited feature of image cropping for the RasterImage class by introducing the crop method. There are two overload versions of thecrop method available based on two different approaches as discussed below,

*   **Shift Mode**: One of the overloads accepts 4 integer parameters denotes as Left, Right, Top and Bottom. Based on these values, the Crop method shrinks the image boundaries toward the center of the image while discarding everything outside the boundaries.
*   **Rectangle Mode**: As the name suggests, this mechanism can be used to highlight a particular area by cutting it out of the image. The area should be defined using an instance of the Rectangle class and passed to the other overload of the crop method.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][2] for a chat.




[1]: https://products.aspose.com/imaging/java
[2]: http://www.aspose.com/community/forums/aspose.imaging-product-family/498/showforum.aspx




