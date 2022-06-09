---
title: 'Compress and Decompress Files using GZip in C#'
seoTitle: "Compress and Decompress GZip in C# | Create or Extract GZip in C# .NET"
description: "Use .NET archive API to compress and decompress GZip archives using C#. Compress files using GNU compression and extract GZip into memory stream."
date: Fri, 07 May 2021 21:01:10 +0000
draft: false
url: /2021/05/07/create-and-extract-gzip-archives-using-csharp/
author: Usman Aziz
summary: '[GZip][1] archives ([.gz][2] are used to compress one or more files using the GNU zip compression algorithm. It is commonly used for file compression in UNIX operating systems. In this article, you will learn how to compress files and **create GZip (.gz) archives programmatically using C#**. Moreover, the article will also cover **how to extract GZip archives using C#**.'
tags: ['Compress Files to GZip in Csharp', 'Csharp API to Create and Extract GZip', 'Decompress Files to GZip in Csharp', 'Extract a GZip Archive in Csharp']
categories: ['Aspose.ZIP Product Family']
---



{{< figure align=center src="images/Create-GZip-in-C.jpg" alt="Create GZip in C#">}}


[GZip][3] archives ([.gz][4] are used to compress one or more files using the GNU zip compression algorithm. It is commonly used for file compression in UNIX operating systems. In this article, you will learn **how to compress files using GZip (.gz) programmatically in [C#][5]**. Moreover, the article will also cover **how to decompress GZip archives in C#**.

*   [.NET API to Compress and Decompress Files using GZip][6]
*   [Compress Files using GZip in C#][7]
*   [Decompress a GZip Archive in C#][8]
*   [Extract a GZip Archive into Stream in C#][9]

## C# API to Compress and Decompress Files using GZip {#C-API-to-Create-and-Extract-GZip}

To compress and decompress files using GZip, we will use [Aspose.ZIP for .NET][10]. It is a powerful API that lets you work with popular archive formats including [ZIP][11], [7z][12], GZip, etc. You can either [download][13] the API or install it using [NuGet][14].

```
PM> Install-Package Aspose.Zip
```

## Compress Files using GZip in C# {#Create-a-GZip-Archive-in-C}

The following are the steps to compress files using GZip in C#.

*   Create an object of the [GzipArchive][15] class.
*   Use [GzipArchive.SetSource(String)][16] method to add a file to archive.
*   Create GZip archive using [GzipArchive.Save(String)][17] method.

The following code sample shows how to compress files to GZip in C#.

{{< gist aspose-com-gists f0195d651fb08e5141e8d8d6069ae461 "create-gzip.cs" >}}

## Decompress a GZip Archive in C# {#Extract-a-GZip-Archive-in-C}

The following are the steps to decompress a GZip archive in C# using Aspose.ZIP for .NET.

*   Create an object of the [GzipArchive][18] class and initialize it with GZip archive's path.
*   Create a file for extracted content using [File.Create(String)][19] method.
*   Open GZip for extraction using [GZipArchive.Open()][20] method.
*   Read the extracted content and write it to the file.

The following code sample shows how to decompress a GZip archive using C#.

{{< gist aspose-com-gists f0195d651fb08e5141e8d8d6069ae461 "extract-gzip.cs" >}}

## Extact a GZip Archive into Stream in C# {#Extract-a-GZip-Archive-into-Stream-in-C}

You can also extract a GZip archive into a memory stream object. The following are the steps to perform this operation.

*   Create a new [MemoryStream][21] object.
*   Create an object of [GzipArchive][22] class and initialize it with GZip archive's path.
*   Extract GZip and copy to memory stream using [GZipArchive.Open().CopyTo(MemoryStream)][23] method.

The following code sample shows how to extract a GZip archive into a memory stream using C#.

{{< gist aspose-com-gists f0195d651fb08e5141e8d8d6069ae461 "extract-gzip-to-stream.cs" >}}

## Get a Free API License

You can [get a free temporary license][24] in order to use the API without evaluation limitations.

## Conclusion

In this article, you have learned how to compress or decompress files using GZip in C#. Furthermore, you have seen how to extract a GZip to stream programmatically. You can explore more about Aspose.ZIP for .NET using [documentation][25]. In addition, you can contact us to share your queries via our [forum][26].

## See Also

*   [Add Files or Folders to ZIP Archives Programmatically in C#][27]
*   [Unzip Files in ZIP Archives using C#][28]




[1]: https://en.wikipedia.org/wiki/Gzip
[2]: https://docs.fileformat.com/compression/gz/)
[3]: https://en.wikipedia.org/wiki/Gzip
[4]: https://docs.fileformat.com/compression/gz/)
[5]: https://docs.fileformat.com/programming/cs/
[6]: #C-API-to-Create-and-Extract-GZip
[7]: #Create-a-GZip-Archive-in-C
[8]: #Extract-a-GZip-Archive-in-C
[9]: #Extract-a-GZip-Archive-into-Stream-in-C
[10]: https://products.aspose.com/zip/net
[11]: https://docs.fileformat.com/compression/zip/
[12]: https://docs.fileformat.com/compression/7z/
[13]: https://downloads.aspose.com/zip/net
[14]: https://www.nuget.org/packages/Aspose.Zip
[15]: https://apireference.aspose.com/zip/net/aspose.zip.gzip/gziparchive
[16]: https://apireference.aspose.com/zip/net/aspose.zip.gzip.gziparchive/setsource/methods/3
[17]: https://apireference.aspose.com/zip/net/aspose.zip.gzip.gziparchive/save/methods/1
[18]: https://apireference.aspose.com/zip/net/aspose.zip.gzip/gziparchive
[19]: https://docs.microsoft.com/en-us/dotnet/api/system.io.file.create
[20]: https://apireference.aspose.com/zip/net/aspose.zip.gzip/gziparchive/methods/open
[21]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream
[22]: https://apireference.aspose.com/zip/net/aspose.zip.gzip/gziparchive
[23]: https://apireference.aspose.com/zip/net/aspose.zip.gzip/gziparchive/methods/open
[24]: https://purchase.aspose.com/temporary-license
[25]: https://docs.aspose.com/zip/net/getting-started/
[26]: https://forum.aspose.com/
[27]: https://blog.aspose.com/2020/04/22/create-zip-archives-add-files-or-folders-to-zip-in-csharp-asp.net/
[28]: https://blog.aspose.com/2020/04/23/unzip-files-in-password-protected-zip-archives-in-csharp-asp.net/





