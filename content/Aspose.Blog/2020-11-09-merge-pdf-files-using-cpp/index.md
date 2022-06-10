---
title: 'Merge Two or More PDF Files using C++'
seoTitle: "Merge PDF Files in C++ | Combine Two or More PDF Files | C++ PDF API"
description: "Use C++ PDF API to merge two or more PDF files into single file using C++. Complete tutorial with API references, source code and API's download link."
date: Mon, 09 Nov 2020 18:13:04 +0000
draft: false
url: /2020/11/09/merge-pdf-files-using-cpp/
author: Usman Aziz
summary: 'In various scenarios, you may need to merge multiple PDF files into a single one. For example, merging the content from a similar type of documents such as resumes, receipts, and etc. [Aspose.PDF][1] lets you automate the PDF merging process from within your web, desktop, or mobile applications. In this article, you are going to learn **how to merge multiple PDF files using the C++** variant of Aspose.PDF.'
tags: ['combine two or more pdf in cpp', 'concatenate pdf files in cpp', 'merge pdf files in cpp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Merge-PDF-Files-into-Single-PDF.jpg" alt="merge pdf files in c++">}}


In various scenarios, you may need to merge multiple PDF files into a single one. For example, merging the content from a similar type of documents such as resumes, receipts, and etc. [Aspose.PDF][2] lets you automate the PDF merging process from within your web, desktop, or mobile applications. In this article, you are going to learn **how to merge multiple PDF files using the C++** variant of Aspose.PDF.

*   [C++ PDF Merger API - Free Download][3]
*   [Steps to Merge PDF Files][4]
*   [Merge Two PDF Files using C++][5]

## C++ PDF Merger API - Free Download {#C++-PDF-Merge-API-Free-Download}

[Aspose.PDF for C++][6] is a feature-rich PDF manipulation API that lets you create and process PDF files seamlessly. The API's PDF merging feature allows you to combine two or more PDF files within a few lines of code. You can either [download][7] the API's package or get it installed using [NuGet][8].

```
Install-Package Aspose.PDF.Cpp
```

## Steps to Merge PDF Files {#Steps-to-Merge-PDF-Files}

Before jumping to the code, let's first have a look at what are the basic steps needed to merge PDF files.

*   Load the source and target PDF files.
*   Fetch the pages from the source PDF file.
*   Add fetched pages to the target PDF file.
*   Save the target PDF file.

Now, let's transform these steps into C++ coding instructions using Aspose.PDF for C++.

## Merge Two PDF Files using C++ {#Merge-two-PDF-Files-using-C++}

The following are the steps along with the API references of the classes and methods used to merge PDF files.

*   Create an object of [Document][9] class to load the first PDF file.
*   Repeat the first step to load the second PDF file.
*   Access the [PageCollection][10] of the second document using [doc2->get\_Pages()][11] method.
*   Add fetched pages to the first document using [doc1->get\_Pages()->Add(PageCollection)][12].
*   Save the first document using [doc1->Save(String)][13] method.

The following code sample shows how to merge two PDF files.

{{< gist aspose-com-gists 15c849f880fecfcf8000d447b4e3cb17 "merge-pdf-files.cpp" >}}

## Conclusion

In this article, you have seen how to merge two or more PDF documents using C++. You can implement this feature in your C++ based applications in order to automate the PDF merging. Explore more about the C++ PDF API using the [documentation][14].

## See Also

*   [Create PDF Files from Scratch using C++][15]




[1]: https://products.aspose.com/pdf
[2]: https://products.aspose.com/pdf
[3]: #C++-PDF-Merge-API-Free-Download
[4]: #Steps-to-Merge-PDF-Files
[5]: #Merge-two-PDF-Files-using-C++
[6]: https://products.aspose.com/pdf/cpp
[7]: https://downloads.aspose.com/pdf/cpp
[8]: https://www.nuget.org/packages/Aspose.pdf.cpp
[9]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[10]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.page_collection
[11]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a481178a0c2c6277ae9b6b931d63e4122
[12]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.page_collection#a581b0054d03d1e10363e7ee093eea053
[13]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a5f0d3a0eaf87e479ae2bf52f7eb438d7
[14]: https://docs.aspose.com/pdf/cpp/developer-guide/
[15]: https://blog.aspose.com/2020/03/17/create-pdf-files-in-cpp-using-pdf-api/





