---
title: 'Merge Multiple PDF Files using C# .NET'
seoTitle: ""
description: ""
date: Thu, 16 Jan 2020 15:24:08 +0000
draft: false
url: /2020/01/16/merge-multiple-pdf-files-in-csharp-net/
author: Usman Aziz
summary: ''
tags: ['combine pdf', 'combine pdf in .net', 'merge multiple pdf in .net', 'merge pdf in .net', 'merge pdf in csharp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Merge-PDF-files-in-C.png" alt="Merge PDF files in C# ">}}


Merging multiple PDF files into a single PDF could be useful in various scenarios. For example, you can keep similar documents (i.e. resumes) into a single file or you may want to share a single file instead of a bulk. In order to meet the above-mentioned or similar requirements, in this article, you will learn **how to merge multiple PDF files in C#**.

*   [C# API to Merge PDFs][1]
*   [Merge two PDF files using C#][2]
*   [Merge multiple (more than two) PDF files in C#][3]
*   [Combine PDF files using file streams][4]

## Merge PDFs using C# PDF API - Free Download {#CSharp-API-to-Merge-PDFs}

[**Aspose.PDF for .NET**][5] is a feature-rich API for creating, editing, reading, or converting PDF documents. Along with other PDF manipulation features, Aspose.PDF for .NET also allows you to **combine** or **merge PDF files** programmatically. You can [download][6] the API or install it either by using the NuGet Package Manager or the Package Manager Console in Visual Studio.

### Installing via NuGet Package Manager



{{< figure align=center src="images/Aspose.PDF-NPM.png" alt="Merge multiple PDF files in C# .NET">}}


### Installing via Package Manager Console```
PM> Install-Package Aspose.PDF
```

## Merge Two PDF Files using C# {#Merge-two-PDF-files-using-CSharp}

The process of merging two PDF files into a single PDF is as simple as pie and can be performed only in two steps.

*   Create an instance of [PdfFileEditor][7] class.
*   Call [PdfFileEditor.Concatenate(string, string , string)][8] method.

The following is the code sample to merge two PDF files using C#.

{{< gist aspose-com-gists deb84b700e3bb699b5af25f4c10b7e8d "merge-two-pdf-files.cs" >}}

## Merge Multiple PDF Files in C# {#Merge-Multiple-PDF-Files-in-CSharp}

In case you want to merge more than two PDF files, you can do it using a string array containing the paths of all the PDF files to be merged. The following are the steps to perform this operation.

*   Create an instance of _PdfFileEditor_ class.
*   Create an array containing paths of the PDF files to be merged.
*   Call [PdfFileEditor.Concatenate(string\[\], string)][9] method.

The following code sample shows how to merge multiple PDF files.

{{< gist aspose-com-gists deb84b700e3bb699b5af25f4c10b7e8d "merge-multiple-pdf-files.cs" >}}

## Merge PDF Files using Streams in C# {#Combine-PDF-files-using-file-streams}

There might be a case when you are not dealing with the files located on the disk. Instead, you want to merge PDF files available in the form of streams. In such a case, you can merge the PDFs directly using the Stream objects in the overloaded _PdfFileEditor.Concatenate()_ methods. The following code samples show how to merge PDF files using the Stream objects.

### Merge Two PDF Files using Stream Objects

{{< gist aspose-com-gists deb84b700e3bb699b5af25f4c10b7e8d "merge-two-pdf-files-using-stream.cs" >}}

### Merge Multiple PDF Files using Stream Objects

{{< gist aspose-com-gists deb84b700e3bb699b5af25f4c10b7e8d "merge-multiple-pdf-files-using-stream.cs" >}}

## Conclusion

In this article, you have learned how to merge PDF files programmatically using C#. Furthermore, this article explicitly discusses how to merge two PDF files or multiple (more than two) PDF files into a single PDF. In case you are interested to explore more about the _Aspose.PDF for .NET_, take a look at the [documentation][10].

## See Also

*   [Create PDF Files Programmatically in ASP.NET Core][11]




[1]: #CSharp-API-to-Merge-PDFs
[2]: #Merge-two-PDF-files-using-CSharp
[3]: #Merge-Multiple-PDF-Files-in-CSharp
[4]: #Combine-PDF-files-using-file-streams
[5]: https://products.aspose.com/pdf/net
[6]: https://downloads.aspose.com/pdf/net
[7]: https://apireference.aspose.com/net/pdf/aspose.pdf.facades/pdffileeditor
[8]: https://apireference.aspose.com/net/pdf/aspose.pdf.facades.pdffileeditor/concatenate/methods/5
[9]: https://apireference.aspose.com/net/pdf/aspose.pdf.facades.pdffileeditor/concatenate/methods/7
[10]: https://docs.aspose.com/display/pdfnet/Product+Overview
[11]: https://blog.aspose.com/2020/02/06/create-pdf-files-in-asp-net-core-mvc/





