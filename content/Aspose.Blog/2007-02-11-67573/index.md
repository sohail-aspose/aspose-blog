---
title: 'Rapid Text Format'
date: Sun, 11 Feb 2007 13:06:00 +0000
draft: false
url: /2007/02/11/67573/
author: DmitryV
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Please download the latest Aspose.Words 4.1.1 if you want to assess the result of the optimizations applied to RTF import within almost two weeks after release.

Let me boast a bit. Let's take our old fellow for the testing: a document named _Microsoft Office Word 2003 Rich Text Format (RTF) Specification_ converted to the format it describes, RTF. Why we commonly use it for testing our import/export modules is because it's well balanced for that purpose: it's large enough (~8 Mb RTF); it contains tons of tables and formatted text; it includes some pictures. Importing the document using Aspose.Words 4.1.1 shows the following results on my machine (P3.6 2Gb RAID0):

whereas Microsoft Word 2003 shows around 8 seconds for open and almost 3 seconds for saving the same document on the same machine!

As ever, this is sort of a challenge for us - whether we are able to gain even more precious seconds or their fractions thereby speeding up your document processing as well. I'm sure we are! I will keep you informed about our progress on this matter.

P.S. Happy forthcoming Valentine's Day!








