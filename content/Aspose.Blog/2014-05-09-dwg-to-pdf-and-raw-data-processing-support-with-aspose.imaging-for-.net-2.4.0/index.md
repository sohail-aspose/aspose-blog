---
title: 'Convert DWG to PDF and Process Raw Data in Images using C#'
date: Fri, 09 May 2014 17:25:10 +0000
draft: false
url: /2014/05/09/dwg-to-pdf-and-raw-data-processing-support-with-aspose.imaging-for-.net-2.4.0/
author: Babar Raza
summary: ''
tags: ['Aspose.Imaging API', 'AutoCAD DWG', 'AutoCAD DXF', 'AutoCAD formats', 'Babar Raza', 'DWG', 'DWG to PDF', 'Imaging', 'PDF']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose-Imaging-for-net_100.png" alt="">}}


[Aspose.Imaging][1] 2.4.0 has been released and we are pleased to announce that this month’s release contains many useful improvements, including the long awaited feature of DWG AutoCAD Drawings to PDF conversion. You can immediately download the latest Aspose.Imaging for .NET release from the [download section][2], and start exploring the features & enhancements we've added.

Here is a look at a few of the biggest features in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the link above.

## DWG Drawings to PDF Conversion

With the release of 2.4.0, Aspose.Imaging for .NET supports loading DWG files for conversion to PDF format. Currently we support reading AutoCAD 2004 DWG (version 16.0 Release 18) format only, but will add more DWG versions with future releases of Aspose.Imaging APIs.

DWG to PDF conversion uses the PdfOptions class to specify the output PDF page size, and additional settings such as which Layout to render, BackgroundColor, DrawType and ScaleMethod. These properties have to be set before calling the Image.Save method for converting DWG to PDF format.

## Raw Data Processing

Another exciting feature that is now available for public use is Raw Data Processing. Prior to 2.4.0, Aspose.Imaging used Color\[\] to internally store data. This approach had issues. First of all, an array of structs affected the performance during copy operations. Secondly, the Color struct required more memory for data storage because the API had to store additional system information together with 4 bytes of data.

With this release, we have partially switched the internal structure to use byte\[\] instead Color\[\] in order to assist developers in getting the best performance out of Aspose.Imaging API. At the moment this system has been introduced for BMP file format only, but soon all other image formats will be supported too.

## Add Thumbnails to EXIF & JFIF Segments of JPEG Images

Aspose.Imaging has exposed additional properties to add thumbnails to EXIF and JFIF data segments of JPEG images. Both types of segments can store only 65,535 bytes of data including the thumbnail image according to the JPEG specifications, therefore Aspose.Imaging API will throw appropriate exception in case the added image is bigger than the specified limit.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][3] for a chat.




[1]: https://products.aspose.com/imaging
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.imaging-for-.net/default.aspx
[3]: http://forum.aspose.com




