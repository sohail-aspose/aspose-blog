---
title: 'Convert PDF Files to SVG using C#'
seoTitle: "Convert PDF to SVG in C# | C# PDF to SVG Conversion with High Fidelity"
description: "Use .NET PDF API to convert PDF files to SVG using C#. Use additional options to customize the PDF to SVG conversion within .NET applications."
date: Thu, 04 Feb 2021 18:31:27 +0000
draft: false
url: /2021/02/04/convert-pdf-files-to-svg-using-csharp/
author: Usman Aziz
summary: 'PDF has become one of the dominant file formats because of its cross-platform support. Due to the consistent layout of the PDF documents across heterogeneous devices, people use to prefer conversion of documents to PDF before sharing. However, in certain cases, PDFs need to be converted into another document format. PDF to SVG conversion is widely adopted in order to embed the content of PDF documents in webpages. Therefore, in this article, you will learn **how to convert PDF files to SVG using C#**.'
tags: ['convert pdf to svg in csharp', 'pdf to svg converter', 'pdf to svg csharp']
categories: ['Aspose.PDF Product Family']
---

[PDF][1] has become one of the dominant file formats because of its cross-platform support. Due to the consistent layout of the PDF documents across heterogeneous devices, people use to prefer conversion of documents to PDF before sharing. However, in certain cases, PDFs need to be converted into some other file format. PDF to [SVG][2] conversion is widely adopted in various scenarios i.e. in order to embed the content of PDF documents in webpages. Therefore, in this article, you will learn **how to convert PDF files to SVG using C#**.

*   [C# PDF to SVG Converter API][3]
*   [Convert PDF Files to SVG using C#][4]
*   [Convert PDF to SVG with Additional Options][5]
*   [Get a Free API License][6]

## C# PDF to SVG Converter API {#CSharp-PDF-to-SVG-Converter-API}

[Aspose.PDF for .NET][7] is a PDF manipulation API that lets you create new and process existing PDF files from within .NET applications. In addition, the API also allows you to convert PDF files to SVG with high fidelity. You can either [download][8] the API's DLL or install it via [NuGet][9].

```
PM> Install-Package Aspose.Pdf 
```

## Convert PDF Files to SVG using C# {#Convert-PDF-Files-to-SVG-using-CSharp}

The following are the steps to convert a PDF file to SVG using Aspose.PDF for .NET.

*   Load the PDF document using [Document][10] class.
*   Create an instance of [SvgSaveOptions][11] class.
*   Save PDF as SVG using [Document.Save(String, SvgSaveOptions)][12] method.

The following code sample shows how to convert a PDF file to SVG using C#.

{{< gist aspose-com-gists f47f16e4e36ef8723f8376ce908baeee "pdf-to-svg.cs" >}}

## Convert PDF to SVG with Additional Options {#Convert-PDF-to-SVG-with-Additional-Options}

Aspose.PDF for .NET also provides some additional options to customize the PDF to SVG conversion. For this, the API provides [SvgSaveOptions][13] class that contains the following options.

*   [CompressOutputToZipArchive][14] - Specifies whether the output will be created as one zip-archive.
*   [CustomStrategyOfEmbeddedImagesSaving][15] - Strategy for customized handling of referenced external image files.
*   [ScaleToPixels][16] - Specifies whether to scale the output document from typographic points to pixels.
*   [TreatTargetFileNameAsDirectory][17] - Defines whether to create a target directory with the same name as the requested output file.
*   [TryMergeAdjacentSameBackgroundImages][18] - To avoid visible boundaries between parts of same background images.

The following are the steps to customize PDF to SVG conversion using SvgSaveOptions class.

*   Load the PDF document using [Document][19] class.
*   Create an instance of [SvgSaveOptions][20] class.
*   Set the desired option such as [SaveOptions.CompressOutputToZipArchive][21].
*   Save PDF as SVG using [Document.Save(String, SvgSaveOptions)][22] method.

The following code sample shows how to convert a PDF file to SVG with additional options using C#.

{{< gist aspose-com-gists f47f16e4e36ef8723f8376ce908baeee "pdf-to-svg-customized.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

In case you want to try the API without evaluation limitations, you can [get a free temporary license][23].

## Conclusion

In this article, you have learned how to convert PDF files to SVG format using C#. Furthermore, the additional options to customize PDF to SVG conversion have been discussed with the code sample. You can explore more about the C# PDF API using [documentation][24].

## See Also

*   [Convert PDF to Word DOC or DOCX in C#][25]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/page-description-language/svg/
[3]: #CSharp-PDF-to-SVG-Converter-API
[4]: #Convert-PDF-Files-to-SVG-using-CSharp
[5]: #Convert-PDF-to-SVG-with-Additional-Options
[6]: #Get-a-Free-API-License
[7]: https://products.aspose.com/pdf/net
[8]: https://downloads.aspose.com/pdf/net
[9]: http://nuget.org/packages/Aspose.PDF
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[11]: https://apireference.aspose.com/pdf/net/aspose.pdf/svgsaveoptions
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/6
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf/svgsaveoptions
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf/svgsaveoptions/fields/compressoutputtoziparchive
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf/svgsaveoptions/fields/customstrategyofembeddedimagessaving
[16]: https://apireference.aspose.com/pdf/net/aspose.pdf/svgsaveoptions/fields/scaletopixels
[17]: https://apireference.aspose.com/pdf/net/aspose.pdf/svgsaveoptions/fields/treattargetfilenameasdirectory
[18]: https://apireference.aspose.com/pdf/net/aspose.pdf/unifiedsaveoptions/fields/trymergeadjacentsamebackgroundimages
[19]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[20]: https://apireference.aspose.com/pdf/net/aspose.pdf/svgsaveoptions
[21]: https://apireference.aspose.com/pdf/net/aspose.pdf/svgsaveoptions/fields/compressoutputtoziparchive
[22]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/6
[23]: https://purchase.aspose.com/temporary-license
[24]: https://docs.aspose.com/pdf/net
[25]: https://blog.aspose.com/2019/11/24/convert-pdf-to-word-doc-docx-in-csharp-vb-net/





