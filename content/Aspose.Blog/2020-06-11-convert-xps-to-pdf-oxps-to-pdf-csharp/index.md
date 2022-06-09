---
title: 'Convert XPS or OXPS to PDF Programmatically using C#'
seoTitle: ""
description: ""
date: Thu, 11 Jun 2020 20:14:58 +0000
draft: false
url: /2020/06/11/convert-xps-to-pdf-oxps-to-pdf-csharp/
author: Farhan Raza
summary: ''
tags: ['Convert XPS to PDF', 'XPS to PDF', 'convert oxps to pdf', 'oxps to pdf']
categories: ['Aspose.Page Product Family']
---



{{< figure align=center src="images/XPS-OXPS-to-PDF-Conversion-csharp.png" alt="">}}


XPS and OXPS files are frequently used for printing because of their resolution independence. However, sometimes we need to convert XPS to PDF or OXPS to PDF. [Aspose.Page for .NET][1] API lets you perform these conversions with high-fidelity and quick rendering. Let us explore the following use cases:

*   [Convert XPS to PDF Programmatically using C#][2]
    *   [Convert Specific Pages of XPS to PDF in C#][3]
    *   [Convert All Pages of XPS to PDF in C#][4]
*   [Convert OXPS to PDF Programmatically using C#][5]
    *   [Convert Specific Pages of OXPS to PDF in C#][6]
    *   [Convert All Pages Pages of OXPS to PDF in C#][7]

## Convert XPS to PDF Programmatically using C# {#section1}

XPS to PDF conversion is simple with Aspose.Page for .NET API. We will be learning the following approaches to perform XPS file conversion:

### i) Convert Specific Pages of XPS to PDF in C# {#section2}

For converting selected pages of XPS document to PDF, please follow the steps below:

1.  Initialize XPS input stream
2.  Load XPS document from stream
3.  Initialize [PdfSaveOptions][8] object
4.  Specify page numbers for conversion
5.  Save the document as PDF file

Below code snippet follows these steps and shows how to convert XPS to PDF using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "XPStoPDFpages.cs" >}}

This code snippet uses an XPS document containing several pages, as the input file. Whereas, only page numbers 1 and 3 are converted to PDF as specified in the code snippet. Following screenshot displays 2 pages rendered to PDF document:



{{< figure align=center src="images/XPStoPDF.png" alt="XPS to PDF">}}


### ii) Convert All Pages of XPS to PDF in C# {#section3}

You can convert a whole XPS file to PDF. Follow the steps below and all pages of the XPS file will be converted to a PDF file:

1.  Load input XPS file
2.  Initialize options object with necessary parameters
3.  Create an instance of [PdfDevice][9] for rendering
4.  Export XPS to PDF document

Below code snippet is based on all these steps which shows how to convert XPS file to PDF using C# language:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "XPStoPDFfile.cs" >}}

## Convert OXPS to PDF using C# {#section4}

OXPS format is an updated and advanced form of XPS file format. However, such files are not supported by some old operating systems. Aspose.Page for .NET API is capable of converting OXPS files as well. Let us proceed to learn the following usage scenarios:

### i) Convert Some Pages of OXPS to PDF in C# {#section5}

An OXPS file may contain many pages and any number of pages can be converted to PDF by following below steps:

1.  Load OXPS file
2.  Declare [PdfSaveOptions][10] object
3.  Set the page number(s) that you want to convert
4.  Render OXPS to PDF

Following code snippet shows how to convert OXPS to PDF using C#. It converts the first page of the OXPS file to PDF as mentioned in the code snippet.

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "OXPStoPDFpages.cs" >}}

### ii) Convert All Pages of OXPS to PDF in C# {#section6}

Converting all pages of OXPS is simple and related to the example we have considered above. Let us follow the steps below and convert all pages of OXPS file to a single PDF document:

1.  Initialize OXPS input stream
2.  Load the OXPS file from stream
3.  Instantiate an object of [PdfSaveOptions][11] class
4.  Export OXPS to PDF file

Below code snippet follows these steps one by one and converts OXPS to PDF using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "OXPStoPDFfile.cs" >}}

## Conclusion

In this article, you have learned how to convert **XPS to PDF** and **OXPS to PDF** programmatically using C#. You have learned with C# code examples and screenshots about high fidelity, efficient, and quick file format conversion. You can further explore [Aspose.Page for .NET][12] API with the help of [API documentation][13] and [API references][14]. Moreover, feel free to ask any inquiry at [Free Support Forums][15].

## See Also

[Create or Edit XPS Documents Programmatically in C++][16]




[1]: https://products.aspose.com/page/net
[2]: #section2
[3]: #section2
[4]: #section3
[5]: #section4
[6]: #section5
[7]: #section6
[8]: https://apireference.aspose.com/page/net/aspose.page.xps.presentation.pdf/pdfsaveoptions
[9]: https://apireference.aspose.com/page/net/aspose.page.eps.device/pdfdevice
[10]: https://apireference.aspose.com/page/net/aspose.page.xps.presentation.pdf/pdfsaveoptions
[11]: https://apireference.aspose.com/page/net/aspose.page.xps.presentation.pdf/pdfsaveoptions
[12]: https://products.aspose.com/page/net
[13]: https://docs.aspose.com/display/pagenet/Home
[14]: https://apireference.aspose.com/page/net
[15]: https://forum.aspose.com/c/page
[16]: https://blog.aspose.com/2020/03/24/create-or-edit-postscript-and-xps-documents-in-cpp/





