---
title: 'Improved PDF to Image Conversion and Specifying Custom Fonts Folder in Aspose.Pdf for .NET 7.9.0'
date: Sun, 14 Apr 2013 18:24:00 +0000
draft: false
url: /2013/04/14/improved-pdf-to-image-conversion-and-the-capability-to-specify-custom-fonts-folder/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', '.NET', 'Adobe Acrobat', 'customer font folder', 'floating box', 'product release', 'underline']
categories: ['Aspose.PDF Product Family']
---

![Aspose.Pdf icon][1]

Hello folks, I am about to share some words regarding new and exciting features in the latest release of [Aspose.Pdf for .NET 7.9.0][2]. In earlier release versions, we supported Table, Cell and Row classes under the Aspose.Pdf namespace. These provided the capability to create tables inside new and existing PDF files. Now I am pleased to share that we have added support for the FloatingBox class to the Aspose.Pdf namespace. Now you can add floating boxes when creating new documents as well as when working with existing PDF files.

## Custom Font Folder

We have also increased the fonts support and along with the capability to use pre-installed fonts from the Windows\\Font directory, you can also specify any other folder where custom fonts are present.

```
FontRepository.Sources.Add(new FolderFontSource("C:\\CustomFontStorage"));
```

## Underline

We have introduced the Underline property to the TextState class and now you can set text formatting to Underline (earlier versions only supported Bold and Italic).

```
 // Create documentation object
Document pdfDocument = new Document();
// Add age page to PDF document
pdfDocument.Pages.Add();
// Create TextBuilder for first page
TextBuilder tb = new TextBuilder(pdfDocument.Pages[1]);
// TextFragment with sample text
TextFragment fragment = new TextFragment("Test message");
// Set the font for TextFragment
fragment.TextState.Font = FontRepository.FindFont("Arial");
fragment.TextState.FontSize = 10;
// Set the formatting of text as Underline
fragment.TextState.Underline = true;
// Specify the position where TextFragment needs to be placed
fragment.Position = new Position(10, 800);
// Append TextFragment to PDF file
tb.AppendText(fragment);
// Save the PDF file
pdfDocument.Save("c:/pdftest/UnderLine.pdf"); 
```

Some enhancements regarding PDF to DOC and PDF to image conversion are also introduced. Please visit the following link for further details on what's new and fixed in [Aspose.Pdf for .NET 7.9.0][3].




[1]: http://www.aspose.com/Images/aspose.pdf-logo2.jpg
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.pdf-for-.net/entry457496.aspx
[3]: http://www.aspose.com/community/files/51/.net-components/aspose.pdf-for-.net/entry457496.aspx




