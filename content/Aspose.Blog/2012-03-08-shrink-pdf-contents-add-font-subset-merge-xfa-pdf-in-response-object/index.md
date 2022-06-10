---
title: 'Shrink PDF contents, add font subset, merge XFA, PDF in Response object'
date: Thu, 08 Mar 2012 08:21:00 +0000
draft: false
url: /2012/03/08/shrink-pdf-contents-add-font-subset-merge-xfa-pdf-in-response-object/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---

![Aspose.Pdf icon][1]

We are very much excited to announce some great new features in [Aspose.Pdf for .NET 6.8.0][2]. With this new release, you can shrink the contents of a PDF file to a smaller size so you'll save hard disk space. The TextFragmentAbsorber has always been a great mechanism for searching & replacing particular text strings inside a PDF file and now it lets you include a subset of the font used when replacing PDF file contents. Use the `TextFragmentAbsorber.TextFragments[1].TextState.Font.IsSubset = true;` code line to include a subset of a font used for in the text replacement process in the output file instead of including the complete font file. This features helps to reduce the size of PDF document significantly.

The Pdf class under the Aspose.Pdf.Generator namespace contains an overloaded Save method which returns the resultant PDF in Response object. To provide the same feature for the Document class, we have introduced a new overloaded method `Document.Save(HttpContext.Current.Response, "test.pdf", ContentDisposition.Inline, new PdfSaveOptions());` which returns the resultant PDF to Response object. Please note that in this release, we have specifically improved the PDF concatenation functionality and we also are introducing the capability to merge XFA forms. Numerous issues related to form field filling, text extraction, conversion of PDF files into image format, PDF printing and much more have been fixed in this release.

Please visit the following link for further details on what's new & fixed in [Aspose.Pdf for .NET 6.8.0][3]




[1]: http://www.aspose.com/Images/aspose.pdf-logo2.jpg
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.pdf-for-.net/entry366517.aspx
[3]: http://www.aspose.com/community/files/51/.net-components/aspose.pdf-for-.net/entry366517.aspx




