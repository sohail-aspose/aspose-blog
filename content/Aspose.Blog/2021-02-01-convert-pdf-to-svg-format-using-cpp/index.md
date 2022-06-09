---
title: 'Convert PDF to SVG Format using C++'
seoTitle: "Convert PDF to SVG Format using C++ | C++ PDF to SVG Converter API"
description: "Use the C++ PDF to SVG converter API to convert PDF files into SVG format with just a few lines of code. Download the API for free from NuGet."
date: Mon, 01 Feb 2021 13:13:24 +0000
draft: false
url: /2021/02/01/convert-pdf-to-svg-format-using-cpp/
author: Muhammad Ahmad
summary: '[PDF][1] is a widely used document format for exchanging documents between individuals and different organizations. It is a standard document format, but sometimes it is not the ideal format for the situation. Nowadays, a lot of people are consuming content on their mobile devices such as smartphones or tablets. In such cases, [SVG][2] is a good alternative. SVG can be scaled to different screen sizes without losing quality and is the most used format for websites. Webpages can also use CSS styling to display SVG content. For this purpose, you will need to convert the PDF files to SVG. In this article, you will learn **how to convert PDF files to SVG format using C++**.'
tags: ['C++ PDF to SVG', 'C++ PDF to SVG Converter', 'Convert PDF to SVG C++', 'PDF to SVG C++']
categories: ['Aspose.PDF Product Family']
---

[PDF][3] is a widely used document format for exchanging documents between individuals and different organizations. It is a standard document format, but sometimes it is not the ideal format for the situation. Nowadays, a lot of people are consuming content on their mobile devices such as smartphones or tablets. In such cases, [SVG][4] is a good alternative. SVG can be scaled to different screen sizes without losing quality and is the most used format for websites. Webpages can also use CSS styling to display SVG content. For this purpose, you will need to convert the PDF files to SVG. In this article, you will learn **how to convert PDF files to SVG format using C++**.

*   [C++ PDF to SVG Converter API – Free Download][5]
*   [PDF to SVG C++ Conversion][6]
*   [Convert PDF to SVG with Additional Options][7]
*   [Get a Free License][8]

## C++ PDF to SVG Converter API – Free Download {#CPP-PDF-to-SVG-Converter-API-Free-Download}

[Aspose.PDF for C++][9] API provides a lot of features for working with PDF files. The API allows you to create, read, convert, and manipulate PDF documents without using Adobe Acrobat. To convert PDF files to SVG, firstly, you need to download the API. Begin by downloading the API for free from the [official website][10] or by using the [NuGet][11] package.

## PDF to SVG C++ Conversion {#PDF-to-SVG-CPP-Conversion}

The following are the steps that you need to follow for converting PDF documents to SVG format:

*   Firstly, use the [Document][12] class to load the PDF file.
*   Create an object of the [SvgSaveOptions][13] class.
*   Lastly, save the PDF as SVG by using the [Document->Save(System::String outputFileName, System::SharedPtr<SaveOptions> options)][14] method.

The following code snippet shows converting PDF to SVG using C++.

{{< gist aspose-com-gists 6ba6048d7d9f0ecbccca3b9c30762302 "PDF-to-SVG-Conversion.cpp" >}}

## Convert PDF to SVG with Additional Options {#Convert-PDF-to-SVG-with-Additional-Options}

The [SvgSaveOptions][15] class provides additional options to customize the PDF to SVG conversion. The following are the options provided by the [SvgSaveOptions][16] class.

*   [CompressOutputToZipArchive][17]: Use this option to create one zip-archive output file.
*   [CustomStrategyOfEmbeddedImagesSaving][18]: Use this option to specify the custom strategy for embedding external images to SVG. That strategy must process the resources and return a string URI of the saved resource.
*   [ScaleToPixels][19]: This option specifies whether to scale the output from typographic points to pixels.
*   [TreatTargetFileNameAsDirectory][20]: Set this option to _true_ to save the output file in the directory with the same name as the output file.

You can follow the steps given below to convert PDF to SVG with additional options:

*   Start by loading the PDF file by using the [Document][21] class.
*   Create an instance of the [SvgSaveOptions][22] class.
*   Set the desired option of the [SvgSaveOptions][23] class, such as [TreatTargetFileNameAsDirectory][24].
*   Finally, save the PDF as SVG with the [Document->Save(System::String outputFileName, System::SharedPtr<SaveOptions> options)][25] method.

The following code snippet demonstrates converting PDF to SVG with additional options.

{{< gist aspose-com-gists 6ba6048d7d9f0ecbccca3b9c30762302 "PDF-to-SVG-Conversion-with-additional-options.cpp" >}}

## Get a Free License {#Get-a-Free-License}

You can try the API without evaluation limitations by requesting [a free temporary license][26].

## Conclusion

In this article, you have learned how to convert PDF to SVG directly or by providing additional options to customize the conversion. Additionally, you can explore the Aspose.PDF for C++ API in detail by using the [official documentation][27].

## See Also

*   [Convert PDF to DOC and DOCX in C++][28]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/page-description-language/svg/
[3]: https://docs.fileformat.com/pdf/
[4]: https://docs.fileformat.com/page-description-language/svg/
[5]: #CPP-PDF-to-SVG-Converter-API-Free-Download
[6]: #PDF-to-SVG-CPP-Conversion
[7]: #Convert-PDF-to-SVG-with-Additional-Options
[8]: #Get-a-Free-License
[9]: https://products.aspose.com/pdf/cpp
[10]: https://downloads.aspose.com/pdf/cpp
[11]: https://www.nuget.org/packages/Aspose.Pdf.cpp
[12]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[13]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.svg_save_options
[14]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a6383c010776212483f51cc41235924db
[15]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.svg_save_options
[16]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.svg_save_options
[17]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.svg_save_options#aded335fda0a9ff2c4ba0828a6885a2a0
[18]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.svg_save_options#a877f396829fa55b338544df7c2ce3829
[19]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.svg_save_options#a387f2a77519ead8fa172a8f8c96ea96d
[20]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.svg_save_options#a5f44e6e886da97ae077c60453ed79ce2
[21]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[22]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.svg_save_options
[23]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.svg_save_options
[24]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.svg_save_options#a5f44e6e886da97ae077c60453ed79ce2
[25]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a6383c010776212483f51cc41235924db
[26]: https://purchase.aspose.com/temporary-license
[27]: https://docs.aspose.com/pdf/cpp/developer-guide/
[28]: https://blog.aspose.com/2019/11/05/convert-pdf-to-doc-and-docx-in-c/





