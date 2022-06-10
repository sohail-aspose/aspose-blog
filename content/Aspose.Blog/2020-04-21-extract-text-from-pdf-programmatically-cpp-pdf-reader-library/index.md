---
title: 'Extract Text from PDF Documents Programmatically using C++'
seoTitle: "Extract Text from PDF in C++ | C++ PDF Reader and Text Extractor Library"
description: "C++ library to extract text from PDF documents programmatically in C++. Read PDF files using C++ PDF reader and extractor library. Parse PDF files in C++."
date: Tue, 21 Apr 2020 12:01:56 +0000
draft: false
url: /2020/04/21/extract-text-from-pdf-programmatically-cpp-pdf-reader-library/
author: Usman Aziz
summary: ''
tags: ['CPP PDF Reader Library', 'CPP PDF Text Extractor Library', 'Extract Text from PDF using Cpp', 'Read PDF Files in CPP']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Extract-Text-From-PDF-C.jpg" alt="Extract Text From PDF C++">}}


Text extraction from documents (PDF, word processing, web pages, etc.) has a variety of use cases in the world of digital information. For example, it can be used for parsing documents, performing text analysis, information retrieval, storing documents' content into databases, and so on. If we narrow it down, PDF is one of the most widely used document formats to keep and share digital information. This popularity makes PDF documents a huge source of information. Therefore, parsing or extracting text from PDF documents could possibly be involved in a number of text analysis scenarios.

In order to automate the PDF parsing in C++ applications, this article demonstrates how to **extract text from PDF** documents using **C++**. It covers the following text extraction scenarios:

*   Extract text from a PDF document using C++.
*   Extract text from particular pages in a PDF document using C++.
*   Page by page text extraction from a PDF document using C++.

## C++ PDF Reader and Text Extractor Library

For extracting text from PDF documents, we'll be using [Aspose.PDF for C++][1] which is a powerful PDF library for creating, converting and parsing PDF documents. You can download the library files as well as the running code samples from the [Downloads][2] section.

## Extract Text from PDF using C++

_Aspose.PDF for C++_ lets you parse the PDF documents in a few simple steps. The following is the recipe for extracting text from a PDF document.

*   Create an object of the [PdfExtractor][3] class.
*   Load the PDF document using [PdfExtractor->BindPdf()][4] function.
*   Extract the text from PDF document to [PdfExtractor][5] using [PdfExtractor->ExtractText()][6] function.
*   Save the extracted text into a _MemoryStream_ object.
*   Read the text as string from _MemoryStream_.

The following code sample shows how to extract text from a PDF using C++.

{{< gist aspose-com-gists ce355c98742d47fd3d575d713c1b4f72 "extract-text-from-pdf.cpp" >}}

## Extract Text from Particular Pages in PDF using C++

There could be the case when you need to extract text from a few pages of PDF only. For such a case, you can specify a range of the pages in PDF by setting starting and ending page numbers. The following are the steps to extract text from particular pages in a PDF document.

*   Create an object of the [PdfExtractor][7] class.
*   Load the PDF document using [PdfExtractor->BindPdf()][8] function.
*   Set the starting and ending page number using [PdfExtractor->set\_StartPage()][9] and [PdfExtractor->set\_EndPage()][10] functions respectively.
*   Extract the text from PDF using [PdfExtractor->ExtractText()][11] function.
*   Save the extracted text into a _MemoryStream_ object.
*   Read the text as string from _MemoryStream_.

The following code sample shows how to extract text from particular pages of PDF in C++.

{{< gist aspose-com-gists ce355c98742d47fd3d575d713c1b4f72 "extract-text-from-pdf-page-range.cpp" >}}

## Extract Page by Page Text from PDF in C++

Instead of extracting all the text from a PDF document, you can extract text from every page of the document separately. The following are the steps to perform the page by page text extraction from PDF.

*   Create an object of the [PdfExtractor][12] class.
*   Load the PDF document using [PdfExtractor->BindPdf()][13] function.
*   Call [PdfExtractor->ExtractText()][14] function to retreive text from PDF document to _PdfExtractor_.
*   Loop through every page using [PdfExtractor->HasNextPageText()][15] function.
*   Extract text into memory stream using [PdfExtractor->GetNextPageText()][16] function.
*   Read text from the memory stream.

The following code sample shows how to extract text page by page from PDF in C++.

{{< gist aspose-com-gists ce355c98742d47fd3d575d713c1b4f72 "extract-text-from-pdf-page-by-page.cpp" >}}

## Learn more about Aspose.PDF for C++

You can explore more about _Aspose.PDF for C++_ using the [documentation][17].

## See also

*   [Create PDF Files Programmatically in C++][18]




[1]: https://products.aspose.com/pdf/cpp
[2]: https://downloads.aspose.com/pdf/cpp
[3]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_extractor/
[4]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_extractor/#ad5ff770378271c85191b2f303d6b99e0
[5]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_extractor/
[6]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_extractor#a6fdbb522ebb2e4af3c5bf8ac83ce3eb3
[7]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_extractor/
[8]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_extractor/#ad5ff770378271c85191b2f303d6b99e0
[9]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_extractor/#acc2bcc77fc3e7be8d369d38b340e0826
[10]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_extractor/#a14868ea6cf51a7920f03e54aea917b33
[11]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_extractor#a6fdbb522ebb2e4af3c5bf8ac83ce3eb3
[12]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_extractor/
[13]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_extractor/#ad5ff770378271c85191b2f303d6b99e0
[14]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_extractor#a6fdbb522ebb2e4af3c5bf8ac83ce3eb3
[15]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_extractor/#a758ae07631ef0682f5153d4b08005595
[16]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_extractor/#aa2e6993533155212fc57f9acc1302cea
[17]: https://docs.aspose.com/display/pdfcpp
[18]: https://blog.aspose.com/2020/03/17/create-pdf-files-in-cpp-using-pdf-api/





