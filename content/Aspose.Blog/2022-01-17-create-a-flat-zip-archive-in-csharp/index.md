---
title: 'Create a Flat ZIP Archive in C#'
date: Mon, 17 Jan 2022 23:45:00 +0000
draft: false
url: /2022/01/17/create-a-flat-zip-archive-in-csharp/
author: 'Usman Aziz'
summary: 'Often, you get a [ZIP][1] archive that contains other ZIP archives inside it forming a nested structure of the archives. In such cases, you may want to get a flat structure by extracting all the inner ZIP archives into the outer archive. To perform this operation programmatically, this article shows **how to create a flat ZIP archive in C#**.'
tags: ['Create a Flat ZIP Archive in Csharp', 'Dotnet API to Create Flat ZIP Archives', 'Dotnet ZIP Library']
categories: ['Aspose.ZIP Product Family']
---



{{< figure align=center src="images/Create-Flat-ZIP-Archive.png" alt="">}}


Often, you get a [ZIP][2] archive that contains other ZIP archives inside it forming a nested structure of the archives. In such cases, you may want to get a flat structure by extracting all the inner ZIP archives into the outer archive. To perform this operation programmatically, this article shows **how to create a flat ZIP archive in C#**.

*   [.NET API to Create Flat ZIP Archives][3]
*   [Create a Flat ZIP Archive][4]

## C# .NET API to Create Flat ZIP Archives {#API-to-Create-Flat-ZIP-Archives}

To create the flat ZIP archives, we will use [Aspose.ZIP for .NET][5]. It is an archiving API that is designed to create and extract popular archive formats including ZIP, TAR, GZip, and 7z. You can either install the API from [NuGet][6] or download its DLL from the [downloads section][7].

```
PM> Install-Package Aspose.Zip
```

## Create a Flat ZIP Archive in C# {#Create-a-Flat-ZIP-Archive}

To understand the structure of a flat ZIP archive, let's take an example. The following is a ZIP archive that contains another ZIP archive inside it.

```
parent.zip
 ├first.txt
 ├inner.zip
 │ ├game.exe
 │ └subitem.bin
 └picture.gif
```

After transforming this ZIP archive to a flat ZIP, all the entries of the inner ZIP will be extracted into the parent ZIP. Finally, we'll get the following structure of the parent ZIP.

```
flatten.zip
 ├first.txt
 ├picture.gif
 ├game.exe
 └subitem.bin
```

Let's see how to perform this transformation programmatically. The following are the steps to create a flat ZIP archive in C#.

*   First, load the parent ZIP archive using [Archive][8] class.
*   Then, create lists to store the inner ZIP entries to delete from parent ZIP, extracted entries and their names.
*   After that, loop through each [ArchiveEntry][9] in the parent ZIP using [Archive.Entries][10] collection.
*   For each entry, perform the following operations:
    *   Check if entry is a ZIP archive using [ArchiveEntry.Name.EndsWith(".zip", StringComparison.InvariantCultureIgnoreCase))][11] method.
    *   Then, add entry to the list of entries to be deleted.
    *   Open entry into a [MemoryStream][12] object using [ArchiveEntry.Open().CopyTo(MemoryStream)][13] method.
    *   Iterate through the entries of inner ZIP archive and in each iteration, perform following steps.
        *   Add name of entry into list of entries to be added.
        *   Then, load entry to _MemoryStream_ using _ArchiveEntry.Open().CopyTo(MemoryStream)_ method.
        *   Finally, add entry to the list of entries to be added to parent ZIP.
*   Then, loop through the list of inner ZIP archives and delete each entry using [Archive.DeleteEntry(ArchiveEntry)][14] method.
*   Loop through the list of entries to be added to parent ZIP and add each entry using [Archive.CreateEntry(String, Stream)][15] method.
*   Finally, save the parent ZIP archive using [Archive.Save(String)][16] method.

The following code sample shows how to create a flat ZIP archive in C#.

{{< gist aspose-com-gists 32d7cf09b1c47c4cddafcb0ca30d0436 "create-flat-zip.cs" >}}

## Get a Free API License

You can get [a free temporary license][17] to use Aspose.ZIP for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to create a flat ZIP archive programmatically in C#. Particularly, we have demonstrated how to make a flat ZIP by extracting the inner ZIP archives into the parent ZIP. Apart from that, you can visit the [documentation][18] to read more about Aspose.ZIP for .NET. Also, you can share your queries with us via our [forum][19].

## See Also

*   [Add Files or Folders to ZIP Archives in C#][20]
*   [Unzip Files in ZIP Archives using C#][21]
*   [Merge Multiple ZIP or TAR Archives in C#][22]
*   [Create Executable Self-extracting Archive in C#][23]




[1]: https://docs.fileformat.com/compression/zip/
[2]: https://docs.fileformat.com/compression/zip/
[3]: #API-to-Create-Flat-ZIP-Archives
[4]: #Create-a-Flat-ZIP-Archive
[5]: https://products.aspose.com/zip/net/
[6]: https://www.nuget.org/packages/Aspose.ZIP
[7]: https://downloads.aspose.com/zip/net/
[8]: https://apireference.aspose.com/zip/net/aspose.zip/archive
[9]: https://apireference.aspose.com/zip/net/aspose.zip/archiveentry
[10]: https://apireference.aspose.com/zip/net/aspose.zip/archive/properties/entries
[11]: https://apireference.aspose.com/zip/net/aspose.zip/archiveentry/properties/name
[12]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream
[13]: https://docs.microsoft.com/en-gb/dotnet/api/system.io.stream.copyto?view=net-6.0#System_IO_Stream_CopyTo_System_IO_Stream_
[14]: https://apireference.aspose.com/zip/net/aspose.zip/archive/methods/deleteentry
[15]: https://apireference.aspose.com/zip/net/aspose.zip.archive/createentry/methods/1
[16]: https://apireference.aspose.com/zip/net/aspose.zip.archive/save/methods/1
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/zip/net/
[19]: https://forum.aspose.com/
[20]: https://blog.aspose.com/2020/04/22/create-zip-archives-add-files-or-folders-to-zip-in-csharp-asp.net/
[21]: https://blog.aspose.com/2020/04/23/unzip-files-in-password-protected-zip-archives-in-csharp-asp.net/
[22]: https://blog.aspose.com/2022/01/06/merge-zip-and-tar-files-in-csharp/
[23]: https://blog.aspose.com/2022/01/10/create-self-extracting-archive-in-csharp/




