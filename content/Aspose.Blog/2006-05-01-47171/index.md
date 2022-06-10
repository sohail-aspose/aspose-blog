---
title: 'Aspose.Words 3.6 Released'
date: Mon, 01 May 2006 15:05:00 +0000
draft: false
url: /2006/05/01/47171/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

**New Features**

*   Added a lot of new code examples to the API. Both in C# and VB.NET. The work on code examples continues, we will eventually have examples for all members.
*   Added a new demo project DocumentExplorer. Not only it provides more example code, but it is a useful tool on its own. You can open a document in HTML or DOC format, explore the nodes of the document object model and save the document as DOC, HTML or PDF.
*   Added IMailMergeDataSource interface. Now a mail merge is possible from any custom data source.
*   Added more resiliency for opening documents that are not entirely valid.
*   Added more resiliency against creating invalid documents (empty cells, first cell merged to previous, table at end of section).
*   DocumentBuilder InsertXXX methods return the document nodes that they create.

**Fixes**

*   Imported table is treated by MS Word as 'corrupted' in the resulting document.
*   A document with some textboxes crashes MS Word on open.
*   A metafile throws value is too large for Int16.
*   TextColumns.SetCount to a smaller than current value did not work.
*   Error opening encrypted document with table with more than 9 collumns.
*   Exception when saving a document as HTML with a scaled image of 1x1 pixel in it.
*   Saving to PDF or HTML throws exception when a table contains no rows.
*   An extra table row gets visible when saving as HTML and then loading back into Aspose.Words.
*   Roman Numerals are not exported to PDF correctly.
*   Heading numbering is incorrect when saved in PDF.
*   Some links in table of contents did not work in PDF.
*   InsertHtml sometimes does not stop marking paragraphs as list members.







