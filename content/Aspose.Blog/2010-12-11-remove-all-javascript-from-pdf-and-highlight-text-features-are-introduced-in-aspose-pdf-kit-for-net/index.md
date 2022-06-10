---
title: 'Remove All JavaScript From PDF and Highlight Text Features are Introduced in Aspose.Pdf.Kit for .NET.'
date: Sat, 11 Dec 2010 00:59:00 +0000
draft: false
url: /2010/12/11/remove-all-javascript-from-pdf-and-highlight-text-features-are-introduced-in-aspose-pdf-kit-for-net/
author: Shahzad Latif
summary: ''
tags: []
categories: ['Aspose.PDF Product Family']
---

Aspose.Pdf.Kit for .NET 5.1.0 has been released with some new features and improvements. We have introduced a new feature to remove all the JavaScript from the PDF file. This can be achieved using Strip method of PdfJavaScriptStripper class. The Strip method returns true in case any scripts were found and removed. You can use the following code snippet:

```
//create PdfJavaScriptStripper object
PdfJavaScriptStripper javascriptStripper = new PdfJavaScriptStripper();
//remove all javaScript from PDF file
bool result = javascriptStripper.Strip(“input.pdf”, “output.pdf”);
```

We have also introduced a feature to highlight text in an existing PDF file. This feature can be used in two ways: you can either simply highlight the text using any color or hide a particular string by using black color. We have used the existing ReplaceText method to introduce this new functionality.

The performance of PdfConverter and PdfFileEditor classes has been enhanced. In addition to that, we have improved concatenate, import XML, PDF to image conversion and PDF printing features. Text replacement feature has also been enhanced to work properly with non-English languages like Norwegian, Russian and Swedish.

You can see the complete list of changes and download the latest version from the [Aspose.Pdf.Kit for .NET download section][1].




[1]: https://downloads.aspose.com/pdf




