---
title: 'Convert ZIP Archives to TAR in C#'
seoTitle: "Convert ZIP Archives to TAR in C# .NET | ZIP to TAR Converter API"
description: "Use .NET ZIP API to convert ZIP archives to TAR format programmatically in C#. Download the API and integrate the source code into your application."
date: Mon, 27 Dec 2021 16:19:00 +0000
draft: false
url: /2021/12/27/convert-zip-to-tar-in-csharp-net/
author: Usman Aziz
summary: '[ZIP][1] is a popular archiving format that is used to compress files and folders. ZIP makes it easier to share multiple files by reducing their size and keeping them into a single file. On the other hand, [TAR][2] is a famous Unix-based archiving format that is used to package the files before sharing. In various cases, you have to convert the ZIP archives into TAR format. To achieve this programmatically, this article shows **how to convert a ZIP archive to TAR in C#**.'
tags: ['Convert ZIP to TAR in Csharp', 'Copy ZIP files to TAR in Csharp', 'Dotnet API to Convert ZIP to TAR', 'ZIP to TAR Converter']
categories: ['Aspose.ZIP Product Family']
---



{{< figure align=center src="images/Convert-ZIP-to-TAR-1.png" alt="Convert ZIP Archives to TAR in C#">}}


[ZIP][3] is a popular archiving format that is used to compress files and folders. ZIP makes it easier to share multiple files by reducing their size and keeping them into a single file. On the other hand, [TAR][4] is a famous Unix-based archiving format that is used to package the files before sharing. In various cases, you have to convert the ZIP archives into TAR format. To achieve this programmatically, this article shows **how to convert a ZIP archive to TAR in C#**.

*   [.NET API to Convert ZIP to TAR][5]
*   [Convert a ZIP Archive to TAR][6]

## C# .NET API to Convert ZIP to TAR {#API-to-Convert-ZIP-to-TAR}

To convert ZIP archives to TAR format, we will use [Aspose.ZIP for .NET][7]. The API provides a wide range of features to create and manipulate ZIP, TAR, and other popular archiving formats. You can either [download][8] the API's DLL or install it from [NuGet][9].

```
PM> Install-Package Aspose.Zip 
```

## Convert a ZIP Archive to TAR in C# {#Convert-a-ZIP-Archive-to-TAR}

The conversion of ZIP to TAR is quite easy using Aspose.ZIP for .NET. Simply, load the ZIP file, transfer its entries to a TAR archive and save the TAR archive to your desired location. The following are the steps to convert a ZIP archive to TAR in C#.

*   Load the ZIP file using [Archive][10] class.
*   Create an object of [TarArchive][11] class for TAR archive.
*   Access each [ArchiveEntry][12] in the ZIP using [Archive.Entries][13] collection.
*   For each entry in ZIP archive, perform the following steps:
    *   Copy entry into a [MemoryStream][14] object using [ArchiveEntry.Open().CopyTo(MemoryStream)][15] method.
    *   Transfer entry to TAR archive using [TarArchive.CreateEntry(String, MemoryStream)][16] method.
*   Finally, save the TAR archive to your desired location using [TarArchive.Save(String)][17] method.

The following code sample shows how to convert a ZIP archive to TAR format in .NET applications.

{{< gist aspose-com-gists b946bed04067591ae454630fd5b4a36c "convert-zip-to-tar.cs" >}}

## Get a Free API License

You can get [a free temporary license][18] to use Aspose.ZIP for .NET without evaluation limitations.

## Conclusion

The conversion of ZIP archives to TAR format is often needed before sharing the files over the internet. Therefore, in this article, you have learned how to convert a ZIP archive to TAR programmatically in C#. You can simply install Aspose.ZIP for .NET and embed the provided code to perform ZIP to TAR conversion from within your .NET applications. In addition, you can visit [documentation][19] to explore more about Aspose.ZIP for .NET. Moreover, you can share your queries with us via our [forum][20].

## See Also

*   [Add Files or Folders to ZIP Archives in C#][21]
*   [Unzip Files in ZIP Archives using C#][22]
*   [Merge Multiple ZIP or TAR Archives in C#][23]
*   [Create Executable Self-extracting Archive in C#][24]




[1]: https://docs.fileformat.com/compression/zip/
[2]: https://docs.fileformat.com/compression/tar/
[3]: https://docs.fileformat.com/compression/zip/
[4]: https://docs.fileformat.com/compression/tar/
[5]: #API-to-Convert-ZIP-to-TAR
[6]: #Convert-a-ZIP-Archive-to-TAR
[7]: https://products.aspose.com/zip/net/
[8]: https://downloads.aspose.com/zip/net/
[9]: https://www.nuget.org/packages/Aspose.ZIP
[10]: https://apireference.aspose.com/zip/net/aspose.zip/archive
[11]: https://apireference.aspose.com/zip/net/aspose.zip.tar/tararchive
[12]: https://apireference.aspose.com/zip/net/aspose.zip/archiveentry
[13]: https://apireference.aspose.com/zip/net/aspose.zip/archive/properties/entries
[14]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream
[15]: https://docs.microsoft.com/en-gb/dotnet/api/system.io.stream.copyto?view=net-6.0#System_IO_Stream_CopyTo_System_IO_Stream_
[16]: https://apireference.aspose.com/zip/net/aspose.zip.tar.tararchive/createentry/methods/1
[17]: https://apireference.aspose.com/zip/net/aspose.zip.tar.tararchive/save/methods/1
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/zip/net/
[20]: https://forum.aspose.com/
[21]: https://blog.aspose.com/2020/04/22/create-zip-archives-add-files-or-folders-to-zip-in-csharp-asp.net/
[22]: https://blog.aspose.com/2020/04/23/unzip-files-in-password-protected-zip-archives-in-csharp-asp.net/
[23]: https://blog.aspose.com/2022/01/06/merge-zip-and-tar-files-in-csharp/
[24]: https://blog.aspose.com/2022/01/10/create-self-extracting-archive-in-csharp/




