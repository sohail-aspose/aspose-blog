---
title: 'Convert PostScript PS/EPS Files to PDF in C#'
date: Mon, 10 Dec 2018 00:14:06 +0000
draft: false
url: /2018/12/10/convert-postscript-files-into-pdf-in-csharp/
author: Asad Ali
summary: ''
tags: ['Asad Ali']
---



{{< figure align=center src="images/aspose_page-for-net.png" alt="EPS Files to PDF in C#">}}


A PostScript (PS) file is saved in page description language and can contain text, vector graphics, and raster images. Whereas, the Encapsulated PostScript (EPS) format is used for images or drawings. In this article, you will learn how to convert** PS/EPS files into PDF** **using C#**.

*   [C# PS/EPS to PDF Converter API][1]
*   [Steps to Convert PostScript PS/EPS to PDF in C#][2]
*   [PS/EPS to PDF - C# Code][3]

## C# PS/EPS to PDF Converter API {#C#-PS-EPS-to-PDF-Converter-API}

[Aspose.Page for C#][4] API is designed to work with PS and EPS files from within the .NET applications. Along with other manipulation features, the API provides a high fidelity conversion of PS/EPS to PDF. You can either [download][5] the API’s DLL or install it using [NuGet][6].

## Steps to Convert PostScript PS/EPS to PDF in C# {#Steps-to-Convert-PostScript-PS-EPS-to-PDF-in-C#}

The following are the steps to convert a PS/EPS file to PDF using Aspose.Page for .NET.

*   Load the file using the [PsDocument][7] class.
*   Create an instance of [PdfSaveOptions][8] class and set PDF options if required.
*   Define an instance of [FileStream][9] for output PDF file.
*   Create an instance of [PdfDevice][10] class and initialize it with output PDF's [FileStream][11] object.
*   Save document as PDF using [PsDocument.Save(PdfDevice, PdfSaveOptions)][12] method.

## PS/EPS to PDF - C# Code {#PS-EPS-to-PDF-C#-Code}

The following code sample converts PS/EPS to PDF in C#.

{{< gist aspose-com-gists 6f0d8b5420af1af6af2d064587dd6803 "Examples-Aspose.Page.Examples.CSharp-WorkingWithDocumentConversion-PostScriptToPdf-1.cs" >}}

## Conclusion

In this article, you have learned how to convert EPS/PS files to PDF using C#. In case you want to explore more about the C# EPS/PS file manipulation API, visit the [documentation][13].

## See Also

*   [Convert XPS, OXPS to JPG or PNG Image using C#][14]




[1]: #C#-PS-EPS-to-PDF-Converter-API
[2]: #Steps-to-Convert-PostScript-PS-EPS-to-PDF-in-C#
[3]: #PS-EPS-to-PDF-C#-Code
[4]: https://products.aspose.com/page/net
[5]: https://downloads.aspose.com/page/net
[6]: https://www.nuget.org/packages/Aspose.Page
[7]: https://apireference.aspose.com/page/net/aspose.page.eps/psdocument
[8]: https://apireference.aspose.com/page/net/aspose.page.eps.device/pdfsaveoptions
[9]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream
[10]: https://apireference.aspose.com/page/net/aspose.page.eps.device/pdfdevice
[11]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream
[12]: https://apireference.aspose.com/page/net/aspose.page.eps/psdocument/methods/save
[13]: https://docs.aspose.com/page/java/developer-guide/
[14]: https://blog.aspose.com/2020/11/02/convert-xps-to-jpg-png-image-csharp-vb-net/



