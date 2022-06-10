---
title: 'How to Generate Real Microsoft Word DOC Documents from Crystal Reports'
date: Sun, 25 Mar 2007 13:33:00 +0000
draft: false
url: /2007/03/25/71350/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Crystal Reports have long been able to produce reports in RTF format (giving them the .DOC extension by default which always created confusion).

Using Aspose.Words you can quickly and easily convert from RTF to real DOC. Either on the server or on the client.

The code to convert any RTF to DOC is as simple as this:

```
Aspose.Words.Document doc = new Document("C:\\MyFolder\\MyFile.rtf");
doc.Save("C:\\MyFolder\\MyFile.doc");
```

Conversions in any direction between Microsoft Word formats (DOC, RTF and WordML) in Aspose.Words are high-fidelity (very accurate).

We have not figured out what is the best way of hooking this up actually to Crystal Reports (it does not seem extensible in this way), but you can write a simple .NET application to do the conversion using Aspose.Words and convert documents when you see fit. If you do find a way to hook this up to Crystal Reports, let us know.

Also, you can use this approach to convert between all other formats supported by Aspose.Words:

**From:**

*   DOC
*   RTF
*   WordML
*   HTML

**To:**

*   DOC
*   RTF
*   WordML
*   HTML
*   PDF
*   TXT








