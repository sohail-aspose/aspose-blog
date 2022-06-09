---
title: 'Convert RTF Documents to PDF using C++'
seoTitle: "RTF to PDF C++ Conversion | Convert RTF Documents to PDF using C++"
description: "Convert RTF documents to PDF format using C++. Step by step guide to perform RTF to PDF conversion within your C++ applications."
date: Wed, 17 Feb 2021 19:32:28 +0000
draft: false
url: /2021/02/17/convert-rtf-documents-to-pdf-using-cpp/
author: Muhammad Ahmad
summary: '[RTF][1] is a cross-platform rich text file format introduced by Microsoft. In addition to text, it can include extra information about font style, formatting, images, etc. There might be situations such as sharing the file over the internet where you do not want the file to be editable or want the file to have a fixed layout. In such cases, [PDF][2] format is your best bet. PDF is a cross-platform format that can be secured and made read-only. Furthermore, the PDF file looks the same wherever you open it. In this article, you will learn **how to convert RTF files to PDF format using C++**.'
tags: ['C++ Convert RTF to PDF', 'Convert RTF to PDF C++', 'convert rtf to pdf']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/RTF-to-PDF-1024x361.jpg" alt="RTF to PDF C++">}}


[RTF][3] is a cross-platform rich text file format introduced by Microsoft. In addition to text, it can include extra information about font style, formatting, images, etc. There might be situations such as sharing the file over the internet where you do not want the file to be editable or want the file to have a fixed layout. In such cases, [PDF][4] format is your best bet. PDF is a cross-platform format that can be secured and made read-only. Furthermore, the PDF file looks the same wherever you open it. In this article, you will learn **how to convert RTF files to PDF format using C++**.

*   [RTF to PDF Conversion API][5]
*   [RTF to PDF Conversion Steps][6]
*   [Get a Free License][7]

## RTF to PDF C++ Conversion API

We will use the [Aspose.Words for C++][8] API to convert RTF documents to PDF format. It is a native C++ library that allows you to generate, alter and convert Microsoft Word files. Furthermore, it also supports converting files to PDF format. You can either install the API through [NuGet][9] or download it directly from the [Downloads][10] section.

```
PM> Install-Package Aspose.Words.Cpp
```

## C++ RTF to PDF Conversion {#CPP-RTF-to-PDF-Conversion}

The following are the steps to convert RTF documents to PDF format.

*   Load the RTF document using the [Document(System::String fileName)][11] constructor of the [Document][12] class.
*   Save the RTF file as PDF using the [Document->Save(System::String fileName, Aspose::Words::SaveFormat saveFormat)][13] method.

The following is the code sample for converting RTF documents to PDF format.

{{< gist aspose-com-gists 50202f13b147b72b23d1b60d67e661da "Convert-RTF-to-PDF.cpp" >}}

## Get a Free License {#Get-a-Free-License}

You can try the API without evaluation limitations by requesting [a free temporary license][14].

## Conclusion

In this article, you have learned how to convert RTF documents to PDF format programmatically using C++. In order to perform this conversion, we have used Aspose.Words for C++, which is a feature-rich API that lets you automate workflows related to MS Word. You can explore the API in detail by using the [official documentation][15].

## See Also

*   [Create MS Word Documents (DOC/DOCX) using C++][16]
*   [Protect or Unprotect Word Documents using C++][17]




[1]: https://docs.fileformat.com/word-processing/rtf/
[2]: https://docs.fileformat.com/pdf/
[3]: https://docs.fileformat.com/word-processing/rtf/
[4]: https://docs.fileformat.com/pdf/
[5]: #RTF-to-PDF-CPP-Conversion-API
[6]: #CPP-RTF-to-PDF-Conversion
[7]: #Get-a-Free-License
[8]: https://products.aspose.com/words/cpp
[9]: https://www.nuget.org/packages/Aspose.Words.Cpp
[10]: https://downloads.aspose.com/words/cpp
[11]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#af5050c6752e758595da945e4de05804c
[12]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[13]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a1355bc15bd6da23c7bf65f3fcf0fb050
[14]: https://purchase.aspose.com/temporary-license
[15]: https://docs.aspose.com/words/cpp/
[16]: https://blog.aspose.com/2020/08/25/create-ms-word-documents-using-cpp/
[17]: https://blog.aspose.com/2021/01/05/protect-or-unprotect-word-documents-using-cpp/





