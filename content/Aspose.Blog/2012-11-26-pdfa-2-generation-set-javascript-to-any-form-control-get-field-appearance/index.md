---
title: 'Generate PDF/A-2 and Set JavaScript to any Form Control in PDF using C#'
date: Mon, 26 Nov 2012 08:41:06 +0000
draft: false
url: /2012/11/26/pdfa-2-generation-set-javascript-to-any-form-control-get-field-appearance/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---

We're pleased to announce the release of [Aspose.PDF for .NET 7.5.0][1]. This new product release supports the feature to generate PDF/A-2 compliant documents and even it offers the feature to create PDF/A-2 files with digital signatures. Earlier to this release version, we only had the support to add JavaScript to pushbutton control but with the release of this version, now you can add JavaScript to any control i.e. CheckBox, over PDF form.

```
FormEditor formEditor = new FormEditor(); 
formEditor.BindPdf("d:/pdftest/HelloWorld (1).pdf"); 
//set JavaScript 
formEditor.SetFieldScript("CB1", "this.getField('CB1').display = display.hidden;");
//set JavaScript 
formEditor.SetFieldScript("bt1", "this.getField('bt1').display = display.hidden;"); 
//save update document 
formEditor.Save("d:/pdftest/CheckBox_javaScript_34248.pdf"); 
```

Recently we also have added the support to retrieve form field appearance by using the following simple code snippet.

```
Aspose.Pdf.Facades.FormEditor form = new Aspose.Pdf.Facades.FormEditor();
form.BindPdf("d:/pdftest/FormField.pdf");
Console.WriteLine(form.GetFieldAppearance("textfield"));
```

We have also improved the product performance while concatenating large number of PDF files i.e. 89 PDF files of 2.1 MB each, took 52 seconds over Intel Core 2 Duo 3.16 Ghz with 4 GB of RAM running Windows 7 X64 Enterprise. PDF to Image especially PDF to TIFF conversion has been improved in terms of performance as well as resultant file size. Product has also been improved to read/manipulate various PDF formats with different complexity and structure. Numerous bugs reported in earlier release versions are also fixed.

Please visit the following link for further details on what's new & fixed in [Aspose.PDF for .NET 7.5.0][2].




[1]: https://products.aspose.com/pdf/net
[2]: https://downloads.aspose.com/pdf/net




