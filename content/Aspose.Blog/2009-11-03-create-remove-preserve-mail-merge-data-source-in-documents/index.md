---
title: 'Create/Remove/Preserve Mail Merge Data Source in Documents using Java'
date: Tue, 03 Nov 2009 23:43:00 +0000
draft: false
url: /2009/11/03/create-remove-preserve-mail-merge-data-source-in-documents/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Many customers have requested the following features over time:

1.  Make sure Aspose.Words does not lose mail merge data source settings in a document during open/save or conversion.
2.  Ability to specify a mail merge data source for a document programmatically.
3.  Ability to query or clear mail merge settings specified in a document.

We are happy to tell that we have implemented this. We have added the **Document.MailMergeSettings** property and **MailMergeSettings**, **Odso**, **OdsoFieldMapData**, **OdsoRecipientData** classes.

The current plan is as follows:

1.  Aspose.Words for Java 3.3 that has just been released [here][1] supports mail merge settings in DOC and DOCX formats and conversions between them and provides the public API.
2.  Aspose.Words for .NET 7.1 that is due out next week supports mail merge settings in DOC, DOCX and WordML formats and conversions and the public API as well.
3.  Support for mail merge settings in RTF will be coming next month.
4.  An article how to create a mail merge data source and code examples will be coming soon.




[1]: https://downloads.aspose.com/words/java




