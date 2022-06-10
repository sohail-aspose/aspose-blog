---
title: 'Split a PDF File into Multiple Files using C#'
seoTitle: "Split PDF into Multiple Files using C# | .NET PDF Splitter Library"
description: "Split a PDF file into multiple files using C#. Split each page or a collection of pages in PDF to separate files in C#. Download PDF splitter API for free."
date: Tue, 03 Nov 2020 23:40:33 +0000
draft: false
url: /2020/11/03/split-pdf-into-multiple-files-using-csharp/
author: Usman Aziz
summary: 'In the [previous article][1], you have seen how to merge multiple PDF files into a single PDF. However, there could be a case when you need to split a single PDF file into multiple files. You can either split each page of the PDF or a collection of pages into multiple PDFs. In this article, you will learn how to cope up with such scenarios and **split a PDF file into multiple PDFs using C#**.'
tags: ['csharp pdf splitter library', 'split pages in pdf using csharp', 'split pdf files csharp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Split-PDF-Files.jpg" alt="Split a PDF File into Multiple Files using C#">}}


In the [previous article][2], you have seen how to merge multiple PDF files into a single PDF. However, there could be a case when you need to split a single PDF file into multiple files. You can either split each page of the PDF or a collection of pages into multiple PDFs. In this article, you will learn how to cope up with such scenarios and **split a PDF file using C#**.

*   [C# API to Split PDF - Free Download][3]
*   [Split a PDF File by Pages][4]
*   [Select Pages to Split a PDF File][5]

## Split PDF C# API - Free Download {#CSharp-API-to-Split-PDF-Free-Download}

[Aspose.PDF for .NET][6] is a powerful PDF file manipulation API that lets you create, edit, and process PDF documents from within your .NET applications. In addition, the API allows you to split a single PDF into multiple files with high fidelity. You can [download][7] the API's DLL or get it installed using [NuGet][8].

```
PM> Install-Package Aspose.Pdf
```

## Split a PDF File using C# {#Split-a-PDF-File-using-CSharp}

The PDF splitting criteria can vary as per your requirements. You can either split the document by each page or a collection of pages. First, let's see how to split every page of a PDF file.

*   Load the PDF document using [Document][9] class.
*   Loop through the [Document.Pages][10] collection to access each page using [Page][11] class.
*   In every iteration, create a new [Document][12], add the current page to the document and save it as a PDF file using [Document.Save(String)][13] method.

The following code sample shows how to split a PDF document using C#.

{{< gist aspose-com-gists 4a65283c94c4ab99a1cd65ddf247df2c "split-pdf.cs" >}}

## Split Selected Pages of PDF using C# {#Split-Selected-Pages-of-PDF-using-CSharp}

You can also split the PDF by specifying the range of pages. For example, you can split the first or last N number pages, the even or odd pages, and etc. For the demonstration, the following are the steps to split even and odd pages from the PDF.

*   Load the PDF document using [Document][14] class.
*   Get the pages to be split into a [Page\[\]][15] array.
*   Create a new [Document][16] and add pages to it using [Document.Pages.Add(Page\[\])][17] method.
*   Save the PDF file using the [Document.Save(String)][18] method.

The following code sample shows how to split a collection of pages from PDF.

{{< gist aspose-com-gists 4a65283c94c4ab99a1cd65ddf247df2c "split-pdf-multiple-pages.cs" >}}

## Conclusion

In this article, you have learned how to split the PDF files using C#. The code samples demonstrated how to split every page or a collection of pages in a PDF to separate files. You can explore more about the .NET PDF API using the [documentation][19].

## See Also

*   [Merge PDF Files using C#][20]




[1]: https://blog.aspose.com/2020/01/16/merge-multiple-pdf-files-in-csharp-net/
[2]: https://blog.aspose.com/2020/01/16/merge-multiple-pdf-files-in-csharp-net/
[3]: #CSharp-API-to-Split-PDF-Free-Download
[4]: #Split-a-PDF-File-using-CSharp
[5]: #Split-Selected-Pages-of-PDF-using-CSharp
[6]: https://products.aspose.com/pdf/net
[7]: https://downloads.aspose.com/pdf/net
[8]: http://nuget.org/packages/Aspose.Pdf
[9]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/pages
[11]: https://apireference.aspose.com/pdf/net/aspose.pdf/page
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf/page
[16]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[17]: https://apireference.aspose.com/pdf/net/aspose.pdf.pagecollection/add/methods/2
[18]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[19]: https://docs.aspose.com/pdf/net
[20]: https://blog.aspose.com/2020/01/16/merge-multiple-pdf-files-in-csharp-net/





