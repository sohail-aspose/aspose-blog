---
title: 'OpenType Fonts with PostScript Outlines in Aspose.Words'
date: Sun, 15 Aug 2010 00:10:00 +0000
draft: false
url: /2010/08/15/opentype-fonts-with-postscript-outlines-in-aspose-words/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

When rendering documents to PDF and XPS formats, Aspose.Words currently supports the following fonts:

*   TrueType Fonts
*   TrueType Font Collections
*   OpenType fonts with TrueType outlines

A number of customers have reported problems that Aspose.Words cannot render some of their documents to PDF and fails with errors like "cannot find the 'loca' table" or changes a font to Times New Roman or to MS Sans Serif.

We have traced many of these errors to a single problem - these documents use OpenType (OTF) fonts, but those fonts contain **PostScript** outlines.

I am happy to tell that Aspose.Words for .NET 9.4 that is coming soon will support rendering with OpenType fonts with PostScript outlines!

In this release the complete font will be embedded without subsetting (Aspose.Words by default subsets TrueType fonts to include only the used glyphs). But we will implement subsetting of fonts with PostScript outlines too in one of the next releases.








