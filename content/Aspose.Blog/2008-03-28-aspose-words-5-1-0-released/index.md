---
title: 'Aspose.Words 5.1.0 Released'
date: Fri, 28 Mar 2008 02:45:00 +0000
draft: false
url: /2008/03/28/aspose-words-5-1-0-released/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

There is Aspose.Words 5.1.0 available in downloads [http://www.aspose.com/community/files/51/file-format-components/aspose.words/entry119442.aspx][1].

Here I just wanted to elaborate more on what we've done:

**Improvements to DrawingML Import (in OOXML)**

When we started implementation of Office Open XML export and import features in Aspose.Words about a year ago, Microsoft Word 2007 was storing images and shapes in the VML format inside a DOCX document. All information we could find at that time was saying that DrawingML although part of the Office Open XML specification is only used by Power Point in Office 2007. Apparently we were mistaken.

Now after a year of hard work we have a good level of support (as you can see from our conformance spreadsheet) for OOXML import and export since Aspose.Words 5.0.0. But sometime during this year Microsoft Word 2007 "started" to store images and shapes in the DrawingML format and that took us by surprise. We completely missed out on DrawingML and hence many customers reported images missing in their documents after DOCX open/save in Aspose.Words.

When you save a document in Word 2007 you can control whether VML or DrawingML is used by checking the "Maintain compatibility with Word 97-2003" in the Save As dialog box. If a document was saved with this option turned off, all images in the document will be stored as DrawingML.

Straight after 5.0 release we started urgently working on DrawingML support. This 5.1 release is a first iteration. Import of inline images stored as DrawingML is now supported.

**Improvements to ODT (OpenDocument) Export**

This is another iteration of features in ODT export. Export of formatting for images, paragraphs, text, sections and tables has been improved in many places. We still continue to actively work on ODT.

**Exporting CSS to a Stylesheet**

A useful new option that was requested by many customer allows to export CSS to a stylesheet (embedded or external file) when exporting a document to HTML.

`

Document doc = new Document("MyFile.doc");

doc.SaveOptions.HtmlExportCssStyleSheetType = CssStyleSheetType.External;

doc.SaveOptions.HtmlExportCssStyleSheetFileName = "myfile_styles.css";

doc.Save("MyFile.html");

`

**Resolved Problems on 64bit Windows**

We've been plagued by occasional customer reports about Aspose.Words failures on Windows Server 2003 64-bit over a period of several months.

The problem was traced down to a setting in the obfuscation tool we use. Some Aspose.Words builds would run on 64-bit successfully, but some will fail, mostly when you attempt to open a document with a memory access exception. The difficulty was that some builds will work and some not.

We hope that we have finally resolved this issue now.




[1]: http://www.aspose.com/community/files/51/file-format-components/aspose.words/entry119442.aspx




