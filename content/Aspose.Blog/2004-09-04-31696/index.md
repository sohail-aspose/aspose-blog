---
title: 'Aspose.Word and VSTO2005'
date: Sat, 04 Sep 2004 11:56:00 +0000
draft: false
url: /2004/09/04/31696/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

Yes, it is “and”, not “vs”.

Of course, VSTO2005 is one of the hottest topics for us at Aspose as it could be very easy for us to lose any competition to Microsoft.

The current thinking is to avoid competition (at least direct one) and do things that VSTO2005 does not do. We are confident there is a bright future for all: VSTO2005, Aspose.Word and Aspose.Cells together as we will always try to maneuvre quickly and provide new and exciting features to our customers.

Here is a thing to keep in mind if you are evaluating whether to use Aspose.Word or VSTO2005: Look for what the products do and don't do. And often you will end up requiring both.

We are still evaluating VSTO2005 and working out our strategy, but here are few ideas that might (or might not) materialize in the near future:

1\. VSTO2005 offers tight integration of MS Word and Excel as document designers into VS.NET. This is useful only for projects that need to build some code around a particular document. Most of the Aspose customers need different approach - they already have documents, possibly created by users, not developer and they just need to somehow process them. This is to say that Aspose.Word is not likely to offer any visual editors for VS.NET like VSTO2005 does.

2\. Aspose.Word allows to programmatically examine and manipulate document content using native .NET code at incredible speed, using an object model similar to MS Word Automation. This is a distinct feature of Aspose.Word - not available in VSTO2005 where you will need to use COM Interop to do these things. In the near future we will grow the document object model significantly and it will still be similar to MS Word object model so it is easy for you to switch from VBA to Aspose.Word.

3\. While VSTO2005 offers capability to fill documents with data at the server without the need for MS Office to be installed, we are evaluating this feature and think it is quite limited in functionality. From what we see now it allows to fill documents with data only. Aspose.Word offers that, plus all document manipulation API described above.

4\. Aspose.Word allows to convert documents into HTML and PDF format. We will extended this to support import/export in HTML, RTF and possibly other formats. We will continously work to improve the precision and quality of conversions.

5\. Aspose.Word will allow printing and viewing documents. Printing can be used on a server or a client and you will not need MS Office installed. Viewing control can be used in a Windows or ASP.NET application if you don't want to require the clients to have MS Word installed.

I hope I have not given many secrets out, yet kept you entertained about the future of Aspose.Word.







