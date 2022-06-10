---
title: 'Get Page Count without Saving Document, Better PDF to Image and Image to PDF Conversion with Aspose.PDF for Java 10.1.0'
date: Tue, 07 Apr 2015 05:50:33 +0000
draft: false
url: /2015/04/07/get-page-count-without-saving-document-better-pdf-to-image-and-image-to-pdf-conversion-with-aspose.pdf-for-java-10.1.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'convert image to pdf in java', 'convert pdf to image in java', 'get page count of pdf in java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java_100.png" alt="Aspose.Pdf for Java logo">}}


A new release of [Aspose.PDF for Java 10.1.0][1] is published and it provides some exciting features which are already supported in its sibling (Aspose.PDF for .NET). Among these new features, the bugs reported in the previous releases are also resolved.

## Get page count without saving PDF

Unless the PDF file is saved and all the elements are actually placed inside the PDF document, we cannot get the page count for a particular document (because we cannot be certain about the number of pages in which all the elements will be accommodated). However starting with release Aspose.Pdf for Java 10.1.0, we have introduced a method named processParagraphs(...) which provides the feature to get page count for PDF document, without saving the file. So we can get page count information on the fly. Please try using the following code snippet to accomplish this requirement. For more information, please visit [Get PDF Page count][2].

```
// instantiate Document instance
com.aspose.pdf.Document doc = new com.aspose.pdf.Document();
// add page to pages collection of PDF file
com.aspose.pdf.Page page = doc.getPages().add();
// create a loop to add 300 TextFragment instances
for (int i = 0; i < 300; i++)
	// add TextFragment to paragraphs collection of first page of PDF
    page.getParagraphs().add(new TextFragment("Pages count test"));
// process paragraphs to get page count information
doc.processParagraphs();
System.out.println("Number of Pages in PDF = "+ doc.getPages().size()); 
```

## Public API Changes in Aspose.PDF for Java 10.1.0

In every new release, we make some modifications in API and the modifications include changes in class names, change in method name, new overloads for existing method etc. These changes are made to correct any spelling mistakes, support new feature requests, removal of redundant features implementation etc. In this new release, there have been some changes in the API and the details can be found over [Public API Changes in Aspose.PDF for Java 10.1.0][3]

## Miscellaneous fixes

As well as the enhancements and features discussed above, there have been numerous fixes related to recently introduced PDF to TIFF and TIFF to PDF conversion, adding watermark/stamp objects, printing PDF documents, SVG to PDF conversion and much more. Please download and try the latest [Aspose.PDF for .NET 10.1.0][4] release.




[1]: http://www.aspose.com/community/files/72/java-components/aspose.pdf-for-java/entry615512.aspx
[2]: https://docs.aspose.com/display/pdfjava/Get+and+Set+Page+Properties#GetandSetPageProperties-GetpagecountwithoutsavingPDF
[3]: https://docs.aspose.com/
[4]: https://downloads.aspose.com/pdf/net




