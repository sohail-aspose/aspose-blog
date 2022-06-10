---
title: 'Performance Improvements and Other Fixes in Aspose.Words for .NET 6.2.0'
date: Tue, 24 Feb 2009 00:44:00 +0000
draft: false
url: /2009/02/24/performance-improvements-and-other-fixes-in-aspose-words-for-net-6-2-0/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Hi,

We've just released Aspose.Words for .NET 6.2.0 and I would like to describe some of the exciting changes we've done.

## Performance Improvements in the Rendering Engine

Thanks to users who've been testing (should I say stress testing) our product we've been able to track down and fix some sore spots in our rendering and page layout code.

One issue was causing memory not to be released soon enough after rendering. The fix makes sure all memory used during document rendering is now released immediately and can be garbage collected.

Another issue was causing non-linear increase in document processing time compared to the document size. Now, a document containing 10,000 paragraphs will take exactly twice as long to process as a document with 5,000 paragraphs. With this fix, you will notice that 100+ pages documents are now processing significantly faster than before.

OK, what's the performance now? _Roughly, 10 pages per second._

Tested on a 3GHz, 2Gb RAM machine you can expect to convert a 100 pages document to PDF in around 10 seconds.

## Other Changes

There are about 30 other important improvements included in this release. They include better conversion of WMF/EMF metafiles with clip regions to PDF, some new shapes in OpenDocument import/export supported, improvements to CSS import in HTML and many others.

Check out for yourself by downloading from [https://downloads.aspose.com/words][1]




[1]: https://downloads.aspose.com/words




