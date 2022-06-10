---
title: 'Aspose.Words 10.7 Released'
date: Sat, 03 Dec 2011 10:17:50 +0000
draft: false
url: /2011/12/03/aspose.words-10.7-released/
author: Romank
summary: ''
tags: ['.NET', 'Microsoft Word', 'java', 'product release']
categories: ['Aspose.Words Product Family']
---

![Aspose.Words logo][1]

You can immediately download our next regular Aspose.Words release from the following links:

*   [Aspose.Words for .NET 10.7][2]
*   [Aspose.Words for Java 10.7][3]

The rest of this topic mentions some of the features that we have delivered in this release:

## ActiveX Controls in DOCX Documents

Support for OLE objects embedded in Word documents has been available in Aspose.Words for long time. ActiveX controls is a technology related to OLE. ActiveX controls are stored in the same way as OLE objects in the binary .DOC documents and they have been already supported by Aspose.Words. But ActiveX controls stored in OOXML documents are stored differently to OLE objects and they were not supported by Aspose.Words during DOCX open/save cycles.

Although ActiveX controls inside wordprocessing documents is not a mainstream thing these days, the lack of this feature in Aspose.Words was causing grief to some of our key customers. Starting from this release ActiveX controls stored in OOXML documents are preserved by Aspose.Words during open/save cycles.

Conversion of ActiveX controls between the binary .DOC and OOXML formats is still not available (an ActiveX control is converted to a picture), but this will be our next feature.

## Custom Footnote Marks Rendering

Footnotes and endnotes in Word documents always have a reference mark. Most of the time, the reference mark is an auto-generated number, such as i, ii, iii etc. But it turns our many customers actually use custom characters as reference mark for footnotes and endnotes, for example "\*".

This Aspose.Words release addresses a long-standing feature request to support proper rendering of footnotes and endnotes with reference marks to PDF and other formats.




[1]: http://www.aspose.com/Images/aspose.words-logo2.jpg
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/category1188.aspx
[3]: http://www.aspose.com/community/files/72/java-components/aspose.words-for-java/category1378.aspx




