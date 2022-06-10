---
title: 'Structured Document Tags (Content Controls) are confirmed in the upcoming Aspose.Words for .NET 9.4'
date: Thu, 02 Sep 2010 01:10:00 +0000
draft: false
url: /2010/09/02/structured-document-tags-content-controls-are-confirmed-in-the-upcoming-aspose-words-for-net-9-4/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Aspose.Words for .NET 9.4. is our next release that is likely to be available early next week.

Another great feature that I can confirm is making into this release is support for Structured Document Tags (Content Controls) in your OOXML documents.

Earlier versions of Aspose.Words would just lose Content Controls if you open/save a DOCX document.

The upcoming version fully preserves Content Controls in your documents during DOCX open/save operations.

There will be a new public class StructuredDocumentTag (derives from CompositeNode) so you will be able to "see" SDTs programmatically. You will be able to remove, clone and move them to another place/document. In this release it will not be possible to create SDTs or access their properties, but we will expose more of the SDT in the public API in the next few versions. We also have plans to support SDTs in RTF and DOCX to/from RTF conversions in the future.

Another great news is that while working on supporting Content Controls we have figured out a good way (and laid foundations) to support Custom XML Markup in OOXML documents in Aspose.Words. Support for Custom XML Markup is not going to be available just yet in 9.4, but it will follow very shortly.








