---
title: 'Load OpenDocument (ODT) Documents in Aspose.Words'
date: Sun, 19 Oct 2008 12:40:00 +0000
draft: false
url: /2008/10/19/load-opendocument-odt-documents-in-aspose-words/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

This is the most important new feature in Aspose.Words for .NET 5.3.0 that I almost forgot to mention!

It is now possible to load OpenDocument (OpenOffice Writer) documents in Aspose.Words! Aspose.Words will recognize ODT files automatically and also a new **LoadFormat.Odt** enumerated value has been added.

It is now easy to convert ODT to OOXML or any other document format supported by Aspose.Words:

Document doc = new Document(@"C:\\MyFile.odt");  
doc.Save(@"C:\\MyFile Out.docx");

Note: Loading OpenDocument is in Beta at the moment. We hope it will come out of Beta in the next Aspose.Words for .NET release.

We hope that the Adobe Buzzword team will be happy since they've been the primary push for ODT support in Aspose.Words. It is interesting to note that ODT to/from Microsoft Word documents conversion is far from trivial because of the many fundamental differences between the document structures. At the moment the set of ODT features supported by Aspose.Words is limited to features found in Buzzword.








