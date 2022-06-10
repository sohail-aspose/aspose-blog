---
title: 'One Million Test Documents is Coming Along'
date: Tue, 28 Nov 2006 19:09:00 +0000
draft: false
url: /2006/11/28/62199/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Our project to test [Aspose.Words][1] against at least one million documents has started ticking.

Dmitry Vorobyev has developed a nice tool that queries Google for Microsoft Word documents and downloads them. In short test runs we downloaded more than 3000 DOC and RTF documents of various content and formatting.

We plan to download at least one million documents to our test machine and run Aspose.Words days and nights on it to load, convert and save documents and verify that it all works smoothly.

Microsoft Word formats (DOC, RTF, WordML) are very complex and not fully documented. When such files are created by programs other than Microsoft Word itself, the potential for little "anomalies" is great.

What "anomalies" I'm talking about?

For example, the SectionStartType enum has only few valid values (0..5 or so), but we came across documents that have value 236 in that field.

Another example, lists are identified by a list identifier within a document and "no list" value is usually zero, but we recently say 0x07ff used instead of zero.

The list can go on for long actually. Yet another example is that each style is of certain type (paragraph, character, list, table). Paragraph styles can be based on paragraph styles. Yet a document can come through which has a paragraph style based on a character style.

If you happen to use Aspose.Words for documents that have some "anomalies", you might find out that Aspose.Words was initially designed to be a pretty "strict reader". That is if it finds something unusual, something we have not seen before, it will throw an exception, usually the PleaseReportException asking you to send the document to us.

On one hand, this approach is good for quickly finding anomalies and helping us, developers to gain more knowledge about the format and develop robust code. But on the other hand it is a "reactive" approach and lets you, the customer, to experience the problem first, then get a fix.

So far we've been testing with about 2000 "problem" documents mostly obtained from our customers, but with the new Google-Proofing project we hope to turn from "reactive" to "proactive" and make sure Aspose.Words can safely read and process all documents with  "anomalies".




[1]: /Products/Aspose.Words




