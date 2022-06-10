---
title: 'Pretty Format HTML, RTF and WordML Output'
date: Tue, 05 Sep 2006 13:17:00 +0000
draft: false
url: /2006/09/05/55901/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

Did you know that in Aspose.Words 4.0 you can turn an option on to pretty format output to HTML, RTF and WordML files?

This could be very useful for you when looking at these files in a text editor trying to figure out what happens with certain document elements or formatting.

doc.SaveOptions.ExportPrettyFormat = true;  
doc.Save(@"C:\\MyFile.html", SaveFormat.FormatHtml);  
doc.Save(@"C:\\MyFile.xml", SaveFormat.FormatWordML);  
doc.Save(@"C:\\MyFile.rtf", SaveFormat.FormatRtf);

The above code will produce human-readable documents with line breaks and indentation. This option is turned off by default.







