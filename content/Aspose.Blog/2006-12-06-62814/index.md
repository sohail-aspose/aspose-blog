---
title: 'Beta RTF and WordprocessingML import available for download'
date: Wed, 06 Dec 2006 12:03:00 +0000
draft: false
url: /2006/12/06/62814/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Aspose.Words 4.0.3.1 includes Beta of RTF and WordprocessingML **import** features. The download is available here http://www.aspose.com/Community/forums/ShowThread.aspx?PostID=62813

You can try this:

Document doc = new Document(MyPath + "MyFile.rtf");

and

Document doc = new Document(MyPath + "MyFile.xml");

Note that ability to **export** to RTF and WordprocessingML is not Beta, these features were released in Aspose.Words 4.0.

To save in RTF or WordprocessingML do this:

doc.Save(MyPath + "MyFile.rtf", SaveFormat.Rtf);

and

doc.Save(MyPath + "MyFile.xml", SaveFormat.WordML);








