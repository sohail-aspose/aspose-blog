---
title: 'C++ PDF Library - Create PDF Files Programmatically in C++'
seoTitle: ""
description: ""
date: Tue, 17 Mar 2020 17:01:35 +0000
draft: false
url: /2020/03/17/create-pdf-files-in-cpp-using-pdf-api/
author: Usman Aziz
summary: ''
tags: ['Aspose.PDF for Cpp', 'Cpp PDF API', 'Create PDF files in Cpp', 'Create PDFs Dynamically']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/PDF-Automation-C.png" alt="">}}


With the power of the Internet, everything has gone digital and paperless systems have become popular. The digital documents, i.e. PDF, are among the building blocks of paperless systems that have made life easier by providing automated generation and processing features. Most of the businesses use **PDF document automation** for generating reports, receipts, invoices, and other business documents dynamically. Therefore, in this article, I'll demonstrate how to integrate the features of **PDF automation in C++** based applications and **generate PDF files using C++**.

## C++ PDF Library

For creating PDF files, we'll use [Aspose.PDF for C++][1] API which is a native C++ library to work with PDF documents programmatically. It allows you to create interactive PDF documents with the support of a variety of PDF elements. _Aspose.PDF for C++_ is available on NuGet as well as in the [Downloads][2] section of Aspose.

## Create a PDF File in C++

First of all, we will create a simple PDF file and add some text to the first page in the form of a paragraph. The following are the steps to be followed:

*   Create a [Document][3] object.
*   Add a page to [PageCollection][4] of the _Document_.
*   Get the paragraph of the page.
*   Create a [TextFragment][5] object and add it to the paragraph.
*   Save the PDF document.

The following code sample shows how to create a PDF document in C++.

{{< gist aspose-com-gists a9295f23ab5d78063e3d162fe39bdbfd "create-pdf-in-cpp.cpp" >}}

### Output



{{< figure align=center src="images/Create-PDF-in-C-1.png" alt="Create PDF Files in C++">}}


## Create a PDF File using TextBuilder in C++

In this section, I'll show you how to use the [TextBuilder][6] class to append various text fragments and paragraphs on the page. Furthermore, in this example, you will learn how to set the position of the text fragment on the page. The following are the steps to perform this operation:

*   Create a _Document_ object.
*   Add a page to the document.
*   Create a [TextBuilder][7] object.
*   Create a _TextFragment_ and add its text.
*   Set the position of the _TextFragment_.
*   Append _TextFragment_ using the _TextBuilder_.
*   Save PDF document.

The following code sample shows how to create a PDF using _TextBuilder_ in C++.

{{< gist aspose-com-gists a9295f23ab5d78063e3d162fe39bdbfd "create-pdf-in-cpp-textbuilder.cpp" >}}

### Output



{{< figure align=center src="images/Create-PDF-in-C-2.png" alt="C++ PDF API">}}


## Create a PDF File with Image in C++

You can also create and add images to the PDF documents using _Aspose.PDF for C++_. The following are the steps to perform this operation:

*   Create a _Document_ object.
*   Add a page to the document.
*   Create an image to be added.
*   Add the image to the PDF file.
*   Save PDF file.

The following code sample shows how to create and add an image to a PDF document in C++.

{{< gist aspose-com-gists a9295f23ab5d78063e3d162fe39bdbfd "create-pdf-in-cpp-image.cpp" >}}

### Output



{{< figure align=center src="images/Create-PDF-in-C-3.png" alt="C++ PDF Library ">}}


## Create a PDF File with Attachments in C++

The PDF format also allows adding attachments to the document. There is a variety of file formats that can be added as an attachment to the PDF file. The following are the steps to embed a file in PDF using _Aspose.PDF for C++_:

*   Load a file to be attached in _SharedPtr<FileSpecification>_.
*   Create an object of _Document_ class.
*   Embed the file to the Document.
*   Save the PDF file.

The following code sample shows how to add an attachment to the PDF document in C++.

{{< gist aspose-com-gists a9295f23ab5d78063e3d162fe39bdbfd "create-pdf-in-cpp-attachment.cpp" >}}

### Output



{{< figure align=center src="images/Create-PDF-in-C-4.png" alt="Generate PDF in C++">}}


## Learn more about Aspose.PDF for C++

You can learn more about _Aspose.PDF for C++_ from the [documentation][8] and source code [examples][9].

## See Also

*   [Convert Word DOC or DOCX to PDF in C++][10]




[1]: https://products.aspose.com/pdf/cpp
[2]: https://downloads.aspose.com/pdf/cpp
[3]: https://apireference.aspose.com/cpp/pdf/class/aspose.pdf.document/
[4]: https://apireference.aspose.com/cpp/pdf/class/aspose.pdf.page_collection/
[5]: https://apireference.aspose.com/cpp/pdf/class/aspose.pdf.text.text_fragment/
[6]: https://apireference.aspose.com/cpp/pdf/class/aspose.pdf.text.text_builder/
[7]: https://apireference.aspose.com/cpp/pdf/class/aspose.pdf.text.text_builder/
[8]: https://docs.aspose.com/
[9]: https://github.com/aspose-pdf/Aspose.PDF-for-C/
[10]: https://blog.aspose.com/2020/04/10/convert-word-doc-or-docx-to-pdf-in-cpp/





