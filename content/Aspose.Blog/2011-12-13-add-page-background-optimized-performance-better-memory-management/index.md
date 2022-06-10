---
title: 'Add Page Background, Optimized Performance, Better Memory Management'
date: Tue, 13 Dec 2011 08:23:23 +0000
draft: false
url: /2011/12/13/add-page-background-optimized-performance-better-memory-management/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.Total Product Family', 'Aspose.PDF Product Family']
---

![Aspose.Pdf icon][1]

We are pleased to announce the release of Aspose.Pdf for .NET 6.5.0. This release  includes some great new features such as setting background color of pages in PDF documents, determining which pages in a PDF document has background color set and support for attaching MP3 files. This release also improves the product's performance when converting PDF files into XPS/TIFF format and extracting text and images from PDF. Aspose.Pdf for .NET 6.5 also includes support for transforming PDF files into HTML and other supported formats. We've also improved the file concatenation features.

## Pass Documents from Class to Class without Saving

We have introduced a mechanism where you can use the single PDF document and pass it to various class objects present under Aspose.Pdf.Facades, without having to repeatedly save and open it. To facilitate this, we have locally added the Document property for almost all facades and extended them with new constructor. However, please note that not all facades work with Document directly.

For example PdfFileInfo only saves changes on invoking methods (SaveNewInfoWithXmp, SaveNewInfo) so has not been extended with the Document property. Document property can be used to access an inner document which is changed by Facade and then we can pass this Document object as an argument to another facade constructor in order to continue editing the same PDF document.

Please have a look at the code snippet below: it shows how PdfContentEditor and PdfAnnotationEditor can work in conjunction.

```
\[C#\] 
PdfContentEditor contentEditor= new PdfContentEditor();
contentEditor.BindPdf("input.pdf");
contentEditor.CreateText(newSystem.Drawing.Rectangle(100,100, 50, 50), 
              "Mine", "Some comment", false,"Comment", 1);

PdfAnnotationEditor annotationEditor= 
              new PdfAnnotationEditor(contentEditor.Document);
annotationEditor.ModifyAnnotationsAuthor(1,1, "Mine","Yours");
annotationEditor.Save(“UpdatedAnnotation.pdf”)
```

## Changes to the PdfConverter Class

We have made following changes to PdfConverter class:

1.  **PdfConverter** property changes: The Resolution property type has changed from int to Resolution. It now allows you to set horizontal and vertical resolution independently.
2.  PdfConverter methods changes: The GetNextImage methods now accepts width and height instead of resolutionX and resolution.
3.  New PdfConverter methods added:
    *   SaveAsTIFFClassF(string outputFile)
    *   SaveAsTIFFClassF(Stream outputStream)
    *   SaveAsTIFF(string outputFile, TiffSettings settings)
    *   SaveAsTIFF(Stream outputStream, TiffSettings settings)
    *   GetNextImage(string outputFile, ImageFormat format, int imageWidth, int imageHeight)
    *   GetNextImage(Stream outputStream, ImageFormat format, int imageWidth, int imageHeight)
    *   GetNextImage(Stream outputStream, ImageFormat format, int quality)
    *   GetNextImage(string outputFile, ImageFormat format, int quality)
4.  New TiffDevice actors added:
    *   TiffDevice(int width, int height, Resolution resolution, TiffSettings settings)
    *   TiffDevice(int width, int height, Resolution resolution)
    *   TiffDevice(int width, int height, TiffSettings settings)
    *   TiffDevice(int width, int height)
5.  New TiffDevice properties added
    *   int Width
    *   int Height

Please visit the following link to download the latest release version of [Aspose.Pdf for .NET 6.5.0][2].




[1]: http://www.aspose.com/Images/aspose.pdf-logo2.jpg
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.pdf-for-.net/entry348420.aspx




