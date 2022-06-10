---
title: 'Convert PDF to Word DOC or DOCX Programmatically in C#'
date: Sun, 24 Nov 2019 15:24:15 +0000
draft: false
url: /2019/11/24/convert-pdf-to-word-doc-docx-in-csharp-vb-net/
author: Kashif Iqbal
summary: ''
tags: ['.NET API', 'C#', 'Convert PDF to DOC', 'Convert PDF to DOC in C#', 'Convert PDF to Word', 'PDF to DOC', 'PDF to DOCX', 'PDF to Word .NET', 'PDF to Word C#', 'convert PDF files']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-net.jpg" alt="Convert PDF to Word">}}


In this article, I am going to demonstrate how to accurately and effortlessly **convert PDF to Word** document including conversion of **PDF to DOC** and **PDF to DOCX** formats. Earlier versions of Microsoft Word saved documents in binary format with [.doc][1] extension. With the release of Office 2007, Microsoft adopted the Office Open XML (OOXML) that is based on a combination of XML and binary files combined together as [ZIP][2] archives. MS Word now uses [.docx][3] as the default extension for saving documents.

The conversion of PDF to DOC and PDF to DOCX could be required in various scenarios. For example, you may want to make the PDF editable or you want to avoid retyping content of PDF into a Word document keeping the original formatting. Another use case could be the bulk PDF to DOC or DOCX conversions without any specialized software. Keeping an eye on such a scenario, this article covers the following PDF to Word conversion programmatically in C#:

*   Convert PDF to DOC in C#
*   Convert PDF to DOCX in C#
*   Convert PDF to DOC with additional settings

## C# PDF to Word DOC or DOCX Converter

[Aspose.PDF for .NET][4] owns a powerful PDF to DOC or DOCX converter API that lets you convert [PDF to Word documents][5] in your .NET applications within a few lines of code. The API can be used in WinForms, ASP.NET, web services, or any .NET based application. You can either [download][6] the API or install it using the [NuGet Package Manager][7] in your project.

## Convert PDF to DOC in C#

The following are the steps to convert PDF to DOC using Aspose.PDF for .NET.

*   Load the PDF documents using the [Document][8] class.
*   Save the document with .doc extension using [Document.Save(string)][9] method.

The following code sample shows how to convert PDF to Word DOC using C#.

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-DocumentConversion-PDFToDOC-PDFToDOC.cs" >}}

## Convert PDF to DOCX in C#

Converting [PDF to DOCX][10] is similar to PDF to DOC conversion as shown earlier. The API has the [DocSaveOptions][11] class that allows you to set the document format to DOCX. The following are the steps to convert PDF to DOCX:

*   Load the PDF documents using the [Document][12] class.
*   Set the output document format as DOCX using [DocSaveOptions][13] class.
*   Save the document with .docx extension using [Document.Save(string)][14] method.

The following code sample shows how to convert a PDF to Word DOCX in C#.

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-DocumentConversion-PDFToDOC-ConvertToDOCX.cs" >}}

## Convert PDF to DOC with Additional Options

Aspose.PDF for .NET provides various other options to customize the PDF to DOC or DOCX conversion. The [DocSaveOptions][15] class exposes the properties to improve or enhance the PDF to DOC conversions, such as image resolution, the distance between lines, and etc. The following code shows how to set additional properties when converting PDF to DOC in C#.

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-DocumentConversion-PDFToDOC-SaveUsingSaveOptions.cs" >}}

## Conclusion

In this article, you have learned some simple ways of converting PDF to DOC and PDF to DOCX using C#. If you want to know more about the powerful conversion features of Aspose.PDF for .NET then you can head-on to the API documentation section, [Conversion of PDF to other formats][16]. Download your free copy of [Aspose.PDF for .NET][17] and you can get started in no time by following the API documentation. If you have any queries, feel free to post to [Aspose.PDF forum][18]. We’ll be glad to assist you with your queries and inquiries.

## See Also

*   [Convert Word DOC or DOCX to PDF Programmatically in C#][19]




[1]: https://wiki.fileformat.com/word-processing/doc/
[2]: https://wiki.fileformat.com/compression/zip/
[3]: https://wiki.fileformat.com/word-processing/docx/
[4]: https://products.aspose.com/pdf/net
[5]: https://docs.aspose.com/display/pdfnet/Convert+PDF+file+to+other+Formats#ConvertPDFfiletootherFormats-ConvertPDFtoWordDOC
[6]: https://downloads.aspose.com/pdf/net
[7]: http://nuget.org/packages/Aspose.pdf
[8]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[9]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[10]: https://docs.aspose.com/display/pdfnet/Convert+PDF+file+to+other+Formats#ConvertPDFfiletootherFormats-ConvertPDFtoWordDOCXinC#
[11]: https://apireference.aspose.com/net/pdf/aspose.pdf/docsaveoptions
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf/docsaveoptions
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[15]: https://apireference.aspose.com/net/pdf/aspose.pdf/docsaveoptions
[16]: https://docs.aspose.com/display/pdfnet/Working+with+Document+Conversion
[17]: https://downloads.aspose.com/pdf/net
[18]: https://forum.aspose.com/c/pdf
[19]: https://blog.aspose.com/2020/01/02/convert-word-doc-docx-to-pdf-in-csharp-net-core/




