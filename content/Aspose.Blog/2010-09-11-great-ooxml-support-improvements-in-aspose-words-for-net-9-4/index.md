---
title: 'Great OOXML improvements in Aspose.Words for .NET 9.4'
date: Sat, 11 Sep 2010 02:58:00 +0000
draft: false
url: /2010/09/11/great-ooxml-support-improvements-in-aspose-words-for-net-9-4/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Lots of customers have been waiting to get their hands on Aspose.Words that does not lose DrawingML and Structured Document Tags (SDT, content controls) when processing DOCX documents.

Finally, it is here. The release page with full details is here [http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/entry258045.aspx][1]

I can only add that in this release you can only expect DrawingML and SDT to be preserved during DOCX open/save and also during document assembly (copying nodes between documents, joining documents together etc). You will be able to see and access these new node classes in the Aspose.Words document object model, but apart from copying and removing you will not be able to do anything with them yet.

We plan to extend our support for DrawingML and SDTs to RTF, we also plan to provide more public methods and properties so you can create SDTs for example and also access their properties. Let us know what do you want to be able to do programmatically with DrawingML and SDTs.

BTW our work to render DrawingML shapes, charts and diagrams to PDF and XPS is underway.




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/entry258045.aspx




