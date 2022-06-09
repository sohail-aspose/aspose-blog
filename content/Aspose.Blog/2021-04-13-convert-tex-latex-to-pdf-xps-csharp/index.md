---
title: 'Convert TeX (LaTeX) to PDF or XPS File Programmatically using C#'
seoTitle: "Convert TeX (LaTeX) to PDF or XPS File Programmatically using C#"
description: "You can convert TeX (LaTeX) files to PDF or XPS file programmatically using C# language. Export, change or typeset TeX files in .NET."
date: Tue, 13 Apr 2021 16:29:00 +0000
draft: false
url: /2021/04/13/convert-tex-latex-to-pdf-xps-csharp/
author: Farhan Raza
summary: 'A TeX file may contain text, symbols, or arithmetic expressions. These are used for typesetting the documents and you can typeset TeX input to PDF, XPS, and several other supported formats. In this article, you will be learning how to convert TeX to PDF or XPS files programmatically using C#.'
tags: ['Convert LaTeX to PDF C#', 'Convert TeX to PDF in C#', 'TeX to PDF', 'TeX to XPS']
categories: ['Aspose.TeX Product Family']
---



{{< figure align=center src="images/TeX-to-PDF-XPS.png" alt="Convert TeX to PDF XPS">}}


A [TeX][1] file may contain text, symbols, or arithmetic expressions. These are used for typesetting the documents and you can typeset TeX input to [PDF][2], [XPS][3], and several other [supported formats][4]. In this article, you will be learning how to convert TeX to PDF or XPS files programmatically using C#. The following sections explain the topic in detail:

*   [TeX to PDF or XPS Converter – C# API Installation][5]
*   [Convert TeX (LaTeX) to PDF Programmatically using C#][6]
*   [TeX ZIP directory to PDF ZIP Directory Conversion using C#][7]
*   [Convert LaTeX (TeX) to XPS File Programmatically using C#][8]
*   [Get Free API License][9]

## TeX to PDF or XPS Converter – C# API Installation {#section1}

[Aspose.TeX for .NET][10] API has been designed for typesetting TeX files to different file formats like PDF, XPS, or images. You can quickly configure the API by downloading the DLL file from the [Downloads][11] section, or you can install it from [NuGet][12] with the following installation command:

```
PM> Install-Package Aspose.TeX
```

## Convert TeX (LaTeX) to PDF Programmatically using C# {#section2}

You can convert TeX to PDF file with the steps below:

1.  Create typesetting options for default [ObjectTeX][13] format.
2.  Specify console or memory stream as an output terminal.
3.  Set options for rendering into PDF format.
4.  Call [TexJob][14] class constructor and save output PDF with [PdfDevice][15] class object.

The following code snippet explains how to convert TeX to PDF file programmatically using C#:

{{< gist aspose-com-gists b6ff8a0d32ac7353678b69d23db6e8c6 "convert-TeX-to-Pdf.cs" >}}

The arguments passed to the [TexJob][16] class constructor are noteworthy here. The first one refers to the path to the input TeX file, the second is [Device][17] type while the third one refers to [TexOptions][18].

## Convert TeX ZIP directory to PDF ZIP Directory using C# {#section3}

You may need to convert multiple TeX files to PDF at a time. In such cases, you may convert TeX file in a ZIP archive to PDF document in zipped form. You need to follow the steps below:

1.  Open streams on ZIP archives as the input and output working directory.
2.  Create typesetting options using the [TeXOptions][19] class object.
3.  Create and specify saving options with [PdfSaveOptions][20].
4.  Run typesetting with [TexJob][21] class constructor.

The code below elaborates how to convert TeX ZIP archive to PDF ZIP archive programmatically using C#:

{{< gist aspose-com-gists b6ff8a0d32ac7353678b69d23db6e8c6 "convert-TeX-zip-PDF.cs" >}}

## Convert TeX (LaTeX) to XPS File Programmatically using C# {#section4}

You can convert TeX to XPS file with the following steps:

1.  Create typesetting options on ObjectTeX engine extension.
2.  Specify a file system working directory for input and output.
3.  Convert TeX to XPS by running Typesetting with [XpsDevice][22].

The following code shows how to convert TeX file to XPS programmatically using C#:

{{< gist aspose-com-gists b6ff8a0d32ac7353678b69d23db6e8c6 "convert-TeX-to-XPS.cs" >}}

## Get Free API License {#section5}

You can evaluate the API with full access by requesting a [Free Temporary License][23].

## Conclusion

In this article, you have explored how to convert TeX files to PDF or XPS files programmatically using C#. Moreover, you have also learned how to convert a TeX file in a ZIP archive and create an output ZIP directory. You can have a look at several other features by visiting the API [Documentation][24]. Please feel free to contact us at the [Free Support Forum][25] in case of any concerns.

## See Also

*   [Convert XPS or OXPS to PDF Programmatically using C#][26]
*   [Convert LaTeX to PNG or JPG Image in C#][27]




[1]: https://docs.fileformat.com/page-description-language/tex/
[2]: https://docs.fileformat.com/pdf/
[3]: https://docs.fileformat.com/page-description-language/xps/
[4]: https://docs.aspose.com/tex/net/supported-file-formats/
[5]: #section1
[6]: #section2
[7]: #section3
[8]: #section4
[9]: #section5
[10]: https://products.aspose.com/tex/net
[11]: https://downloads.aspose.com/tex/net
[12]: https://www.nuget.org/packages/Aspose.TeX/
[13]: https://apireference.aspose.com/tex/net/aspose.tex/texconfig/methods/objecttex
[14]: https://apireference.aspose.com/tex/net/aspose.tex/texjob
[15]: https://apireference.aspose.com/tex/net/aspose.tex.presentation.pdf/pdfdevice
[16]: https://apireference.aspose.com/tex/net/aspose.tex/texjob
[17]: https://apireference.aspose.com/tex/net/aspose.tex.presentation/device
[18]: https://apireference.aspose.com/tex/net/aspose.tex/texoptions
[19]: https://apireference.aspose.com/tex/net/aspose.tex/texoptions
[20]: https://apireference.aspose.com/tex/net/aspose.tex.presentation.pdf/pdfsaveoptions
[21]: https://apireference.aspose.com/tex/net/aspose.tex/texjob
[22]: https://apireference.aspose.com/tex/net/aspose.tex.presentation.xps/xpsdevice
[23]: https://purchase.aspose.com/temporary-license
[24]: https://docs.aspose.com/tex/net/
[25]: https://forum.aspose.com/c/tex
[26]: https://blog.aspose.com/2020/06/11/convert-xps-to-pdf-oxps-to-pdf-csharp/
[27]: https://blog.aspose.com/2021/12/28/convert-latex-to-png-jpg-csharp/





