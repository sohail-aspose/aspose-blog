---
title: 'Merge Multiple ZIP or TAR Archives in C#'
date: Thu, 06 Jan 2022 13:59:18 +0000
draft: false
url: /2022/01/06/merge-zip-and-tar-files-in-csharp/
author: 'Usman Aziz'
summary: 'While working with archives from within your .NET applications, you may need to merge multiple [ZIP](https://docs.fileformat.com/compression/zip/) or [TAR](https://docs.fileformat.com/compression/tar/) files. For instance, you may want to extract files and folders from multiple archives and put them into a single archive. To achieve it, this article covers **how to merge multiple [ZIP](https://docs.fileformat.com/compression/zip/) or [TAR](https://docs.fileformat.com/compression/tar/) files in C#**. We will cover the merging of ZIP into ZIP, TAR into TAR, ZIP into TAR, and TAR into ZIP.'
tags: ['Combine TAR with ZIP in Csharp', 'Combine ZIP with TAR in Csharp', 'Csharp API to Merge ZIP and TAR Files', 'Merge Multiple TAR Files in CSharp', 'Merge Multiple ZIP Files in Csharp']
categories: ['Aspose.ZIP Product Family']
---



{{< figure align=center src="images/Merge-ZIP-and-TAR-Archives.jpg" alt="Merge Multiple ZIP or TAR Archives in C#">}}


While working with archives from within your .NET applications, you may need to merge multiple [ZIP](https://docs.fileformat.com/compression/zip/) or [TAR](https://docs.fileformat.com/compression/tar/) files. For instance, you may want to extract files and folders from multiple archives and put them into a single archive. To achieve it, this article covers **how to merge multiple [ZIP](https://docs.fileformat.com/compression/zip/) or [TAR](https://docs.fileformat.com/compression/tar/) files in C#**. We will cover the merging of ZIP into ZIP, TAR into TAR, ZIP into TAR, and TAR into ZIP.

*   [C# API to Merge ZIP and TAR Files](#API-to-Create-tar-gz-Archive)
*   [Merge Multiple ZIP Files in C#](#Merge-Multiple-ZIP-Files)
*   [Merge Multiple TAR Files in C#](#Combine-Multiple-TAR-Files)
*   [Combine ZIP with TAR in C#](#Combine-ZIP-and-TAR-Files)
*   [Combine TAR with ZIP in C#](#Combine-TAR-with-ZIP)

## C# .NET API to Merge ZIP and TAR Files {#API-to-Create-tar-gz-Archive}

To merge multiple ZIP and TAR archives, we will leverage [Aspose.ZIP for .NET](https://products.aspose.com/zip/net/). It is a feature-rich .NET API that allows you to create and manipulate various popular archive formats. You can either [download](https://downloads.aspose.com/zip/net/) the API's DLL or install it directly using [NuGet](https://www.nuget.org/packages/Aspose.ZIP).

```
PM> Install-Package Aspose.Zip
```

## Merge Multiple ZIP Files in C# {#Merge-Multiple-ZIP-Files}

Let's start our journey of merging archives with ZIP format. We will take two ZIP archives and collect their entries into a single ZIP file. The following are the steps to merge multiple ZIP files in C#.

*   Load the first ZIP file using [Archive](https://apireference.aspose.com/zip/net/aspose.zip/archive) class.
*   Similarly, load the second ZIP file using [Archive](https://apireference.aspose.com/zip/net/aspose.zip/archive) class.
*   Now, loop through the entries of first ZIP using [Archive.Entries](https://apireference.aspose.com/zip/net/aspose.zip/archive/properties/entries) collection.
*   Copy each [ArchiveEntry](https://apireference.aspose.com/zip/net/aspose.zip/archiveentry) to a [MemoryStream](https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream) object using [ArchiveEntry.Open().CopyTo(MemoryStream)](https://docs.microsoft.com/en-gb/dotnet/api/system.io.stream.copyto?view=net-6.0#System_IO_Stream_CopyTo_System_IO_Stream_) method.
*   Add entry to second ZIP using [Archive.CreateEntry(string, MemoryStream)](https://apireference.aspose.com/zip/net/aspose.zip.archive/createentry/methods/1) method.
*   Save the merged ZIP as a separate file using [Archive.Save(string)](https://apireference.aspose.com/zip/net/aspose.zip.archive/save/methods/1) method.

The following code sample shows how to merge two ZIP files in C#.

\[gist id="1ca1a64b63a37ce4b2f6b47b86b922e5" file="merge-zip.cs"\]

## Merge Multiple TAR Files in C# {#Combine-Multiple-TAR-Files}

Let's now check out how to merge multiple TAR archives in C#. The following are the steps to achieve this.

*   Load the first TAR file using [TarArchive](https://apireference.aspose.com/zip/net/aspose.zip.tar/tararchive) class.
*   Similarly, load the second TAR file using [TarArchive](https://apireference.aspose.com/zip/net/aspose.zip.tar/tararchive) class.
*   Now, loop through the entries of first TAR using [TarArchive.Entries](https://apireference.aspose.com/zip/net/aspose.zip.tar/tararchive/properties/entries) collection.
*   Copy each [TarEntry](https://apireference.aspose.com/zip/net/aspose.zip.tar/tarentry) to a [MemoryStream](https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream) object using [TarEntry.Open().CopyTo(MemoryStream)](https://docs.microsoft.com/en-gb/dotnet/api/system.io.stream.copyto?view=net-6.0#System_IO_Stream_CopyTo_System_IO_Stream_) method.
*   Add entry to second TAR using [TarArchive.CreateEntry(string, MemoryStream)](https://apireference.aspose.com/zip/net/aspose.zip.tar.tararchive/createentry/methods/1) method.
*   Save the merged TAR using [TarArchive.Save(string)](https://apireference.aspose.com/zip/net/aspose.zip.tar.tararchive/save/methods/1) method.

The following code sample shows how to merge multiple TAR files in C#.

\[gist id="1ca1a64b63a37ce4b2f6b47b86b922e5" file="merge-tar.cs"\]

## Merge ZIP into TAR in C# {#Combine-ZIP-and-TAR-Files}

In this section, we will see how to merge a ZIP file into TAR archive in C#. The following are the steps to perform this operation.

*   Load the ZIP file using [Archive](https://apireference.aspose.com/zip/net/aspose.zip/archive) class.
*   Load TAR file using [TarArchive](https://apireference.aspose.com/zip/net/aspose.zip.tar/tararchive) class.
*   Now, loop through the entries of ZIP using [Archive.Entries](https://apireference.aspose.com/zip/net/aspose.zip/archive/properties/entries) collection.
*   Copy each [ArchiveEntry](https://apireference.aspose.com/zip/net/aspose.zip/archiveentry) to a [MemoryStream](https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream) object using [ArchiveEntry.Open().CopyTo(MemoryStream)](https://docs.microsoft.com/en-gb/dotnet/api/system.io.stream.copyto?view=net-6.0#System_IO_Stream_CopyTo_System_IO_Stream_) method.
*   Add entry to TAR using [](https://apireference.aspose.com/zip/net/aspose.zip.archive/createentry/methods/1)[TarArchive.CreateEntry(string, MemoryStream)](https://apireference.aspose.com/zip/net/aspose.zip.tar.tararchive/createentry/methods/1) method[.](https://apireference.aspose.com/zip/net/aspose.zip.archive/createentry/methods/1)
*   Save the TAR file using [TarArchive.Save(string)](https://apireference.aspose.com/zip/net/aspose.zip.tar.tararchive/save/methods/1) method.

The following code sample shows how to merge a ZIP archive into TAR.

\[gist id="1ca1a64b63a37ce4b2f6b47b86b922e5" file="merge-zip-tar.cs"\]

## Combine TAR with ZIP in C# {#Combine-TAR-with-ZIP}

Similar to the previous example, you can merge a TAR file into ZIP. The following code sample shows how to extract files from a TAR and merge them into a ZIP.

\[gist id="1ca1a64b63a37ce4b2f6b47b86b922e5" file="merge-tar-zip.cs"\]

## Get a Free API License

You can use Aspose.ZIP for .NET without evaluation limitations by getting [a free temporary license](https://purchase.aspose.com/temporary-license).

## Conclusion

In this article, you have learned how to merge multiple ZIP or TAR archives programmatically in C#. Particularly, we have covered how to merge ZIP files, TAR files, ZIP into TAR, and TAR into ZIP dynamically. To explore more about Aspose.ZIP for .NET, you can visit the [documentation](https://docs.aspose.com/zip/net/). Also, you can post your queries to our [forum](https://forum.aspose.com/).

## See Also

*   [Add Files or Folders to ZIP Archives in C#](https://blog.aspose.com/2020/04/22/create-zip-archives-add-files-or-folders-to-zip-in-csharp-asp.net/)
*   [Unzip Files in ZIP Archives using C#](https://blog.aspose.com/2020/04/23/unzip-files-in-password-protected-zip-archives-in-csharp-asp.net/)



