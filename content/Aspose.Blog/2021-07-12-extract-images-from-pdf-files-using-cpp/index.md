---
title: 'Extract Images from PDF Files using C++'
seoTitle: "Extract Images from PDF Files using C++ | Parse PDF Files using C++"
description: "Learn how to extract images from PDF files using the robust and feature-rich Aspose.PDF for C++ API within your C++ applications."
date: Mon, 12 Jul 2021 18:42:20 +0000
draft: false
url: /2021/07/12/extract-images-from-pdf-files-using-cpp/
author: Muhammad Ahmad
summary: '[PDF][1] is a popular format for sharing information over the internet. Most of the time, PDF files contain images along with text and other elements. There might be scenarios where you need to extract these images from PDF files to process them further. To that end, this article will teach you **how to extract images from PDF files using C++**.'
tags: ['C++ Extract PDF Images', 'Extract Images from PDF Files using C++']
categories: ['Aspose.PDF Product Family']
---

[PDF][2] is a popular format for sharing information over the internet. Most of the time, PDF files contain images along with text and other elements. There might be scenarios where you need to extract these images from PDF files to process them further. To that end, this article will teach you **how to extract images from PDF files using C++**.

*   [C++ API for Extracting Images from PDF Files][3]
*   [Extracting Images from PDF Files using C++][4]

## C++ API for Extracting Images from PDF Files {#CPP-API-for-Extracting-Images-from-PDF-Files}

[Aspose.PDF for C++][5] is a C++ library that allows you to create, read and modify PDF documents. Furthermore, the API supports extracting images from PDF files. You can either install the API through [NuGet][6] or download it directly from the [downloads][7] section.

```
PM> Install-Package Aspose.PDF.Cpp
```

## Extract Images from PDF Files using C++ {#Extract-Images-from-PDF-Files-using-CPP}

The following are the steps to extract images from a PDF file.

*   Load the PDF document using the [Document][8] class.
*   Get the pages of the document using the [Document->get\_Pages()][9] method and iterate over them.
*   Get images for each page using the page->get\_Resources()->get\_Images() method and iterate over them.
*   Create a [FileStream][10] object for each image and save it as JPEG, PNG, etc.

The following sample code demonstrates how to extract images from a PDF file using C++.

{{< gist aspose-com-gists 1bca97ec93cc6a52525c2e735da5b3f3 "Extract_Images_From_PDF_Files.cpp" >}}

## Get a Free License

You can try the API without evaluation limitations by requesting [a free temporary license][11].

## Conclusion

In this article, you have learned how to extract images from PDF files using C++. We used the robust and easy-to-use Aspose.PDF for C++ API to achieve this. The API provides a bunch of additional features for working with PDF files that you can explore in detail by visiting the [official documentation][12]. If you have any questions regarding any aspect of the API, please feel free to reach us at our [free support forum][13].

## **See Also**

*   [Create, Fill, or Edit Fillable PDF Forms with C++][14]
*   [Rotate PDF Pages, Text or Images using C++][15]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #CPP-API-for-Extracting-Images-from-PDF-Files
[4]: #Extract-Images-from-PDF-Files-using-CPP
[5]: https://products.aspose.com/pdf/cpp
[6]: https://www.nuget.org/packages/Aspose.Pdf.cpp
[7]: https://downloads.aspose.com/pdf/cpp
[8]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[9]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a481178a0c2c6277ae9b6b931d63e4122
[10]: https://apireference.aspose.com/pdf/cpp/class/system.i_o.file_stream
[11]: https://purchase.aspose.com/temporary-license
[12]: https://docs.aspose.com/pdf/cpp/
[13]: https://forum.aspose.com/c/pdf/10
[14]: https://blog.aspose.com/2021/06/18/create-fill-or-edit-fillable-pdf-forms-with-cpp/
[15]: https://blog.aspose.com/2021/05/31/rotate-pdf-pages-text-or-image-using-cpp/





