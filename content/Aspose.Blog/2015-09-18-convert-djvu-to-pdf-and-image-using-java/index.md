---
title: 'Convert DjVu Files to PDF and Image Formats using Java'
date: Fri, 18 Sep 2015 13:19:39 +0000
draft: false
url: /2015/09/18/convert-djvu-to-pdf-and-image-using-java/
author: Babar Raza
summary: ''
tags: ['Babar Raza', 'Convert DjVu to Image using Java', 'Convert DjVu to PDF using Java']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose_imaging-for-java.jpg" alt="">}}


We are pleased to announce September's release of Aspose.Imaging for Java. This month's release contains many useful improvements including the long-awaited support for DjVu file format. Please refer to the release notes of [Aspose.Imaging for Java 3.0.0][1] for a full list of bug fixes and improvements along with sample code snippets for newly added features. If you are planning to upgrade the API to the latest revision, we strongly suggest you check the [Public API Change][2] section to know what has been changed in the public API since your current version.

While you are downloading the latest build, here is a look at just a few of the showcased features of this release.

## Convert DjVu Files using Java

DjVu file format is becoming popular as an alternative to PDF because it has smaller file size as compared to PDF. DjVu format can also be considered as a superior alternative to PDF for digital documents, to TIFF for scanned bitonal documents, to JPEG and JPEG2000 for photographs and pictures, and to GIF for large palatalized images.

With the release of Aspose.Imaging for Java 3.0.0, the API has provided the support for loading DjVu files for possible conversion to raster image formats as well as PDF. In order to provide this support, the API has exposed DjvuImage class along with many new helping classes, methods & properties listed in the [Public API Changes in Aspose.Imaging for Java 3.0.0][3].

## Convert DjVu to Multi-Frame Raster Formats using Java

Like PDF & TIFF, the DjVu files can have multiple pages/frames therefore while converting the DjVu files to raster formats such as TIFF & GIF, all pages of DjVu are rendered to the resultant image by default. Here is the code to [convert all pages of DjVu to TIFF format][4].

{{< gist aspose-imaging 8c9bd83e0d07145ba0c1 "Examples-src-main-java-com-aspose-imaging-examples-djvu-ConvertDjvuToTiff-ConvertDjvuToTiff.java" >}}

## Convert of DjVu to PDF Format using Java

Aspose.Imaging for Java 3.0.0 can also be used to [convert the DjVu files to PDF][5] format while using the existing PdfOptions class. It is up to the user requirement if all DjVu pages or a subset of the pages are to be exported in PDF format.

The following code snippet demonstrates the usage of Aspose.Imaging for Java 3.0.0 to convert a subset of DjVu pages to PDF format.

{{< gist aspose-imaging 8c9bd83e0d07145ba0c1 "Examples-src-main-java-com-aspose-imaging-examples-djvu-ConvertDjvuToPdf-ConvertDjvuToPdf.java" >}}

## Convert Specific DjVu Pages to Multi-Frame Raster Images

Aspose.Imaging for Java 3.0.0 has exposed a new class IntRange that can be used to specify a range that in turn can be passed to an instance of DjvuMultiPageOptions for the conversion of specific range of DjVu pages to TIFF or GIF.

The following piece of code uses the IntRange & DjvuMultiPageOptions classes to render a subset of DjVu pages to TIFF.

{{< gist aspose-imaging 8c9bd83e0d07145ba0c1 "Examples-src-main-java-com-aspose-imaging-examples-djvu-ConvertRangeOfDjVuPages-ConvertRangeOfDjVuPages.java" >}}

## Convert Specific Portion of DjVu Page to Image using Java

Another overload constructor of the DjvuMultiPageOptions class can accept an integer value as well as an instance of Rectangle to [export a specific portion of DjVu page to raster image format][6].

The following piece of code creates an instance of a Rectangle to specify the location and size of the desired area to be exported in PNG format.

{{< gist aspose-imaging 8c9bd83e0d07145ba0c1 "Examples-src-main-java-com-aspose-imaging-examples-djvu-ConvertSpecificPortionOfDjVuPage-ConvertSpecificPortionOfDjVuPage.java" >}}

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][7] for a chat.




[1]: https://downloads.aspose.com/imaging/java
[2]: https://docs.aspose.com/display/imagingjava/Migrating+from+Earlier+Versions+of+Aspose.Imaging
[3]: https://docs.aspose.com/display/imagingjava/Migrating+from+Earlier+Versions+of+Aspose.Imaging
[4]: https://docs.aspose.com/display/imagingjava/Manipulating+DjVu+Formats#ManipulatingDjVuFormats-ConvertingDjVutoTIFFFormat
[5]: https://docs.aspose.com/display/imagingjava/Manipulating+DjVu+Formats#ManipulatingDjVuFormats-ConvertingDjVutoPDFFormat
[6]: https://docs.aspose.com/display/imagingjava/Manipulating+DjVu+Formats#ManipulatingDjVuFormats-ConvertingSpecificPortionofDjVuPage
[7]: https://downloads.aspose.com/imaging/java




