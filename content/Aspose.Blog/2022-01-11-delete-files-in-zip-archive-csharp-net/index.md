---
title: 'Delete Files in a ZIP Archive in C# .NET'
seoTitle: "Delete Files inside ZIP Archive in C# .NET | Delete ZIP Files and Folders"
description: "Use .NET archiving API to delete files and folders inside ZIP archives in C# or VB.NET. Delete files using ArchiveEntry or index programmatically."
date: Tue, 11 Jan 2022 16:18:25 +0000
draft: false
url: /2022/01/11/delete-files-in-zip-archive-csharp-net/
author: Usman Aziz
summary: "While working with archives from within your .NET applications, you may need to manipulate files inside a [ZIP][1]. In the [previous post][2], you have seen how to add files/folders in a ZIP archive. In this article, you will learn **how to delete files inside the ZIP archives programmatically in C#**. So let's begin."
tags: ['Delete Files from ZIP Archives Csharp', 'Delete a ZIP folder programmatically in Csharp', 'Delete a directory in ZIP in Csharp net', 'Delete folders inside ZIP archives in csharp']
categories: ['Aspose.ZIP Product Family']
---



{{< figure align=center src="images/Delete-Files-in-ZIP-Archive.jpg" alt="Delete Files in a ZIP Archive in C# .NET">}}


While working with archives from within your .NET applications, you may need to manipulate files inside a [ZIP][3]. In the [previous post][4], you have seen how to add files/folders in a ZIP archive. In this article, you will learn **how to delete files inside the ZIP archives programmatically in C#**. So let's begin.

*   [.NET API to Delete Files from ZIP Archives][5]
*   [Delete Files from ZIP Archives][6]
    *   [Delete a File in a ZIP Archive using ArchiveEntry][7]
    *   [Remove a File in a ZIP Archive using Index][8]

## C# .NET API to Delete Files Inside ZIP Archives {#API-to-Delete-Files-from-ZIP-Archives}

[Aspose.ZIP for .NET][9] is a powerful API that provides a wide range of archiving features. It lets you create and manipulate archives of popular formats including ZIP, TAR, 7z, and GZip. We will use this API to delete the files inside ZIP archives dynamically. You can either install the API from [NuGet][10] or [download][11] the DLL and reference it manually.

```
PM> Install-Package Aspose.Zip 
```

## Delete Files Inside ZIP Archives in C# {#Delete-Files-from-ZIP-Archives}

There are two ways to delete files inside a ZIP archive using Aspose.ZIP for .NET. One is using the index of the file while the other is using the [ArchiveEntry][12] class. Let's see how to use both of the aforementioned methods.

### Delete a File in ZIP using ArchiveEntry {#Delete-a-File-inside-a-ZIP-Archive}

Aspose.ZIP for .NET represents each file/folder inside a ZIP as an **ArchiveEntry** object and all the files and folders make a collection of **ArchiveEntry** objects. Thus, to delete a file from ZIP, you can access and delete the relevant **ArchiveEntry** object from the collection. The following are the steps to delete a file from a ZIP archive in C#.

*   Load the ZIP archive using [Archive][13] class.
*   Loop through the entries in [Archive.Entries][14] collection.
*   Filter the desired files/folders and add them to a list.
*   Delete each entry in the list using [Archive.DeleteEntry(ArchvieEntry)][15] method.
*   Save the updated ZIP archive using [Archive.Save(string)][16] method.

The following code sample shows how to delete files inside a ZIP archive in C#.

{{< gist aspose-com-gists 3d1a4be10e21094fba8e54969909c3d3 "delete-file-in-zip-archive-entry.cs" >}}

## Delete a File in ZIP using Index {#Remove-a-File-in-ZIP-Archive-using-Index}

You can also delete the ZIP entries using their index. The following are the steps to remove a file/folder from a ZIP archive using its index.

*   Load the ZIP archive using [Archive][17] class.
*   Delete the file by specifying index in [Archive.DeleteEntry(int)][18] method.
*   Save the updated ZIP archive using [Archive.Save(string)][19] method.

The following C# code sample shows how to remove a file in a ZIP archive using its index.

{{< gist aspose-com-gists 3d1a4be10e21094fba8e54969909c3d3 "delete-file-in-zip-index.cs" >}}

## Get a Free API License

You can use Aspose.ZIP for .NET without evaluation limitations by getting [a free temporary license][20].

## Conclusion

In this article, you have learned how to delete files from ZIP archives in C#. With the help of code samples, we have seen how to delete files using the ArchiveEntry class or the index. In case you want to learn more about Aspose.ZIP for .NET, you can visit [documentation][21]. Also, you can ask your questions via our [forum][22].

## See Also

*   [Add Files or Folders to ZIP Archives in C#][23]
*   [Unzip Files in ZIP Archives using C#][24]
*   [Merge Multiple ZIP or TAR Archives in C#][25]
*   [Create Executable Self-extracting Archive in C#][26]




[1]: https://docs.fileformat.com/compression/zip/
[2]: https://blog.aspose.com/2020/04/22/create-zip-archives-add-files-or-folders-to-zip-in-csharp-asp.net/
[3]: https://docs.fileformat.com/compression/zip/
[4]: https://blog.aspose.com/2020/04/22/create-zip-archives-add-files-or-folders-to-zip-in-csharp-asp.net/
[5]: #API-to-Delete-Files-from-ZIP-Archives
[6]: #Delete-Files-from-ZIP-Archives
[7]: #Delete-a-File-inside-a-ZIP-Archive
[8]: #Remove-a-File-in-ZIP-Archive-using-Index
[9]: https://products.aspose.com/zip/net/
[10]: https://www.nuget.org/packages/Aspose.ZIP
[11]: https://downloads.aspose.com/zip/net/
[12]: https://apireference.aspose.com/zip/net/aspose.zip/archiveentry
[13]: https://apireference.aspose.com/zip/net/aspose.zip/archive
[14]: https://apireference.aspose.com/zip/net/aspose.zip/archive/properties/entries
[15]: https://apireference.aspose.com/zip/net/aspose.zip/archive/methods/deleteentry
[16]: https://apireference.aspose.com/zip/net/aspose.zip.archive/save/methods/1
[17]: https://apireference.aspose.com/zip/net/aspose.zip/archive
[18]: https://apireference.aspose.com/zip/net/aspose.zip/archive/methods/deleteentry
[19]: https://apireference.aspose.com/zip/net/aspose.zip.archive/save/methods/1
[20]: https://purchase.aspose.com/temporary-license
[21]: https://docs.aspose.com/zip/net/
[22]: https://forum.aspose.com/
[23]: https://blog.aspose.com/2020/04/22/create-zip-archives-add-files-or-folders-to-zip-in-csharp-asp.net/
[24]: https://blog.aspose.com/2020/04/23/unzip-files-in-password-protected-zip-archives-in-csharp-asp.net/
[25]: https://blog.aspose.com/2022/01/06/merge-zip-and-tar-files-in-csharp/
[26]: https://blog.aspose.com/2022/01/10/create-self-extracting-archive-in-csharp/




