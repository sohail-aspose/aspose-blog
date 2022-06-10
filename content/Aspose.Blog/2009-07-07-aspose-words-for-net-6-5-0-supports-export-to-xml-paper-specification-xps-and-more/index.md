---
title: 'Aspose.Words for .NET 6.5.0 supports export to XML Paper Specification (XPS) and more'
date: Tue, 07 Jul 2009 18:52:00 +0000
draft: false
url: /2009/07/07/aspose-words-for-net-6-5-0-supports-export-to-xml-paper-specification-xps-and-more/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

We have recently released Aspose.Words for .NET 6.5.0 with great new features and fixes. You can read the usual release details [here][1], while in this post I want to highlight some of what we've done.

**Export to XPS (XML Paper Specification)**

Aspose.Words for .NET now supports converting any document to XPS!

Microsoft XML Paper Specification (XPS) is a fixed-layout document format designed to provide device-independent document appearance.

Aspose.Words uses the same high-fidelity page layout and rendering engine for output to all its fixed-layout formats: PDF, XPS, thumbnails (images of pages) and printing. This means that XPS documents produced by Aspose.Words appear equally good to PDF.

You can read more and see screenshots of Aspose.Words export to XPS here.

**Improved Support for Table Styles and Conditional Formatting**

Before today's release, support for Table Styles in Aspose.Words was limited. Only if you opened a DOC file and then saved again as DOC, table styles were preserved.

Table Styles are used by our customers more frequently and now Aspose.Words for .NET provides better support for Table Styles. Here is what's supported:

*   DOC to DOC conversion - table styles are preserved.
*   DOCX/WordML to DOCX/WordML conversion - table styles are preserved.
*   DOCX/WordML to any other format (including rendering and preinting) - table styles are converted to direct formatting to preserve the look of the tables.

What it means, is that in many cases DOCX or WordML conversions to PDF, XPS, HTML or printing will result in more fidelity to the original, much better looking output documents.

It is important to note that Aspose.Words now supports all Conditional Table Style Formatting as per the OOXML specification. If you have a document with table styles that specify alternating row or column colors, first/last row, first/last column formatting and so on, all this formatting will be faitfully preserved during conversions.

We continue to work to provide even more support for table styles. In the future versions we will add table styles to the public API and we will preserve table styles during conversions between DOC and RTF (without expanding table styles to direct formatting).

**Improved Support for Themes**

Before today's release, Aspose.Words did not support Themes. Themes were introduced in Microsoft Word 2007 documents. Themes allows to apply font and color formatting in a document "centrally", overriding the normal style-based formatting. Themes can occur in OOXML, DOC and RTF documents. Aspose.Words used to ignore Themes completely and that affected conversion results. For example, conversion from DOCX to DOC often resulted in font Calibri (applied by the default theme) converted to Times New Roman.

Now Apsose.Words for .NET supports Themes in the following ways:

*   DOCX to DOCX conversion - Themes are completely preserved in the document.
*   DOCX to other formats - fonts specified in Themes is converted into direct formatting.

This improvement will solve many outstanding support requests, but we continue our work to support Themes fully. We will include themes in the public API, support theme colors, tints, shading in all formats.

**Loading of Encrypted OOXML Documents**

Aspose.Words for .NET now supports loading of encrypted OOXML documents. You can see there is a new **LoadFormat.OoxmlEncrypted** value returned by the **Document.DetectFileFormat** method.

I can also mention there is one more new value **LoadFormat.DocEncrypted** that allows you to programmatically distinguish a DOC file that requires a password to open from a file that does not.

**Fixes to Many Crashes**

Our new "motto" is to make Aspose.Words completely crash free. This includes both Aspose.Words refusing to load some documents by throwing an exception and the very rare cases of Microsoft Word refusing to load documents produced by Aspose.Words.

We have addressed all such issues reported by our customers so far and fixed them all! We have also randomly selected and downloaded many documents in different formats from the Google search engine. For this release, we have tested Aspose.Words and proved it is crash free on about 30,000 documents.

**Reorganized Documentation**

We have also reorganized Aspose.Words documentation to make it easier to use and also added some new topics. But I will write more about this in my next post.




[1]: http://www.aspose.com/community/files/51/file-format-components/aspose.words-for-.net-and-java/entry186045.aspx




