---
title: 'Extract Images from PDF using C#'
seoTitle: "Extract Images from PDF using C# | Parse PDF Files in C# ASP.NET"
description: "Use .NET PDF API to extract images from PDF using C# or VB.NET. Parse PDF files to extract content programmatically in C# ASP.NET."
date: Tue, 15 Jun 2021 18:22:55 +0000
draft: false
url: /2021/06/15/extract-images-from-pdf-in-csharp/
author: Usman Aziz
summary: '[PDF][1] format is widely used to create read-only documents for sharing and printing. Generally, the PDF documents contain images along with text and in certain cases, you may need to extract these images while parsing the PDFs. In accordance with that, this article covers **how to extract images from PDF programmatically using C#**.'
tags: ['API to Extract Images from PDF', 'How to Extract Images from PDF in csharp', 'csharp pdf image extractor']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Extract-Images-from-PDF.jpg" alt="Extract Text from PDF C#">}}


[PDF][2] format is widely used to create read-only documents for sharing and printing. Generally, the PDF documents contain images along with text and in certain cases, you may need to extract these images while parsing the PDFs. In accordance with that, this article covers **how to extract images from PDF programmatically using C#**.

*   [API to Extract Images from PDF][3]
*   [How to Extract Images from PDF][4]

## C# API to Extract Images from PDF {#API-to-Extract-Images-from-PDF}

In order to extract images from PDF, we will use [Aspose.PDF for .NET][5]. It is a powerful API that lets you implement a wide range of PDF generation and manipulation features. In addition, it allows you to parse the PDF and extract images seamlessly. You can either [download][6] the API or install it using [NuGet][7].

```
PM> Install-Package Aspose.PDF
```

## How to Extract Images from a PDF {#Extract-Images-from-PDF}

The following are the steps to extract images from a PDF using C#.

*   Load the document using the [Document][8] class.
*   Loop through the pages of the PDF document using [Document.Pages][9] collection.
*   For each page, access every [XImage][10] in the [Page.Resources.Images][11] collection.
*   Create a [FileStream][12] object for each image and save it as JPEG, PNG, etc.
*   Finally, close the _FileStream_.

The following code sample shows how to extract images from the PDF.

{{< gist aspose-com-gists 3d84c7b9f7285728d5ad8da67a8b2a0a "extract-images-from-pdf.cs" >}}

## Get a Free License {#Get-a-Free-License}

You can use Aspose.PDF for .NET without evaluation limitations using a [temporary license][13].

## Conclusion

Parsing the PDF files and extracting the text or images could be required in various cases. In this article, you have learned how to extract images from PDF files programmatically using C#. You can explore more about the C# PDF API using the [documentation][14]. Also, you can post your queries on our [forum][15].

## See Also

*   [Create PDF Files using C# – .NET PDF API][16]
*   [Extract Data from Tables in PDF using C#][17]
*   [Extract Text from PDF using C#][18]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #API-to-Extract-Images-from-PDF
[4]: #Extract-Images-from-PDF
[5]: https://products.aspose.com/pdf/net/
[6]: https://downloads.aspose.com/pdf/net/
[7]: https://nuget.org/packages/Aspose.PDF
[8]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[9]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/pages
[10]: https://apireference.aspose.com/net/pdf/aspose.pdf/ximage
[11]: https://apireference.aspose.com/pdf/net/aspose.pdf/resources/properties/images
[12]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream
[13]: https://purchase.aspose.com/temporary-license
[14]: https://docs.aspose.com/pdf/net/overview/
[15]: https://forum.aspose.com/
[16]: https://blog.aspose.com/2020/12/02/create-pdf-files-using-csharp/
[17]: https://blog.aspose.com/2021/06/10/extract-table-from-pdf-using-csharp/
[18]: https://blog.aspose.com/2020/05/16/extract-text-from-pdf-csharp-vb-net/





