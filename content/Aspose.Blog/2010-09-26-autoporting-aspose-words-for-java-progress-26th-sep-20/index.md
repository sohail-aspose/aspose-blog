---
title: 'Autoporting Aspose.Words for Java Progress - 26th Sep 20'
date: Sun, 26 Sep 2010 02:04:00 +0000
draft: false
url: /2010/09/26/autoporting-aspose-words-for-java-progress-26th-sep-20/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Just yesterday we had only 86% unit tests passing in our internal Aspose.Foundation for Java library. Today I am happy to say it is 100% green.

Just to remind you we are trying to make Aspose.Words for Java by automatically converting Aspose.Words for .NET written in C# to Java using our own tool.

Aspose.Foundation is an internal library, a part of Aspose.Words. We first achieved compile on the generated Java source code on 27th August. We then spent this month getting all unit tests to pass by fixing all autoporting deficiencies.

What's next?

1\. Achieve compile for the rest of the Aspose.Words for Java code.

2\. Achieve 100% unit tests for the rest of the Aspose.Words for Java code.

I'd say Aspose.Foundation is about 1/3rd of Aspose.Words source code. It might appear that we are only 1/3rd complete, but in terms of autoporting difficulty I think Aspose.Foundation was the most complex part because it contains lower-level modules (for example to deal with images) that need a lot of platform abstraction work.

This makes Nov-Dec 2010 look promising for Aspose.Words for Java 10.0 delivery.

Aspose.Words for .NET 6.0 that featured the PDF and XPS rendering engine appeared end of 2008.

Aspose.Words for Java 4.0 that featured our first manual porting of the PDF rendering feature appeared end of 2009.

It would be nice to see Aspose.Words for Java 10.0 that is our first automatically ported product before end of 2010 finally.








