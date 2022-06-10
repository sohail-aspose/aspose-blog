---
title: 'Improved PDF printing, set JavaScript as Page Action, Hide Stamps'
date: Thu, 07 Feb 2013 16:10:51 +0000
draft: false
url: /2013/02/07/print-text-as-text-not-image-javascript-as-page-action-hide-stamps/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---

![Aspose.Pdf icon][1]

It gives us an immense pleasure to introduce the latest release of [Aspose.Pdf for .NET 7.7.0][2]. This version has new and useful features such as rendering text as text rather than graphic objects when printing  documents. It makes the printing feature more viable and robust when it comes to the usage of the Document as well as PdfViewer classes. One of the new features regarding document conversion is rendering headers and footers as Microsoft Word headers and footers when converting PDFs to DOCs.

In this release , we also support many classes including Table, Row, Cell, MarginInfo, BorderInfo etc. in the Aspose.Pdf namespace which were earlier in the Aspose.Pdf.Generator namespace. These changes lets you add table objects to existing features. You can also add [a table into the header and footer sections of existing PDF files][3] . Prior to the release of Aspose.Pdf for .NET 7.7.0, we only supported adding JavaScript to document actions. With this release, you can add JavaScript against page actions. To accomplish this, we've implemented the PageActionCollection. This class has the following properties:

*   public PdfAction OnOpen
*   public PdfAction OnClose

```
Document doc = new Document(TestSettings.GetInputFile("PdfWithSeveralPages.pdf"));   
doc.Pages[5].Actions.OnOpen = new JavascriptAction("app.alert('open')");
doc.Pages[5].Actions.OnClose = new JavascriptAction("app.alert('close')"); 
doc.Save(TestSettings.GetOutputFile("34589.pdf"));
```

We have also introduced a feature for hiding a stamp object already present in a PDF. To fulfill this requirement, the following methods were added to the PdfContentEditor class:

*   HideStampById(int pageNumber, int stampId) - hides stamp by its ID
*   ShowStampById(int pageNumber, int stampId) - shows stamp which was hidden by previous call of HideStampById.

We have also made many improvements in terms of performance, XPS to PDF, HTML to PDF, PDF to image rendering, PDF concatenation and much more. Please visit the following link for further details on what's new & fixed in [Aspose.Pdf for .NET 7.7.0][4].




[1]: http://www.aspose.com/Images/aspose.pdf-logo2.jpg
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.pdf-for-.net/entry443335.aspx
[3]: http://www.aspose.com/community/forums/thread/443253/adding-table-in-pdf-footer.aspx
[4]: http://www.aspose.com/community/files/51/.net-components/aspose.pdf-for-.net/entry443335.aspx




