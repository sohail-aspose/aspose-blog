---
title: 'Parse PostScript and Convert PDF to Image using C#'
date: Wed, 09 Feb 2011 23:56:00 +0000
draft: false
url: /2011/02/09/parse-postscript-and-convert-pdf-to-image-using-csharp/
author: Shahzad Latif
summary: ''
tags: []
categories: ['Aspose.PDF Product Family']
---

[Aspose.Pdf.Kit for .NET][1] 5.3.0 has been released with some improvements. During the development of this version, the major focus areas were PDF to image conversion with improved text rendering, better OpenType font support during image conversion and importing data from XML to PDF form.

In certain scenarios, while converting PDF to images, some of the characters were missing or most of the text was not rendered at all. However, with the improved OpenType font support and enhanced text rendering Aspose.Pdf.Kit for .NET is able to produce high quality images. You can also save a particular range of the PDF pages as a single TIFF image with this latest version. As SaveAsTIFF is the only method which currently allows you to save the output image with TiffSettings including CompressionType, if you are interested to save PDF pages as individual images with the above settings, you may use SaveAsTIFF method and set StartPage and EndPage values to the current page. This way you can navigate through all the PDF pages and save the individual page as TIFF image with TiffSettings and CompressionType. In addition to that, we have enhanced ImportXml method to import multiple rows into a PDF form.

You can see the complete list of changes and download the latest version from the [Aspose.Pdf.Kit for .NET download section][2].




[1]: https://products.aspose.com/pdf/net
[2]: https://downloads.aspose.com/pdf/net




