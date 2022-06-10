---
title: 'Split MS Word Documents using C#'
seoTitle: "Split Word Documents using C# | Split Document by Page, Section, Range"
description: "Split MS Word documents into multiple documents using C#. Split a Word document (DOC/DOCX) by sections, pages or range of pages using C# or VB.NET."
date: Wed, 26 Aug 2020 22:11:55 +0000
draft: false
url: /2020/08/26/split-ms-word-documents-using-csharp/
author: Usman Aziz
summary: ''
tags: ['split word document by page csharp', 'split word document by section csharp', 'split word document csharp']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Split-Word-Documents.jpg" alt="Split Word Documents">}}


MS Word documents are widely used to keep and share information. In some cases, you may need to split the data from a Word document that could be located in different sections or pages. Also, you may need to split the pages of a single document into multiple documents. In accordance with such scenarios, this article aims to show you **how to split MS Word documents programmatically using C#**.

*   [C# API to Split MS Word Documents][1]
*   [Split Word Documents by Section using C#][2]
*   [Split Word Documents Page by Page using C#][3]
*   [Use a Page Range to Split Word Documents using C#][4]

## C# API to Split MS Word Documents {#CSharp-API-to-Split-MS-Word-Documents}

[Aspose.Words for .NET][5] is a powerful word processing API that lets you create and manipulate MS Word documents using C# or VB.NET. Along with that, it also allows you to split MS Word documents by section, page, or page range. You can [download][6] the API or install it within your application using [NuGet][7].

```
PM> Install-Package Aspose.Words
```

## Split Word Documents by Section using C# {#Split-Word-Documents-by-Section-using-CSharp}

Sections refer to the parts of a document where different formatting can be applied. A section may be composed of a single page, a range of pages, or the whole document. The section breaks are used to split a document into multiple sections. The following are the steps to split a Word document based on its sections using Aspose.Words for .NET.

*   Load the Word document using the [Document][8] class.
*   Loop through the page sections using [Document.Sections][9] property.
*   Clone the section into a new [Section][10] object.
*   Create a new [Document][11] object.
*   Add the section into new [Document][12] using [Document.Sections.Add(Section)][13] method.
*   Save the documents using [Document.Save(String)][14] method.

The following code sample shows how to split MS Word documents by sections using C#.

{{< gist aspose-com-gists c7cafec957d110f5c10270d77195a36b "split-word-document-section.cs" >}}

## Split Word Documents Page by Page using C# {#Split-Word-Documents-Page-by-Page-using-CSharp}

There might be the case when a Word document contains a similar type of information on each page such as invoices or receipts. In such a case, you can split the document's pages in order to save each invoice as a separate document. For splitting the documents page by page, you can use the helper class DocumentPageSplitter based on Aspose.Words for .NET. You can simply copy the class within your project and split the Word documents page by page by following the below steps.

*   Load the Word document using [Document][15] class.
*   Create an object of DocumentPageSplitter class and initialize it with the _Document_ object.
*   Iterate through the document's pages.
*   Extract each page into a new _Document_ object using DocumentPageSplitter.GetDocumentOfPage(int PageIndex) method.
*   Save each document using [Document.Save(String)][16] method.

The following code sample shows how to split the Word document by pages using C#.

{{< gist aspose-com-gists c7cafec957d110f5c10270d77195a36b "split-word-document-page.cs" >}}

## Split Word Documents by Page Range using C# {#Split-Word-Documents-by-Page-Range-using-CSharp}

You can also specify a page range to split it from the original document using DocumentPageSplitter class. For example, if you need to split the pages from 2 to 4, just specify the starting and ending page's index in DocumentPageSplitter.GetDocumentOfPageRange(int StartIndex, int EndIndex) method.

The following code sample shows how to split a page range from Word document using C#.

{{< gist aspose-com-gists c7cafec957d110f5c10270d77195a36b "split-word-document-page-range.cs" >}}

## Conclusion

In this article, you have learned how to split MS Word documents programmatically using C#. The scenarios of splitting Word documents by sections, pages, and page ranges have been discussed along with code samples. You can explore more about Aspose.Words for .NET using the [documentation][17].

## See Also

*   [Merge MS Word Documents using C#][18]




[1]: #CSharp-API-to-Split-MS-Word-Documents
[2]: #Split-Word-Documents-by-Section-using-CSharp
[3]: #Split-Word-Documents-Page-by-Page-using-CSharp
[4]: #Split-Word-Documents-by-Page-Range-using-CSharp
[5]: https://products.aspose.com/words/net
[6]: https://downloads.aspose.com/words/net
[7]: https://nuget.org/packages/Aspose.Words
[8]: https://apireference.aspose.com/words/net/aspose.words/document
[9]: https://apireference.aspose.com/words/net/aspose.words/document/properties/sections
[10]: https://apireference.aspose.com/words/net/aspose.words/section
[11]: https://apireference.aspose.com/words/net/aspose.words/document
[12]: https://apireference.aspose.com/words/net/aspose.words/document
[13]: https://apireference.aspose.com/words/net/aspose.words/nodecollection/methods/add
[14]: https://apireference.aspose.com/words/net/aspose.words.document/save/methods/2
[15]: https://apireference.aspose.com/words/net/aspose.words/document
[16]: https://apireference.aspose.com/words/net/aspose.words.document/save/methods/2
[17]: https://docs.aspose.com/words/net/getting-started/
[18]: https://blog.aspose.com/2020/07/07/merge-ms-word-documents-using-csharp-asp.net-core/





