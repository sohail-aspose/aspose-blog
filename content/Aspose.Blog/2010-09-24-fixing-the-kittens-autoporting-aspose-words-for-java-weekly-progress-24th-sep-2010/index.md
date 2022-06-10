---
title: 'Fixing the Kittens: Autoporting Aspose.Words for Java Weekly Progress - 24th Sep 2010'
date: Fri, 24 Sep 2010 22:33:00 +0000
draft: false
url: /2010/09/24/fixing-the-kittens-autoporting-aspose-words-for-java-weekly-progress-24th-sep-2010/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

In my previous post I delivered no good news about when Aspose.Words for Java with PDF rendering will be avaialble.

I want to correct the situation today.

We are still working on making sure that all unit tests pass for Aspose.Foundation (our internal library that contains the PDF and XPS renderers, platform independent graphics, imaging, font utilities etc).

Currently Aspose.Foundation, the autoported to Java version happily produces PDF and XPS output that matches our .NET product output very very closely.

The number of unit tests that pass today in Aspose.Foundation is 86% (it was 76% when I last reported).

I am attaching some screenshots for you. We spent several days "fixing the kittens". There are about 40 test files with small kitten images of different formats and color depths. It took a while to get them all working on Java.

**This image shows that many different image formats are supported when rendering to PDF and XPS in Aspose.Words for Java.**  

**This shows how well Aspose.Words for Java converts a Windows Metafile (WMF, EMF) to a vector graphic and renders to PDF and XPS exactly the same.**  

**This shows that Aspose.Words for Java supports exporting Microsoft Word document form fields as PDF form fields.**  

**Clipping works. This is used both when rendering Word documents (some layout areas need to be clipped) as well as rendering metafiles.**








