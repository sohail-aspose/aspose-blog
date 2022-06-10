---
title: 'Converting Word Documents to PDF with Aspose.Words'
date: Fri, 12 Dec 2008 00:00:00 +0000
draft: false
url: /2008/12/12/converting-word-documents-to-pdf-with-aspose-words/
author: Romank
summary: ''
tags: ['Aspose.Words for .NET', 'aspose doc to pdf', 'aspose word to pdf', 'doc to pdf', 'doc to pdf c#', 'docx to pdf', 'docx to pdf c#', 'word to pdf', 'word to pdf c#']
categories: ['Aspose.Words Product Family']
---

Aspose.Words for .NET 6.0 introduces a new direct to PDF document conversion (see [Converting Word to PDF - A complete guide][1]. This means there are now two ways to convert documents to PDF and this deserves some explanation.

**Legacy Method**

As you can see the "old" method was to use Aspose.Words and Aspose.Pdf working together. This was the solution we choose as "fastest to the market" and it was the only one possible at the time. This solution has served us and customers since Aspose.Words for .NET 2.0, that's 3.5 years.

To convert documents to PDF that way you had to write about 20 lines of code. First, you had to instruct Aspose.Words to save the document in an XML format called Aspose.Pdf.Xml. Then you had to load that file into Aspose.Pdf, which in turn produced the PDF file on the output.

Due to various reasons we could not make a "tighter" integration at that time. Apart from the obvious coding complexity there were a number of other issues that we could not resolve. Some annoyances included the fact that any images inside a document had to be passed via files. This was not always convenient in server side scenarios.

There was a more important issue that Aspose.Words and Aspose.Pdf were developed by different development teams and at Aspose each team supports "their" product independently. Whenever a customer had a problem, they often had to bounce between two support forums and two support teams before the source of the problem was located.

Memory and CPU utilization was also a bit of a problem. The need to serialize a complete document into intermediary XML with image files on a side just to load it all back again in another library automatically added significant performance overheads.

**New Method, Direct **

Over the past several years we've been busy developing a Rendering Engine. That's a piece of code that takes a Word document and tries to lay it out into pages exactly like Microsoft Word would do that. Once laid out, it can render the pages into a "fixed-page" format. At the moment it can print, save to image, render to .NET Graphics or convert to PDF.

When we talk about DOC2PDF we sometimes use the phrase "convert to PDF" because it is easier for a customer to understand. But we sometimes use the phrase "render to PDF" because the work is actually done by the rendering engine.

To convert any document to PDF in Aspose.Words all you need to do is just call **Document.SaveToPdf.**

Needless to say, we recommend the new direct method for conversion of Word documents to PDF. The legacy method for conversion is still available in case you need it, but we plan to stop supporting it within 1-2 years depending on the customer feedback.




[1]: https://blog.aspose.com/2020/01/02/convert-word-doc-docx-to-pdf-in-csharp-net-core/)




