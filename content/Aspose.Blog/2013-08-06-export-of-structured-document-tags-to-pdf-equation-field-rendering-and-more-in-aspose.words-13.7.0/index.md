---
title: 'Export Structured Document Tags to PDF and Render Equation Field using C# and Java'
date: Tue, 06 Aug 2013 10:15:11 +0000
draft: false
url: /2013/08/06/export-of-structured-document-tags-to-pdf-equation-field-rendering-and-more-in-aspose.words-13.7.0/
author: Adam Skelton
summary: ''
tags: ['EQ field', 'Structured Document Tag', 'content control', 'form field']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose.words-logo2.jpg" alt="">}}


We are pleased to announce the monthly release of Aspose.Words for .NET and Java 13.7.0. Our team has been hard at work and this release adds more than 138 useful improvements to the Aspose.Words library.

You can download the latest release of Aspose.Words from the following links:

*   [Aspose.Words for .NET 13.7.0][1]
*   [Aspose.Words for Java 13.7.0][2]

Here is a look at a few of the biggest features in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

## Export of Structured Document Tags as Editable PDF Form Fields

Structured document tags (also known as content controls) are a feature found in OOXML documents that provide dynamic UI controls to Word documents, such as adding fillable fields that can also be linked to document properties or custom data found inside the document. There are also special kinds of content controls, for example for displaying a drop-down list of choices.



{{< figure align=center src="images/StructuredDocumentTag.png" alt="A Microsoft Word Structured Document Tag" caption="A structured document tag in a Microsoft Word document">}}


Aspose.Words can now export structured document tags to PDF as editable form fields, which provides the opportunity to use these controls in your templates that are destined to be fillable and to also to provide a richer user experience for the end user.

Simply set **PdfSaveOptions.PreserveFormFields** to true when saving to PDF with custom options to preserve both legacy form fields and structured document tags in the output PDF document.

## Rendering of Mathematical Equation (EQ) Field Introduced

An EQ field is one of the several ways to insert a mathematical formula into a word document.  In previous versions of Aspose.Words this field would be partially rendered or skipped altogether when saving to fixed-page formats such as PDF, XPS or image.

With this release of Aspose.Words EQ fields are now rendered correctly with high fidelity. This means they look just as they appear in the output document as they do in the source Microsoft Word document.



{{< figure align=center src="images/EQ-Field.gif" alt="An EQ Field inside a Microsoft Word Document" caption="A side by side look at the visual representation of an EQ field and the field code which determines the equation’s appearance">}}





[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java




