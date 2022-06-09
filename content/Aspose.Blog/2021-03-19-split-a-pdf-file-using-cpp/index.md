---
title: 'Split a PDF File using C++'
seoTitle: "Split a PDF File using C++ | Use custom criteria to split PDF files"
description: "Split a PDF file into multiple files using C++. Use custom criteria for splitting PDF files within your C++ applications."
date: Fri, 19 Mar 2021 12:40:16 +0000
draft: false
url: /2021/03/19/split-a-pdf-file-using-cpp/
author: Muhammad Ahmad
summary: '[PDF][1] is a standard format for sharing documents over the internet. Its global support and consistent layout make it an ideal choice for such scenarios. But there may be situations where sharing the complete PDF file is not an ideal or appropriate option. For such cases, you can split the PDF file according to your requirements. You can do this manually, but that might prove to be less efficient and time-consuming. Alternatively, you can split the PDF document programmatically. In this article, you will learn **how to split PDF files using C++**.'
tags: ['C++ Split PDF File using Custom Criteria', 'C++ Split PDF Files', 'Split PDF Files By Page', 'Split PDF files using C++']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Split-PDF-Files.jpg" alt="Split PDF files using C++">}}


[PDF][2] is a standard format for sharing documents over the internet. Its global support and consistent layout make it an ideal choice for such scenarios. But there may be situations where sharing the complete PDF file is not an ideal or appropriate option. For such cases, you can split the PDF file according to your requirements. You can do this manually, but that might prove to be less efficient and time-consuming. Alternatively, you can split the PDF document programmatically. In this article, you will learn **how to split PDF files using [C++][3]**.

*   [C++ API for Splitting PDF Files][4]
*   [Split a PDF File using C++][5]
*   [Split Selected PDF Pages using C++][6]
*   [Get a Free License][7]

## C++ API for Splitting PDF Files {#CPP-API-for-Splitting-PDF-Files}

[Aspose.PDF for C++][8] is a C++ library that allows you to create, read and update PDF documents. Furthermore, the API supports splitting PDF files into multiple documents. You can either install the API through [NuGet][9] or download it directly from the [downloads][10] section.

```
PM> Install-Package Aspose.PDF.Cpp
```

## Split a PDF File using C++ {#Split-a-PDF-File-using-CPP}

Aspose.PDF for C++ lets you save each page of the PDF file as a separate PDF document. The following are the steps to achieve this using C++.

*   Load the source PDF file using the [Document][11] class.
*   Loop through the pages of the source PDF file using the [Document->get\_Pages()][12] method.
*   Within the loop, create an instance of the [](https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document)[Document][13] class to represent the new PDF file.
*   Add the [Page][14] retrieved in the loop to the newly created [](https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document)[Document][15] object.
*   Save the new PDF file using [Document->Save (System::String outputFileName)][16] method.

The following is the sample code to split a PDF file using C++.

{{< gist aspose-com-gists 93276a7077c995408e36ef974aa241d5 "Split-PDF-Document-By-Page.cpp" >}}

## Split Selected PDF Pages using C++ {#Split-Selected-PDF-Pages-using-CPP}

Instead of saving each page separately, you may specify different conditions for splitting the PDF file. The following are the steps to split selected PDF pages using C++.

*   Load the source PDF file using the [](https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document)[Document][17] class.
*   Create an instance of the [](https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document)[Document][18] class to represent the new PDF file.
*   Loop through the pages of the source PDF file using the [Document->get\_Pages()][19] method.
*   Add the desired pages to the newly created [Document][20] object.
*   Save the new PDF file using the [Document->Save (System::String outputFileName)][21] method.

The following is the sample code to split specific PDF pages using C++.

{{< gist aspose-com-gists 93276a7077c995408e36ef974aa241d5 "Split-PDF-Document-With-Specific-Pages.cpp" >}}

## Get a Free License {#Get-a-Free-License}

You can try the API without evaluation limitations by requesting [a free temporary license][22].

## Conclusion

In this article, you have learned how to split PDF files into individual pages using C++. Furthermore, you have learned how to use custom criteria to customize the splitting of PDF files. Aspose.PDF for C++ is a vast library with many additional features for working with PDF files. You can explore the API in detail by using the [official documentation][23]. In case of any questions, please feel free to reach us on our [free support forum][24].

## See Also

*   [Convert PDF to SVG Format using C++][25]
*   [Find and Replace Text in PDF Files using C++][26]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: https://docs.fileformat.com/programming/cpp/
[4]: #CPP-API-for-Splitting-PDF-Files
[5]: #Split-a-PDF-File-using-CPP
[6]: #Split-Selected-PDF-Pages-using-CPP
[7]: #Get-a-Free-License
[8]: https://products.aspose.com/pdf/cpp
[9]: https://www.nuget.org/packages/Aspose.Pdf.cpp
[10]: https://downloads.aspose.com/pdf/cpp
[11]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[12]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a481178a0c2c6277ae9b6b931d63e4122
[13]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[14]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.page
[15]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[16]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a5f0d3a0eaf87e479ae2bf52f7eb438d7
[17]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[18]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[19]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a481178a0c2c6277ae9b6b931d63e4122
[20]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[21]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a5f0d3a0eaf87e479ae2bf52f7eb438d7
[22]: https://purchase.aspose.com/temporary-license
[23]: https://docs.aspose.com/pdf/cpp/
[24]: https://forum.aspose.com/c/pdf/10
[25]: https://blog.aspose.com/2021/02/01/convert-pdf-to-svg-format-using-cpp/
[26]: https://blog.aspose.com/2021/03/11/find-and-replace-text-in-pdf-files-using-cpp/





