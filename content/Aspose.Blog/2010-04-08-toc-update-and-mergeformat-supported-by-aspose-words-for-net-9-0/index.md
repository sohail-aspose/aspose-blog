---
title: 'TOC Update and MERGEFORMAT Supported by Aspose.Words for .NET 9.0'
date: Thu, 08 Apr 2010 13:43:00 +0000
draft: false
url: /2010/04/08/toc-update-and-mergeformat-supported-by-aspose-words-for-net-9-0/
author: DmitryV
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

We are happy to announce that a top priority feature (40+ requests logged in our defect database) is now implemented in the recently released Aspose.Words for .NET 9.0. TOC fields are now updated along with others!

TOC stands for Table of Contents and is represented by the TOC field in a Microsoft Word document. TOC entries may be built from:

*   Paragraphs having the HeadingN style where N is the level of the heading
*   Paragraphs having special styles specified in the TOC field code
*   Paragraphs having outline level other than body text
*   TC (TOC entry) fields

Earlier you had to update TOC manually by pressing F9 in Microsoft Word, but now Aspose.Words takes care of that. Of course, Aspose.Words does not use Microsoft Word Automation and implements the complete field update itself. Just two simple lines of code do the magic:

```
Document doc = new Document("mydoc.docx");
doc.UpdateFields();
doc.UpdatePageLayout();
```

Why two-stage update? **Document.UpdateFields()** rebuilds and updates field structure while **Document.UpdatePageLayout()** recalculates and inserts actual page numbers. Voila:

Most of the field switches are supported, paragraph numbering is preserved, and in whole the TOC field looks exactly as it was updated by Microsoft Word.

Another great feature added in Aspose.Words for .NET 9.0 is the support for the MERGEFORMAT field format option. MERGEFORMAT is widely used in Microsoft Word documents. It instructs the field to retain the formatting and structure of its value when the field is being updated. Imagine an IF field whose _TrueText_ and _FalseText_ look as tricky as in the screenshot:

And the current value looks like the following:

Now after you update the fields in the document by calling

```
doc.UpdateFields();
```

the value gets updated, but its formatting and structure remain the same:

To download Aspose.Words for .NET 9.0 that introduces these and many other great features, please visit [https://downloads.aspose.com/words/net][1].




[1]: https://downloads.aspose.com/words/net




