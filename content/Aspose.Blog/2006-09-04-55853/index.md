---
title: 'Aspose.Words for .NET 4.0.0 Beta Released'
date: Mon, 04 Sep 2006 12:53:00 +0000
draft: false
url: /2006/09/04/55853/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

We listened to you and now Aspose.Words is almost ready for a next big step forward in the Word document processing technology.

**Important New Features**

· Full support for drawing objects and textboxes in documents.

· New public API for drawing objects in the Aspose.Words.Drawing namespace.

· High-Fidelity export to Rich Text Format 1.8 (RTF).

· High-Fidelity export to WordprocessingML (WordML).

· Export to XHTML 1.0 Transitional.

· Improved HTML import.

· Separate Aspose.Words assemblies provided for .NET 1.x and .NET 2.0.

· [Updated demo projects][1] to showcase export to new formats.

Please note that some API changes are breaking and you might have to modify your existing code in order to compile. The breaking changes are due to the introduction of the new drawing objects API.

**Why Beta?**

To give you a better chance to comment on the new exciting features that we added. In the meantime we will do final touches and update examples and documentation. This Beta will become a proper release within a month.

If you are in the process of buying the current version of Aspose.Words, don’t hold off because a subscription gives free upgrades for a year and you automatically will have access to the new version.

**Fixes**

Most of the issues in this list were caused by known limitations of drawing objects and HTML import.

**HTML Import/Export**

· 1201 - Colspans and rowspans appear corrupted when used together

· 1178 - Cell width is lost during HTML import

· 1171 - Meta and Img fields are not closed during HTML export.

· 1151 - Allow setting resolution when exporting metafiles to HTML and PDF

· 1129 - InsertHtml with nested table cause problems in the resulting document.

· 1099 - HTML table rendered incorrectly during import.

· 1097 - Font color is lost during html import.

· 1096 - Support different measurement units in HTML import.

· 1093 - Document fails with 'Unexpected measurement units' exception when opened in Aspose.Words.

· 996 - Nested tables are imported incorrectly

· 731 - Export alternative text specified on an image to HTML

**DOC Import/Export**

· 1197 - Document throws exception 'Specified argument was out of the range of valid values.' when opened in Aspose.Words.

· 1138 - Document cause exception when saved in Aspose.Words.

· 1137 - Document crashes MS Word after being opened/saved by Aspose.Words

· 1134 - Documents fail with 'System.ArgumentException: duplicate' when opened in Aspose.Words.

· 1101 - Openning document fails with 'Cannot find an entry for the specified position in the PLCF' exception.

· 1057 - Documents with grouped images combined using Aspose.Words produce the document that crashes MS Word.

· 867 - Document with textboxes is displayed incorrectly in Word2000

· 714 - MS Word crashes on document with group shapes

· 696 - Z order of shapes is not preserved when exporting to PDF.

· 689 - Executing MailMerge produces faulty document

**PDF Export**

· 1071 - A character is lost from the hyperlink text in PDF

· 1070 - Russian characters in the hyperlink are lost in PDF

· 1030 - Text watermarks are lost during pdf conversion.

· 963 - Framed text is positioned incorrectly

· 895 - Aspose.Pdf skips a paragraph in a table

· 815 - Line spacing issue in PDF

· 766 - Adjacent runs with identical formatting are dispplayed incorrectly when converted to PDF

· 751 - Fixed row height is exported incorrectly

**Other**

· 1166 - MalMerge.Execute(string\[\], object\[\]) is case sensitive

· 1163 - Disallow users setting document properties to null

· 1153 - Make RowFormat.CellSpacing property public

· 1133 - Setting Borders.LineWidth to value greater than 0 without explicit setting of Borders.LineStyle to value other than LineStyle...

· 1126 - Document template cause strange behavior in MS Word 2003.

· 1123 - Problems when resaving .dot files as .doc with Aspose.Words

· 1117 - Document is saved differently in VS2005 vs VS2003

· 1116 - Implement Range.Bookmarks.Clear() method

· 1081 - Add possibility to set alternative text for shapes.

· 802 - Fix calculated cell width for horizontally merged cells

· 642 - Implement a way of linking images instead of embedding

· 598 - Add setter for Shape.ImageBytes

· 570 - Placing merge fields inside textboxes makes the fields move out of place

· 543 - Multiple textboxes in a group shape are not supported.

· 350 - Add horizontal line support

· 287 - Image shape contains text and Unsupported image format exceptions

· 272 - Textboxes in organizational chart or in a diagram cause index out of range exception.

· 253 - Many Escher and textbox problems in one document

· 135 - Insert textboxes at specified positions

· 93 - Inline images are in the document, but not visible in Word 97.

· 92 - Inline textbox placement is incorrect when opened in Word 97

· 14 - Rework Escher so Z-order, spids, regrouping and connectors all work nicely




[1]: /Products/Aspose.Words/Demos/



