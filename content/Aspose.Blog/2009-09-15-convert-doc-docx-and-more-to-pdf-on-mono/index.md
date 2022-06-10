---
title: 'Convert Word DOC, DOCX to PDF on Mono'
date: Tue, 15 Sep 2009 18:05:00 +0000
draft: false
url: /2009/09/15/convert-doc-docx-and-more-to-pdf-on-mono/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

How about creating an application that generates DOC files, or maybe converts DOC and DOCX to PDF and much more, all on openSUSE or Ubuntu? Yes, you can run Aspose.Words for .NET with Mono and take the exciting document processing capabilities really multi-platform.

Aspose.Words has been known to work on Mono for quite a while, yet conversion to PDF (rendering) was not working. Document rendering was a major feature that we first released at end of 2008 and it worked on .NET only.

Now I am happy to tell that over the last few months we've invested a considerable effort into making the upcoming Aspose.Words for .NET 7.0 to convert documents to PDF well. Here is a little preview.

## Supported Platforms

We have [used the virtual machine][1] from the [Mono website][2] and tested in the following configuration:

We hope Aspose.Words will run with Mono in other operating systems too, but at this stage, we have not performed any other testing.

## Supported Features

Aspose.Words for .NET was initially designed to be used on Windows systems with the .NET Framework. We must give credit to the developers working on the Mono project, because when we just tried to run Aspose.Words on Mono we’ve been delighted to see that most of the functionality was working straight away.

But Aspose.Words for .NET is a big product that relies on many .NET features and not all of them are available in Mono or not working exactly like in .NET because Mono is still under development. In some cases, we’ve managed to implement missing functions ourselves, yet in some cases, the result is a limitation or a difference in the output because of our work on the multi-platform capabilities of Aspose.Words is still in progress.

The following table contains a brief list of Aspose.Words features and comments about their level of support on Mono.

<figure class="wp-block-table"><table class=""><tbody><tr><td><br>**Feature</strong></td><td><br><strong>Supported on Mono</strong></td><td><br><strong>Comment</strong></td></tr><tr><td><br><strong>Load and save DOC, OOXML, RTF, WordprocessingML</strong></td><td><br>Yes</td><td><br> </td></tr><tr><td><br><strong>Load and save OpenDocument, HTML/XHTML</strong></td><td><br>Yes</td><td><br> </td></tr><tr><td><br><strong>Save MHTML, EPUB, TXT</strong></td><td><br>Yes</td><td><br> </td></tr><tr><td><br><strong>Convert between the above formats</strong></td><td><br>Yes</td><td><br> </td></tr><tr><td><br><strong>Convert to PDF, XPS</strong></td><td><br>Yes</td><td><br>The layout of the text on a page might be different from the .NET version (less accurate).<br>Images in the PNG 16RGBA format are not supported.<br>Lines drawn using a brush or texture are not supported.<br>Not all gradient fills are supported.<br> </td></tr><tr><td><br><strong>Render document pages to images</strong></td><td><br>No</td><td><br>Work in progress. Some coordinate transformation modes in Mono are not working like in .NET.</td></tr><tr><td><br><strong>Program with the Document Object Model</strong></td><td><br>Yes</td><td><br> </td></tr><tr><td><br><strong>Mail merge from ADO.NET data sources</strong></td><td><br>Yes</td><td><br> </td></tr><tr><td><br><strong>Mail merge from custom data sources**</td><td><br>Yes</td><td><br> </td></tr></tbody></table></figure>




[1]: http://www.go-mono.com/mono-downloads/download.html
[2]: http://www.mono-project.com/Main_Page




