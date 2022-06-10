---
title: 'Autoporting Aspose.Words for .NET to Java Weekly Progress - 19th Aug 2010'
date: Fri, 20 Aug 2010 00:05:00 +0000
draft: false
url: /2010/08/20/autoporting-aspose-words-for-net-to-java-weekly-progress-19th-aug-2010/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

In my earlier post http://www.aspose.com/community/blogs/aspose.words-product-family/archive/2010/08/12/when-conversion-to-pdf-in-aspose-words-for-java-will-be-fully-available.aspx I offered to post regular updates on our internal progress towards releasing a fully up-to-date (with field update, Table of Contents, footnotes etc) Word to PDF conversion in Aspose.Words for Java.

Here is an update for this week.

Compiles okay = 71.7% (up 1.7% from 70% last week)

Does not compile = 28.2%

While from this numbers you could estimate there are about 16 weeks to go to get to 100%, I think we are going to deliver much sooner. This week the amount of visible progress is little because:

1\. We had to take some effort away from autoporting to ensure the DrawingML roundtripping feature will be ready in Aspose.Words for .NET release at end of August.

2\. In autoporting we worked on the very tricky parts - abstracting our work with XML and images. So the number of C# source files we made autoportable was not much, but they all required large porting questions to solve. The percentage of files that requires such work in the whole project is small.

So time to get back to work and see how much we can advance next week.








