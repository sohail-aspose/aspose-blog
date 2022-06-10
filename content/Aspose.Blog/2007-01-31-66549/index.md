---
title: 'Aspose.Words for .NET 4.1 Released'
date: Wed, 31 Jan 2007 23:11:00 +0000
draft: false
url: /2007/01/31/66549/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

This release of [Aspose.Words][1] contains a single important new feature:

*   **RTF Import**

Support for RTF in Aspose.Words was requested by many customers and for very long time. We are proud to announce that RTF in Aspose.Words is now fully supported. We released RTF export a few months ago in Aspose.Words 4.0 and now we complete the job by adding RTF import.

Aspose.Words was initially developed to generate, open, modify, save and convert primarily Microsoft Word DOC documents, but it later grew to include support for other Microsoft Word and non-Microsoft Word formats.

Here is a brief summary of the file formats that Aspose.Words for .NET now supports:

*   _DOC read and write, Microsoft Word versions 97 to 2007._
*   _RTF read and write according to the Rich Text Format 1.8 specification._
*   _WordprocessingML write (read will soon be ready) as per Microsoft Word 2003._
*   _DOCX - Open XML, Word 2007, read and write planned for Q2 2007._
*   HTML/XHTML read and write with inline CSS. XHTML is 1.0 Transitional.
*   TXT plain text write (read will soon be ready).
*   PDF (requires Aspose.Pdf).

The formats in _italics_ above are Microsoft Word formats and Aspose.Words document model is explicitly designed to support Microsoft Word documents. Therefore, an unprecedented, high level of accuracy conversions between these formats is supported by Aspose.Words. We call it _high-fidelity_ conversion and you probably will not find the same level of support for these file formats in any other software, except Microsoft Word itself.

Here is a summary of the file formats supported by Aspose.Words for Java:

*   DOC read and write, Microsoft Word versions 97 to 2007.
*   HTML/XHTML write with inline CSS. XHTML is 1.0 Transitional.

All other formats that are supported by Aspose.Words for .NET will be available in Aspose.Words for Java too.

**Other Fixes and Improvements in Aspose.Words for .NET 4.1**

*   1452 - Add support for Roman page numbers per section. PDF export.
*   1442 - Aspose.Words throws NullReferenceException when saving a particular file in evaluation mode.
*   1420 - Sequential floating tables are put into one table in the model.
*   1319 - Add the possibility to turn tracking changes on and off. Added the Document.TrackRevisions property.
*   Added a new exception class: UnsupportedFileFormatException is thrown by the Document constructor when a document format is not recognized or not supported.
*   Added a new exception class: FileCorruptedException is thrown by the Document constructor when the document appears to be corrupted and cannot be loaded.

To download Aspose.Words: http://www.aspose.com/Downloads/Aspose.Words/Default.aspx




[1]: /Products/Aspose.Words/Default.aspx




