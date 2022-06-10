---
title: 'Convert PDF to TIFF using C#'
date: Thu, 01 Jul 2010 01:26:00 +0000
draft: false
url: /2010/07/01/convert-pdf-to-tiff-using-csharp/
author: Shahzad Latif
summary: ''
tags: []
categories: ['Aspose.PDF Product Family']
---

[Aspose.Pdf.Kit for .NET][1] 4.6.0 has been published. In this latest version, we have introduced some new features and improved many existing features. The main enhancements have been made in PdfViewer, PdfAnnotationEditor, PdfConverter, PdfFileEditor and PdfFileInfo classes.

We have improved font rendering mechanism which allows better PDF printing using PdfViewer class and enhanced PDF to image conversion using PdfConverter class. We have added support for a new image format; EMF is the new image format which is supported while converting PDF to images. Many new features have been added for PDF to TIFF conversion as well. You can set color depth, orientation and margins using ColorDepth and ShapeType enumerations and Margins class respectively. The respective properties have been introduced using TiffSettings class. You can specify any of these attributes and then pass the object of TiffSettings class to SaveAsTIFF method. You can also skip any blank PDF pages while converting to TIFF images using SkipBlankPages property of the TiffSettings class.

Our team has also worked on PDF printing and image conversion, so that you get proper and quality output. The enhanced font rendering allows the component to produce better quality text on print or image output. Concatenate and Append methods are also improved. In addition to that, we have tried to improve performance and memory utilization to let you enjoy better overall experience of the component.

You can see the complete list of changes and download the latest version from the [Aspose.Pdf.Kit for .NET download section][2].




[1]: https://products.aspose.com/pdf/net
[2]: https://downloads.aspose.com/pdf/net




