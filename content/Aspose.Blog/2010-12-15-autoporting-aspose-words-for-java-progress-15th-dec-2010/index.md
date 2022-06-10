---
title: 'Autoporting Aspose.Words for Java Progress - 15th Dec 2010'
date: Wed, 15 Dec 2010 01:00:00 +0000
draft: false
url: /2010/12/15/autoporting-aspose-words-for-java-progress-15th-dec-2010/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Today there are only 1176 out of 8805 unit tests are failing in Aspose.Words for Java.

Some unit tests are comparing output documents with "gold" (a.k.a last known good) documents for regression testing.

Now both the original Aspose.Words for .NET and autoported Aspose.Words for Java need to produce documents that match the same set of gold files initially produced by Aspose.Words for .NET. Only a small number of files will be different and accepted as "java only golds".

Here is an example in the output difference that we are very proud of:

**aspose.GoldDifferenceException: Found difference in line 7 at position 51.  
User: t="Aspose.Words for Java 9.5.0.0" />  
Gold: t="Aspose.Words for .NET 9.5.0.0" />**

That basically confirms yes, we are going to be releasing Aspose.Words for .NET and Java with the same functionality, same version numbers, on the same release days in the very near future.








