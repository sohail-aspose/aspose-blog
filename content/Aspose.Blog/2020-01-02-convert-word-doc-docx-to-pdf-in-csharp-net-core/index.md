---
title: 'Convert Word DOCX/DOC to PDF in C# .NET - A Complete Guide'
seoTitle: "Convert Word DOCX to PDF in C# | DOC to PDF, DOCX to PDF"
description: "Convert Word DOCX or DOC to PDF in C# .NET. Convert DOCX to PDF with multiple customization options in C#. Convert DOCX to PDF in C# or ASP.NET or .NET Core."
date: Thu, 02 Jan 2020 12:07:49 +0000
draft: false
url: /2020/01/02/convert-word-doc-docx-to-pdf-in-csharp-net-core/
author: Usman Aziz
summary: ''
tags: ['Aspose.Words for .NET', 'Microsoft Word to PDF C#', 'Word to pdf conversion C#', 'convert word to pdf in c#', 'doc to pdf', 'doc to pdf c#', 'docx to pdf', 'docx to pdf c#', 'word to pdf', 'word to pdf .net core', 'word to pdf c#', 'word to pdf in .NET', 'word to pdf programmatically']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Word-to-PDF-Conversion-C.png" alt="C# Word to PDF - DOC to PDF">}}


**Word to PDF** conversion is a common practice these days and it is preferred before sharing the documents. MS Word provides a builtin feature to save Word documents as PDF, however, there might be a case when you want to convert Word document to PDF programmatically such as in your web applications or you may require **batch Word to PDF** conversions without installing MS Office. So in this article, you will learn how to **convert Word DOCX** or **DOC** to **PDF** using **C#** in **.NET** or **.NET Core** framework.

## Word to PDF C# Conversion Scenarios

In this article, you will learn how to:

*   [Convert Word DOCX/DOC to PDF in C#][1]
*   [Convert desired pages of Word document to PDF in C#][2]
*   [Word to PDF conversion with a particular PDF Standard such as PDF 1.7, PDF/A-1a, etc.][3]
*   [Convert Word to PDF with image/text compression in C#][4]
*   [DOCX/DOC to PDF with a digital signature in C#][5]
*   [Word to PDF conversion with the desired JPEG quality for images][6]

## C# DOCX/DOC to PDF Converter

[Aspose.Words for .NET][7] is a powerful API for creating and manipulating popular Word document formats. The API also provides an easy way of converting Word documents to PDF with a high degree of fidelity. Therefore, for Word to PDF conversion in C#, we'll first add a reference to _Aspose.Words for .NET_ [DLL][8] in the project or install it using one of the following methods.

### Using NuGet Package Manager

*   Create/open the project in Visual Studio.
*   Go to NuGet Package Manager and search _Aspose.Words_.
*   Install the _Aspose.Words for .NET_.



{{< figure align=center src="images/Aspose.Words-NuGet.png" alt="Convert Word to PDF C# .NET">}}


### Using the Package Manager Console```
PM> Install-Package Aspose.Words
```

## Simple Word (DOCX/DOC) to PDF C# Conversion {#Convert-Word-DOCX-DOC-to-PDF-in-CSharp}

To convert a Word document to PDF, you'll have to invoke the [Document.Save()][9] method and specify the output file name with the “.pdf” extension. The following code sample shows how to convert Word DOC to PDF in C#.

{{< gist aspose-com-gists 7291ec6e6426497c7788117d1199990c "Convert-Word-To-PDF-CSharp.cs" >}}

### Word Document



{{< figure align=center src="images/Word-to-PDF-Conversion.png" alt="C# Convert Word to PDF ">}}


### Converted PDF



{{< figure align=center src="images/Word-to-PDF-Conversion2.png" alt="Word to PDF programmatically in C#">}}


## Convert Selected Pages of Word DOCX to PDF in C# {#Convert-desired-pages-of-Word-document-to-PDF-in-CSharp}

You can also customize the Word to PDF conversion by specifying the range of pages you want to get in the resultant PDF document. You can either convert first N pages or define a range of pages specifying the starting page's index. The following code sample shows how to convert 3 pages starting from the second page of Word document to PDF in C#.

{{< gist aspose-com-gists 7291ec6e6426497c7788117d1199990c "Convert-Word-To-PDF-Page-Range.cs" >}}

## Convert Word DOCX/DOC to PDF with a Particular PDF Standard in C# {#Convert-Word-DOC-DOCX-to-Particular-PDF-Standard-in-CSharp}

PDF documents may compliant with different PDF standards such as PDF 1.7, PDF 1.5, PDF/A-1a, etc. In accordance with this, _Aspose.Words for .NET_ allows specifying the PDF compliance level in Word to PDF conversion. You can specify the compliance level using [PdfCompliance][10] enum. The following code sample shows how to set the compliance level in Word DOCX to PDF conversion in C#.

{{< gist aspose-com-gists 7291ec6e6426497c7788117d1199990c "Convert-Word-To-PDF-Compliance.cs" >}}

## Convert Word to PDF with Text/Image Compression in C# {#Convert-Word-to-PDF-with-image-text-compression-in-CSharp}

The PDF format supports text and image compression to reduce the size of the document. Since a PDF document could be bulky in size, the compression of its content makes it easy to upload, share, print, etc. The text and image compression can also be applied in Word to PDF conversion using _Aspose.Words for .NET_.

### Text Compression Options

The following text compression options are available in [PdfTextCompression][11] enum.

*   _None_: Saving PDF without text compression.
*   _Flate_: Saving PDF with flate (ZIP) compression.

### Image Compression

The following image compression options are available in [PdfImageCompression][12] enum.

*   _Auto_: The API automatically selects the most appropriate compression for every image in the document.
*   _Jpeg_: Compression to JPEG images (does not support transparency).

The following code sample shows how to convert Word DOCX to PDF with text and image compression in C#.

{{< gist aspose-com-gists 7291ec6e6426497c7788117d1199990c "Convert-Word-To-PDF-Text-Image-Compression.cs" >}}

## C# Word to PDF Conversion with a Digital Signature {#DOCX-DOC-to-PDF-with-a-digital-signature-in-CSharp}

You can also apply a digital signature to the output PDF while performing Word to PDF conversion. The [CertificateHolder][13] class allows you to specify the digital certificate and the password. The [PdfDigitalSignatureDetails][14] class allows providing the details of the digital signature such as certificate holder, reason, location and date/time. The following code sample shows how to convert Word DOC/DOCX to PDF with a digital signature in C#.

{{< gist aspose-com-gists 7291ec6e6426497c7788117d1199990c "Convert-Word-To-PDF-Digital-Signature.cs" >}}

## Convert Word to PDF with Desired JPEG Quality in C# {#Convert-Word-to-PDF-with-Desired-JPEG-Quality-in-CSharp}

You can also specify the desired JPEG quality you want to get in the converted PDF document using [PdfSaveOptions.JpegQuality][15] property. The value of _JpegQuality_ may vary from 0 to 100 where 0 means the worst quality but maximum compression and 100 means the best quality but minimum compression.

The following code sample shows how to set JPEG quality when converting Word DOCX to PDF in C#.

{{< gist aspose-com-gists 7291ec6e6426497c7788117d1199990c "Convert-Word-To-PDF-Jpeg-Quality.cs" >}}

## Conclusion

In this article, you have learned how to convert MS Word DOCX/DOC documents using C# with various options. Visit [documentation][16] of _Aspose.Words for .NET_ to see the complete set of features offered by the API. For any questions or queries, contact us via our [forum][17].

## Related Article(s)

*   [PowerPoint Presentations to PDF Conversion in Java][18]
*   [Convert PowerPoint Presentations to PDF in C#][19]
*   [PDF to Excel in C#][20]
*   [Convert PDF to MS Word Documents in Java][21]
*   [Convert TXT to PDF in C#][22]
*   [HTML to Word in C#][23]
*   [Convert Word to Markdown in C#][24]
*   [Convert Word to EPUB in C#][25]




[1]: #Convert-Word-DOCX-DOC-to-PDF-in-CSharp
[2]: #Convert-desired-pages-of-Word-document-to-PDF-in-CSharp
[3]: #Convert-Word-DOC-DOCX-to-Particular-PDF-Standard-in-CSharp
[4]: #Convert-Word-to-PDF-with-image-text-compression-in-CSharp
[5]: #DOCX-DOC-to-PDF-with-a-digital-signature-in-CSharp
[6]: #Convert-Word-to-PDF-with-Desired-JPEG-Quality-in-CSharp
[7]: https://products.aspose.com/words/net
[8]: https://downloads.aspose.com/Words/NET
[9]: https://apireference.aspose.com/net/words/aspose.words.document/save/methods/2
[10]: https://apireference.aspose.com/net/words/aspose.words.saving/pdfcompliance
[11]: https://apireference.aspose.com/net/words/aspose.words.saving/pdftextcompression
[12]: https://apireference.aspose.com/net/words/aspose.words.saving/pdfimagecompression
[13]: https://apireference.aspose.com/
[14]: https://apireference.aspose.com/net/words/aspose.words.saving/pdfdigitalsignaturedetails/
[15]: https://apireference.aspose.com/net/words/aspose.words.saving/pdfsaveoptions/properties/jpegquality
[16]: https://docs.aspose.com/display/wordsnet/Product+Overview
[17]: https://forum.aspose.com/c/words
[18]: https://blog.aspose.com/2019/12/31/convert-powerpoint-ppt-pptx-to-pdf-in-java-using-aspose-slides/
[19]: https://blog.aspose.com/2020/02/12/convert-powerpoint-ppt-pptx-to-pdf-in-csharp-net/
[20]: https://blog.aspose.com/2020/01/03/convert-pdf-to-excel-in-csharp-net-pdf-to-xls-pdf-to-xlsx/
[21]: https://blog.aspose.com/2020/01/17/convert-pdf-to-word-doc-docx-in-java/
[22]: https://blog.aspose.com/2021/11/02/convert-txt-to-pdf-in-csharp/
[23]: https://blog.aspose.com/2020/12/09/convert-html-webpage-to-word-docx-csharp/
[24]: https://blog.aspose.com/2021/11/12/convert-word-to-markdown-using-csharp/
[25]: https://blog.aspose.com/2021/12/01/convert-a-word-to-epub-in-csharp/





