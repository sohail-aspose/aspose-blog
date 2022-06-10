---
title: 'Aspose.Words for .NET 9.3 delivers a bunch of long awaited fixes and improvements'
date: Tue, 03 Aug 2010 02:02:00 +0000
draft: false
url: /2010/08/03/aspose-words-for-net-9-3-delivers-a-bunch-of-long-awaited-fixes-and-improvements/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

It has been just under a month since we released 9.2. Our release cycle has recently been close to two months and we did not plan to release next version so soon. But we have been very productive this month and managed to close 82 issues, most of them had customers waiting for significant time. We decided no need to force so many customers to wait for another month just to repeat our regular two months release pattern.

I will just go over the most important things here and you can find the rest of the details on the release page [http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/entry251663.aspx][1]

**Endnotes are Supported in Rendering**

This was a long awaited feature and I am happy it is now done. Aspose.Words also supports footnotes rendering (was available for a few versions). There are some features (custom reference marks etc) that are not yet supported, but for majority documents and customers you should find footnotes and endnotes support in Aspose.Words adequate.

**Removed the Legacy PDF Conversion Method (via Aspose.Pdf.xml)**

This method (that required Aspose.Words + Aspose.Pdf and communication via an XML file) has been obsolete for long time. Now that we have supported endnotes in rendering, the direct to PDF conversion method has surpassed the legacy method by all parameters and we decided it was time to finally remove the old conversion method.

**No More Font Changes during Append Document etc**

Many customers reported several problems related to font in a document changed or other formatting lost after they combined several documents or document parts together. This was caused by complexities with theme and document default formatting, most of which we have managed to resolve in this version.

**Migration to Aspose.Words 9.2 or Higher Article is Ready**

We have made a lot of breaking changes in the public API last month when released 9.2. We listed the changes on the release page. Now we have added a more detailed article to the documentation that should make your migration easier.

Read the article http://www.aspose.com/documentation/.net-components/aspose.words-for-.net/howto-migrate-to-aspose-words-9-2-or-higher.html

**References to API Members in Documentation are Hyperlinked**

We ate our own "dog food" again and used Aspose.Words to make a tool that hyperlinked all the references to API members in the documentation. This will allow you to quickly jump to the API topics from the Programmers Guide documentation. The links follow the "MSDN style". E.g. if a particular member is mentioned on a topic more than once, only the first occurrence is hyperlinked.

See how a hyperlinked page looks like http://www.aspose.com/documentation/.net-components/aspose.words-for-.net/save-a-document.html




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/entry251663.aspx




