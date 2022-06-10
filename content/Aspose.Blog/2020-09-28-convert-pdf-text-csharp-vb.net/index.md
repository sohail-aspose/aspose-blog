---
title: 'Convert PDF to TEXT or TXT to PDF using C# VB.NET'
seoTitle: "Convert PDF to TXT | Text to PDF Programmatically in C# VB.NET"
description: "Convert PDF to TXT or Text to PDF Programmatically using C# or VB.NET. Read text from PDF file and convert it with or without formatting routines."
date: Mon, 28 Sep 2020 22:29:14 +0000
draft: false
url: /2020/09/28/convert-pdf-text-csharp-vb.net/
author: Farhan Raza
summary: 'PDF files are popular because they support text, images, animations, videos, and many other annotations. However, the text is the most important part of the majority of PDF documents. In this article, we will convert PDF to TXT file and TXT file to PDF format using C# .NET.'
tags: ['C# PDF to TEXT', 'C# PDF to TXT', 'C# TEXT to PDF', 'C# TXT to PDF', 'Convert TXT file to PDF format', 'Pdf to text', 'TXT to PDF', 'convert PDF to TXT', 'convert txt to pdf', 'text to pdf']
categories: ['Aspose.PDF Product Family']
---

[PDF][1] files are popular because they support text, images, animations, videos, and many other annotations. However, the text is the most important part of the majority of PDF documents. In this article, we will convert [PDF][2] to [TXT][3] file and TXT file to PDF format using C# .NET. This conversion comes handy in situations where you are concerned with only the text contents of PDF documents. Let us go through the following headings for an overview of upcoming topics:

*   [TXT to PDF or PDF to TXT Converter API][4]
*   [Convert PDF to TEXT File without Formatting using C# or VB.NET][5]
*   [Convert PDF to TXT File with Formatting Routines using C# or VB.NET][6]
*   [Convert TXT File to PDF Programmatically using C# or VB.NET][7]

**Tip**: You may be interested in a free [Text to GIF Converter][8] that allows you to generate animations from texts.

## TXT to PDF or PDF to TXT Converter {#section1}

PDF to TXT conversion as well as TXT file to PDF conversion is very helpful when your main concern is the text string used in the document. You can convert these file formats into one another with few simple steps using [Aspose.PDF for .NET][9] API. Being a .NET framework based API, it lets you work with C# as well as the VB.NET programming language. You can easily install the API in your .NET applications either by downloading the DLL files from [Downloads][10] or via the [NuGet][11] gallery.

After installing the API successfully, let us proceed to convert a PDF file to TXT file with two different approaches:

## Convert PDF to TEXT File without Formatting using C# or VB.NET {#section2}

First of all, we will convert the PDF to Text without any formatting routine. The text contents will be converted in their as-is form. So the output text will not follow any formatting as of the input PDF file. You need to follow the steps below to convert PDF to TXT with great efficiency and reliability.

1.  Load input PDF document
2.  Initialize an instance of [StringBuilder][12] Class
3.  Iterate through each page of the PDF document
4.  Read Text using [TextDevice][13] and [Raw][14] mode
5.  Save output Text as a TXT file

The code snippet below shows how to convert PDF to TXT file using C# or VB in .NET Framework:

{{< gist aspose-com-gists 21b0333293862a8730041a424ce1c5cc "Convert_PDF_Text_Raw.cs" >}}

## Convert PDF to TXT File with Formatting Routines using C# or VB.NET {#section3}

Now, let us consider the use case where you need to convert the PDF to Text with little bit of formatting routines. For example, paragraph indentations, tabs, styles, or column-wise formatting. You can easily render the text contents of a PDF document to a TXT file with C# by following the steps below:

1.  Load source PDF File
2.  Initiate a string variable
3.  Read through each page with [TextFormattingMode.Pure][15]
4.  Save converted TXT file

The following code snippet shows how to convert PDF to TXT file with formatting using C# or VB.NET language:

{{< gist aspose-com-gists 21b0333293862a8730041a424ce1c5cc "Convert_PDF_Text_Pure.cs" >}}

### Visual Comparison of PURE and RAW Text Conversion

The following screenshot is a visual comparison of the two approaches we have just discussed. You can notice that Pure mode (right-most window) shows the Text with the same formattings as in the PDF file (left-most window).



{{< figure align=center src="images/Convert_PDF_TXT_csharp-1024x436.png" alt="Convert PDF TXT csharp">}}


This screenshot of input and output files lets you decide which conversion approach suites you the best.

## Convert TXT File to PDF Programmatically using C# or VB.NET {#section4}

TXT files often contain huge text contents. You can easily convert a TXT file to PDF file with Aspose.PDF for .NET API. Simply follow the steps below to perform text to PDF conversion:

1.  Create an instance of [TextReader][16] class
2.  Initialize a PDF document and Add Blank Page
3.  Instantiate [TextBuilder][17] object
4.  Read each line of text from input TXT file
5.  Save output PDF file

The code snippet below explains how to programmatically convert a TXT file containing text, to a PDF document using C# or VB.NET language:

{{< gist aspose-com-gists 21b0333293862a8730041a424ce1c5cc "Convert_TXT_PDF.cs" >}}

## Conclusion

In this article, we have learned and explored the conversion of the text in PDF file to the TXT file format. Moreover, we have converted the text in a TXT file to a PDF document using C# or VB in .NET Framework. You can convert PDF and TXT files quite efficiently and quickly. However, if you have any concerns or queries, please feel free to write back to us at [Free Support Forum][18] or explore [Product Documentation][19]. We would love to hear from you!

## See Also

[Fill, Create, or Edit Fillable PDF Forms Programmatically using Java][20]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: https://docs.fileformat.com/word-processing/txt/
[4]: #section1
[5]: #section2
[6]: #section3
[7]: #section4
[8]: https://products.aspose.app/slides/text-to-gif
[9]: https://products.aspose.com/pdf/net
[10]: https://downloads.aspose.com/pdf/net
[11]: https://www.nuget.org/packages/Aspose.PDF/
[12]: https://docs.microsoft.com/en-us/dotnet/api/system.text.stringbuilder
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf.devices/textdevice
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf.text.textextractionoptions/textformattingmode
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf.text.textextractionoptions/textformattingmode
[16]: https://docs.microsoft.com/en-us/dotnet/api/system.io.textreader?view=netcore-3.1
[17]: https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/methods-auto/textbuilder/textbuilder-data-type
[18]: https://forum.aspose.com/c/pdf
[19]: https://docs.aspose.com/pdf/net/
[20]: https://blog.aspose.com/2020/07/20/create-fill-edit-fillable-pdf-form-field-java/





