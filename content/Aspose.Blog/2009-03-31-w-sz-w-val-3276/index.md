---
title: 'w:sz w:val=&quot;3276&quot;'
date: Tue, 31 Mar 2009 22:12:00 +0000
draft: false
url: /2009/03/31/w-sz-w-val-3276/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

<w:style w:type\="paragraph" w:default\="1" w:styleId\="Normal">

<w:name  w:val\="Normal" />

<w:qFormat  />

<w:rsid  w:val\="00067620" />

<w:rPr\>

<w:rFonts  w:cs\="Times New Roman" />

**<****w:sz**  **w:val****\="****3276****" />**

**<****w:szCs**  **w:val****\="****3276****" />**

</w:rPr\>

</w:style\>

The above value means the font size is 3276/2 = 1638pt = 22.75inches!

That value is reliably written by Microsoft Word 2007 into every .dotx file that has glossary (building block) entries.

Apparently, this is some sort of a "magic number" that probably means "use font size from the main document" or something like that.

This value is not in the ECMA 376 or the OOXML standard.

This issue cropped up when we were working on implementing support for the Glossary document part in Aspose.Words. Soon, Aspose.Words will support documents with Glossary (Building Blocks) and you will be able to create/modify and also insert building blocks into your documents using Aspose.Words.

I guess this must go to the list of reasons why use Aspose.Words instead of OpenXML SDK.








