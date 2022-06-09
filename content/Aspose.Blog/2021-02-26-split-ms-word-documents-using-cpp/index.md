---
title: 'Split MS Word Documents using C++'
seoTitle: "Split MS Word Documents using C++ | Split DOCX files"
description: "Split MS Word documents using C++. Split DOCX files by sections, pages, or a range of pages using Aspose.Words for C++ API."
date: Fri, 26 Feb 2021 10:47:31 +0000
draft: false
url: /2021/02/26/split-ms-word-documents-using-cpp/
author: Muhammad Ahmad
summary: 'MS Word is a popular format for storing and sharing information. There might be scenarios where you want to split a Word document into multiple files. For example, a document may contain different sections that need to be shared with different people or contain some confidential information that needs to be separated. In such cases, splitting the Word document proves to be helpful. In this article, you will learn **how to split MS Word documents using C++**.'
tags: ['C++ split word documents', 'C++ word document splitter', 'Split word documents C++']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Split-Word-Documents.jpg" alt="Split Word Documents C++">}}


MS Word is a popular format for storing and sharing information. There might be scenarios where you want to split a Word document into multiple files. For example, a document may contain different sections that need to be shared with different people or contain some confidential information that needs to be separated. In such cases, splitting the Word document proves to be helpful. In this article, you will learn **how to split MS Word documents using C++**.

*   [C++ API for Splitting Word Documents][1]
*   [Split Word Documents by Page using C++][2]
*   [Use Page Range to Split a Word Document][3]
*   [Split Word Document by Sections using C++][4]
*   [Get a Free License][5]

## C++ API for Splitting Word Documents {#CPP-API-for-Splitting-Word-Documents}

[Aspose.Words for C++][6] is a native C++ library that allows you to generate, change and convert Microsoft Word documents. In addition, it also supports splitting Word documents into multiple files. You can either install the API through [NuGet][7] or download it directly from the [Downloads][8] section.

```
PM> Install-Package Aspose.Words.Cpp
```

## Split Word Documents by Page using C++ {#Split-Word-Documents-by-Page-using-CPP}

The following are the steps to split Word files using C++.

*   Load the Word document using the [Document][9] class.
*   Create an instance of the DocumentPageSplitter class and initialize it with the [Document][10] object created in the previous step.
*   Loop through the pages of the [Document][11].
*   Extract each page with DocumentPageSplitter.GetDocumentOfPage(int32\_t PageIndex) method.
*   Save the documents using the [Document->Save (System::String fileName)][12] method.

The following is the sample code to split a Word document by page.

{{< gist aspose-com-gists e1805dc8ef1cfc13daa4b8fcd5d392e2 "Split-Word-Documents-By-Page.cpp" >}}

## Use Page Range to Split a Word Document {#Use-Page-Range-to-Split-a-Word-Document}

Instead of separating each and every page, you can also split the Word document by providing a page range. The following are the steps to split a Word document using page range.

*   Firstly, load the Word document using the [Document][13] class.
*   Create an instance of the DocumentPageSplitter class and initialize it with the previous step's [Document][14] object.
*   Retrieve the pages in the required range using the DocumentPageSplitter.GetDocumentOfPageRange(int32\_t pageIndex, int32\_t pageIndex) method.
*   Lastly, save the Word document using the [Document->Save (System::String fileName)][15] method.

The following is the sample code to split a Word document using page range.

{{< gist aspose-com-gists e1805dc8ef1cfc13daa4b8fcd5d392e2 "Split-Word-Documents-By-Page-Range.cpp" >}}

## Split Word Document by Sections using C++ {#Split-Word-Document-by-Sections-using-CPP}

Word files can contain one or more sections that might have different formatting and may consist of any number of pages. To add a new section in the Word file, use the _Layout>Breaks>Section Breaks_ option. The following are the steps to split Word files by sections using Aspose.Words for C++ API.

*   Load the Word file using the  [Document][16] class.
*   Retrieve the sections of the document using the [Document->get\_Sections()][17] method and iterate over them.
*   Clone the section into a [Section][18] object using the [Document->get\_Sections()->idx\_get(int32\_t index)->Clone()][19] method.
*   Create a new Word document using the [Document][20] class.
*   Add the cloned section to the newly created Word document using [Document->get\_Sections()->Add (System::SharedPtr<Aspose::Words::Node> node)][21] method.
*   Finally, save the Word file using the [Document->Save (System::String fileName)][22] method.

The following is the sample code to split Word documents by sections.

{{< gist aspose-com-gists e1805dc8ef1cfc13daa4b8fcd5d392e2 "Split-Word-Documents-By-Section.cpp" >}}

## Get a Free License {#Get-a-Free-License}

You can try the API without evaluation limitations by requesting [a free temporary license][23].

## Conclusion

In this article, you have learned how to split Word documents into multiple files using C++. You have learned how to use Aspose.Words for C++ API to split word documents by page, page range, and sections. You can explore the API in detail by using the [official documentation][24]. If you have any questions, please feel free to contact us on the [forum][25].

## See Also

*   [Merge MS Word Documents using C++][26]




[1]: #CPP-API-for-Splitting-Word-Documents
[2]: #Split-Word-Documents-by-Page-using-CPP
[3]: #Use-Page-Range-to-Split-a-Word-Document
[4]: #Split-Word-Document-by-Sections-using-CPP
[5]: #Get-a-Free-License
[6]: https://products.aspose.com/words/cpp
[7]: https://www.nuget.org/packages/Aspose.Words.Cpp
[8]: https://downloads.aspose.com/words/cpp
[9]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[10]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[11]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[12]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a4ba337135cd6c8bed74a268ba60218bd
[13]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[14]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[15]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a4ba337135cd6c8bed74a268ba60218bd
[16]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[17]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#ab9f72b25508f474a5ff2d9fd35287e6a
[18]: https://apireference.aspose.com/words/cpp/class/aspose.words.section
[19]: https://apireference.aspose.com/words/cpp/class/aspose.words.section#ae0079b76c5fd99ea809988089877e3c4
[20]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[21]: https://apireference.aspose.com/words/cpp/class/aspose.words.node_collection#a404c14dde05211ac3c990fbbbe503b74
[22]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a4ba337135cd6c8bed74a268ba60218bd
[23]: https://purchase.aspose.com/temporary-license
[24]: https://docs.aspose.com/words/cpp/
[25]: https://forum.aspose.com/c/words/8
[26]: https://blog.aspose.com/2021/02/23/merge-ms-word-documents-using-cpp/





