---
title: 'Merge Multiple ZIP or TAR Archives in C#'
seoTitle: "Merge Multiple ZIP or TAR Files in C# | Combine ZIP and TAR Archives"
description: "Merge multiple ZIP and TAR archives into a single file in C# from within .NET applications. Merge ZIP into ZIP, TAR into TAR, ZIP into TAR, or TAR into ZIP."
date: Thu, 06 Jan 2022 13:59:18 +0000
draft: false
url: /2022/01/06/merge-zip-and-tar-files-in-csharp/
author: Usman Aziz
summary: 'While working with archives from within your .NET applications, you may need to merge multiple [ZIP][1] or [TAR][2] files. For instance, you may want to extract files and folders from multiple archives and put them into a single archive. To achieve it, this article covers **how to merge multiple [ZIP][3] or [TAR][4] files in C#**. We will cover the merging of ZIP into ZIP, TAR into TAR, ZIP into TAR, and TAR into ZIP.'
tags: ['Combine TAR with ZIP in Csharp', 'Combine ZIP with TAR in Csharp', 'Csharp API to Merge ZIP and TAR Files', 'Merge Multiple TAR Files in CSharp', 'Merge Multiple ZIP Files in Csharp']
categories: ['Aspose.ZIP Product Family']
---



{{< figure align=center src="images/Merge-ZIP-and-TAR-Archives.jpg" alt="Merge Multiple ZIP or TAR Archives in C#">}}


While working with archives from within your .NET applications, you may need to merge multiple [ZIP][5] or [TAR][6] files. For instance, you may want to extract files and folders from multiple archives and put them into a single archive. To achieve it, this article covers **how to merge multiple [ZIP][7] or [TAR][8] files in C#**. We will cover the merging of ZIP into ZIP, TAR into TAR, ZIP into TAR, and TAR into ZIP.

*   [C# API to Merge ZIP and TAR Files][9]
*   [Merge Multiple ZIP Files in C#][10]
*   [Merge Multiple TAR Files in C#][11]
*   [Combine ZIP with TAR in C#][12]
*   [Combine TAR with ZIP in C#][13]

## C# .NET API to Merge ZIP and TAR Files {#API-to-Create-tar-gz-Archive}

To merge multiple ZIP and TAR archives, we will leverage [Aspose.ZIP for .NET][14]. It is a feature-rich .NET API that allows you to create and manipulate various popular archive formats. You can either [download][15] the API's DLL or install it directly using [NuGet][16].

```
PM> Install-Package Aspose.Zip
```

## Merge Multiple ZIP Files in C# {#Merge-Multiple-ZIP-Files}

Let's start our journey of merging archives with ZIP format. We will take two ZIP archives and collect their entries into a single ZIP file. The following are the steps to merge multiple ZIP files in C#.

*   Load the first ZIP file using [Archive][17] class.
*   Similarly, load the second ZIP file using [Archive][18] class.
*   Now, loop through the entries of first ZIP using [Archive.Entries][19] collection.
*   Copy each [ArchiveEntry][20] to a [MemoryStream][21] object using [ArchiveEntry.Open().CopyTo(MemoryStream)][22] method.
*   Add entry to second ZIP using [Archive.CreateEntry(string, MemoryStream)][23] method.
*   Save the merged ZIP as a separate file using [Archive.Save(string)][24] method.

The following code sample shows how to merge two ZIP files in C#.

{{< gist aspose-com-gists 1ca1a64b63a37ce4b2f6b47b86b922e5 "merge-zip.cs" >}}

## Merge Multiple TAR Files in C# {#Combine-Multiple-TAR-Files}

Let's now check out how to merge multiple TAR archives in C#. The following are the steps to achieve this.

*   Load the first TAR file using [TarArchive][25] class.
*   Similarly, load the second TAR file using [TarArchive][26] class.
*   Now, loop through the entries of first TAR using [TarArchive.Entries][27] collection.
*   Copy each [TarEntry][28] to a [MemoryStream][29] object using [TarEntry.Open().CopyTo(MemoryStream)][30] method.
*   Add entry to second TAR using [TarArchive.CreateEntry(string, MemoryStream)][31] method.
*   Save the merged TAR using [TarArchive.Save(string)][32] method.

The following code sample shows how to merge multiple TAR files in C#.

{{< gist aspose-com-gists 1ca1a64b63a37ce4b2f6b47b86b922e5 "merge-tar.cs" >}}

## Merge ZIP into TAR in C# {#Combine-ZIP-and-TAR-Files}

In this section, we will see how to merge a ZIP file into TAR archive in C#. The following are the steps to perform this operation.

*   Load the ZIP file using [Archive][33] class.
*   Load TAR file using [TarArchive][34] class.
*   Now, loop through the entries of ZIP using [Archive.Entries][35] collection.
*   Copy each [ArchiveEntry][36] to a [MemoryStream][37] object using [ArchiveEntry.Open().CopyTo(MemoryStream)][38] method.
*   Add entry to TAR using [](https://apireference.aspose.com/zip/net/aspose.zip.archive/createentry/methods/1)[TarArchive.CreateEntry(string, MemoryStream)][39] method[.][40]
*   Save the TAR file using [TarArchive.Save(string)][41] method.

The following code sample shows how to merge a ZIP archive into TAR.

{{< gist aspose-com-gists 1ca1a64b63a37ce4b2f6b47b86b922e5 "merge-zip-tar.cs" >}}

## Combine TAR with ZIP in C# {#Combine-TAR-with-ZIP}

Similar to the previous example, you can merge a TAR file into ZIP. The following code sample shows how to extract files from a TAR and merge them into a ZIP.

{{< gist aspose-com-gists 1ca1a64b63a37ce4b2f6b47b86b922e5 "merge-tar-zip.cs" >}}

## Get a Free API License

You can use Aspose.ZIP for .NET without evaluation limitations by getting [a free temporary license][42].

## Conclusion

In this article, you have learned how to merge multiple ZIP or TAR archives programmatically in C#. Particularly, we have covered how to merge ZIP files, TAR files, ZIP into TAR, and TAR into ZIP dynamically. To explore more about Aspose.ZIP for .NET, you can visit the [documentation][43]. Also, you can post your queries to our [forum][44].

## See Also

*   [Add Files or Folders to ZIP Archives in C#][45]
*   [Unzip Files in ZIP Archives using C#][46]




[1]: https://docs.fileformat.com/compression/zip/
[2]: https://docs.fileformat.com/compression/tar/
[3]: https://docs.fileformat.com/compression/zip/
[4]: https://docs.fileformat.com/compression/tar/
[5]: https://docs.fileformat.com/compression/zip/
[6]: https://docs.fileformat.com/compression/tar/
[7]: https://docs.fileformat.com/compression/zip/
[8]: https://docs.fileformat.com/compression/tar/
[9]: #API-to-Create-tar-gz-Archive
[10]: #Merge-Multiple-ZIP-Files
[11]: #Combine-Multiple-TAR-Files
[12]: #Combine-ZIP-and-TAR-Files
[13]: #Combine-TAR-with-ZIP
[14]: https://products.aspose.com/zip/net/
[15]: https://downloads.aspose.com/zip/net/
[16]: https://www.nuget.org/packages/Aspose.ZIP
[17]: https://apireference.aspose.com/zip/net/aspose.zip/archive
[18]: https://apireference.aspose.com/zip/net/aspose.zip/archive
[19]: https://apireference.aspose.com/zip/net/aspose.zip/archive/properties/entries
[20]: https://apireference.aspose.com/zip/net/aspose.zip/archiveentry
[21]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream
[22]: https://docs.microsoft.com/en-gb/dotnet/api/system.io.stream.copyto?view=net-6.0#System_IO_Stream_CopyTo_System_IO_Stream_
[23]: https://apireference.aspose.com/zip/net/aspose.zip.archive/createentry/methods/1
[24]: https://apireference.aspose.com/zip/net/aspose.zip.archive/save/methods/1
[25]: https://apireference.aspose.com/zip/net/aspose.zip.tar/tararchive
[26]: https://apireference.aspose.com/zip/net/aspose.zip.tar/tararchive
[27]: https://apireference.aspose.com/zip/net/aspose.zip.tar/tararchive/properties/entries
[28]: https://apireference.aspose.com/zip/net/aspose.zip.tar/tarentry
[29]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream
[30]: https://docs.microsoft.com/en-gb/dotnet/api/system.io.stream.copyto?view=net-6.0#System_IO_Stream_CopyTo_System_IO_Stream_
[31]: https://apireference.aspose.com/zip/net/aspose.zip.tar.tararchive/createentry/methods/1
[32]: https://apireference.aspose.com/zip/net/aspose.zip.tar.tararchive/save/methods/1
[33]: https://apireference.aspose.com/zip/net/aspose.zip/archive
[34]: https://apireference.aspose.com/zip/net/aspose.zip.tar/tararchive
[35]: https://apireference.aspose.com/zip/net/aspose.zip/archive/properties/entries
[36]: https://apireference.aspose.com/zip/net/aspose.zip/archiveentry
[37]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream
[38]: https://docs.microsoft.com/en-gb/dotnet/api/system.io.stream.copyto?view=net-6.0#System_IO_Stream_CopyTo_System_IO_Stream_
[39]: https://apireference.aspose.com/zip/net/aspose.zip.tar.tararchive/createentry/methods/1
[40]: https://apireference.aspose.com/zip/net/aspose.zip.archive/createentry/methods/1
[41]: https://apireference.aspose.com/zip/net/aspose.zip.tar.tararchive/save/methods/1
[42]: https://purchase.aspose.com/temporary-license
[43]: https://docs.aspose.com/zip/net/
[44]: https://forum.aspose.com/
[45]: https://blog.aspose.com/2020/04/22/create-zip-archives-add-files-or-folders-to-zip-in-csharp-asp.net/
[46]: https://blog.aspose.com/2020/04/23/unzip-files-in-password-protected-zip-archives-in-csharp-asp.net/




