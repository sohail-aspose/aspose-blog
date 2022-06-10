---
title: 'Convert DOCX to DOC or DOC to DOCX with C# VB.NET'
seoTitle: "Convert DOCX to DOC | DOC to DOCX Programmatically in C# VB.NET"
description: "Convert DOCX to DOC or From DOC to DOCX Programmatically using C# or VB.NET. Batch convert DOC and DOCX files. Change DOCX to DOC or Save As word files."
date: Sat, 24 Oct 2020 19:34:27 +0000
draft: false
url: /2020/10/24/convert-docx-doc-with-csharp-vb-net/
author: Farhan Raza
summary: 'Microsoft Word Documents are majorly of two types, DOC and DOCX. You can convert DOCX to DOC as well as from DOC to DOCX using C# or VB.NET programmatically. Each document can be processed and converted one by one or you can batch convert the DOC and DOCX files if you need to work with a lot of files.'
tags: ['convert doc to docx', 'convert docx to doc', 'doc to docx', 'doc to docx c#', 'doc to docx vb.net', 'docx to doc', 'docx to doc c#']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Convert-DOCX-to-DOC-to-DOCX.png" alt="Convert DOCX to DOC C#">}}


Microsoft Word Documents are majorly of two types, [DOC][1] and [DOCX][2]. You can convert DOCX to DOC as well as from DOC to DOCX using C# or VB.NET programmatically. Each document can be processed and converted one by one or you can batch convert the DOC and DOCX files if you need to work with a lot of files. You can explore the following use cases to understand the topic in detail:

*   [DOCX to DOC and DOC to DOCX Converter API – Installation][3]
*   [Convert DOCX to DOC File Programmatically using C# or VB.NET][4]
*   [Batch Convert DOCX to DOC Files using C# or VB.NET][5]
*   [Convert DOC to DOCX File Programmatically using C# or VB.NET][6]
*   [Batch Convert DOC to DOCX using C# or VB.NET][7]

## DOCX to DOC and DOC to DOCX Converter API – Installation {#section1}

[Aspose.Words for .NET][8] API can be used for efficient and quick conversion of DOCX to DOC and DOC to DOCX file format. You can configure the API in your .NET framework based applications so you can use C# as well as VB.NET language to programmatically perform the conversion. You can download the DLL file as ZIP achieve from the [official website][9], or you can install the API in your solution using the following [NuGet][10] command:

```
Install-Package Aspose.Words
```

## Convert DOCX to DOC File Programmatically using C# or VB.NET {#section2}

The main difference between DOC and DOCX is that the DOC file format is a binary file where DOCX file format is a ZIP file containing all related XML files. You can convert DOCX file to DOC document with the following steps:

1.  Specify [LoadFormat][11] of the source file
2.  Load input DOCX file
3.  Save output DOC file using [SaveFormat][12]

The code snippet below shows how to convert DOCX to DOC using C# or VB.NET:

{{< gist aspose-com-gists 3b020dbd88282d9be60ca0bc280947da "DOCXtoDOC.cs" >}}

## Batch Convert DOCX to DOC Files using C# or VB.NET {#section3}

You may need to convert hundreds of DOCX files to DOC format in your .NET applications. You can easily convert a batch of files by executing the program only once. Follow the steps below for converting a batch of DOCX files:

1.  Load all DOCX files from a directory or folder
2.  Load each DOCX file using [LoadOptions][13] class
3.  Change the extension of each input file to DOC
4.  Save output file as DOC format file

The following code shows how to convert a batch of DOCX files to DOC format files using C# or VB.NET:

{{< gist aspose-com-gists 3b020dbd88282d9be60ca0bc280947da "DOCXtoDOCbatch.cs" >}}

## Convert DOC to DOCX File using C# or VB.NET {#section4}

You can convert Microsoft Word DOC files to DOCX format file in your .NET Framework based applications using C# or VB.NET. Below are the steps to perform the conversion:

1.  Set the [LoadFormat][14] of input DOC file
2.  Initialize the source document with Document class
3.  Save output file in DOCX format

The code below shows how to convert DOC to DOCX using C# or VB.NET:

{{< gist aspose-com-gists 3b020dbd88282d9be60ca0bc280947da "DOCtoDOCX.cs" >}}

## Batch Convert DOC to DOCX Programmatically using C# or VB.NET {#section5}

You can also process the conversion of multiples files and different batches for DOC to DOCX conversion. You need to follow the steps below to convert such files:

1.  Load all DOC files from a directory
2.  Set the DOC value from [LoadFormat][15] enumeration
3.  Load input document
4.  Save output DOCX file using [SaveFormat][16]

The following code sample explains how to convert a batch of DOC files to DOCX files using C# or VB.NET:

{{< gist aspose-com-gists 3b020dbd88282d9be60ca0bc280947da "DOCtoDOCXbatch.cs" >}}

## Conclusion

You have learned how to perform inter-conversion of DOC and DOCX file format. Specifically, you have explored how to convert DOC to DOCX as well as DOCX to DOC. Moreover, you have also learned how to convert a batch of DOC or DOCX files programmatically using C# or VB.NET. However, if you are interested to learn further then you can refer to [API Documentation][17] and [Product Page][18]. Furthermore, in case of any queries, please feel free to reach out to us at [Free Support Forum][19].

## See Also

[Convert Word DOC or DOCX to HTML, MHTML in C# VB.NET][20]




[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/word-processing/docx/
[3]: #section1
[4]: #section2
[5]: #section3
[6]: #section4
[7]: #section5
[8]: https://products.aspose.com/words/net
[9]: https://releases.aspose.com/
[10]: https://www.nuget.org/packages/Aspose.Words
[11]: https://apireference.aspose.com/words/net/aspose.words/loadformat
[12]: https://apireference.aspose.com/words/net/aspose.words/saveformat
[13]: https://apireference.aspose.com/words/net/aspose.words.loading/loadoptions/constructors/main
[14]: https://apireference.aspose.com/words/net/aspose.words/loadformat
[15]: https://apireference.aspose.com/words/net/aspose.words/loadformat
[16]: https://apireference.aspose.com/words/net/aspose.words/saveformat
[17]: https://docs.aspose.com/words/net/
[18]: https://products.aspose.com/words/net
[19]: https://forum.aspose.com/c/words
[20]: https://blog.aspose.com/2020/10/02/convert-word-doc-or-docx-to-html-mhtml-csharp-vb-net/





