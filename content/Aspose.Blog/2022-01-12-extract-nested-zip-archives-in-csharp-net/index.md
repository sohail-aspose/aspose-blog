---
title: 'Extract Nested ZIP Archives in C#'
seoTitle: "Extract Nested ZIP Archives in C# .NET | Unzip Nested ZIP Files in C#"
description: "Use .NET archiving API to extract nested ZIP archives using C# or VB.NET. Unzip the archives encapsulated in another ZIP archive programmatically."
date: Wed, 12 Jan 2022 15:02:35 +0000
draft: false
url: /2022/01/12/extract-nested-zip-archives-in-csharp-net/
author: Usman Aziz
summary: 'We often come across the scenario where multiple [ZIP][1] archives are encapsulated inside another ZIP. In such cases, first, you have to extract the parent ZIP and then the nested archives one by one. To make things easier for you, in this article, we will demonstrate **how to extract the nested ZIP archives in C# .NET** without writing complex code.'
tags: ['Dotnet API to Extract Nested ZIP Archives', 'Extract Nested ZIP Archives in Csharp', 'Open Nested ZIP Archives in CSharp', 'Unzip Nested ZIP Archives in Csharp']
categories: ['Aspose.ZIP Product Family']
---



{{< figure align=center src="images/Unzip-Nested-ZIP-Archives-1.png" alt="">}}


We often come across the scenario where multiple [ZIP][2] archives are encapsulated inside another ZIP. In such cases, first, you have to extract the parent ZIP and then the nested archives one by one. To make things easier for you, in this article, we will demonstrate **how to extract the nested ZIP archives in C# .NET** without writing complex code.

*   [.NET API to Extract Nested ZIP Archives][3]
*   [Unzip Nested ZIP Archives in C#][4]

## C# .NET API to Extract Nested ZIP Archives {#API-to-Extract-Nested-ZIP-Archives}

To unzip the nested ZIP archives, we will utilize [Aspose.ZIP for .NET][5]. The API is designed to perform archiving operations from within the .NET applications. It allows you to create and manipulate popular archive formats seamlessly. You can either [download][6] the API's DLL or install it using [NuGet][7].

```
PM> Install-Package Aspose.Zip
```

## Extract Nested ZIP Archives in C# {#Unzip-Nested-ZIP-Archives}

To demonstrate the extraction of nested ZIP archives, we have created the following ZIP file which contains 3 entries.



{{< figure align=center src="images/Nested-ZIP-Archive.png" alt="Nested ZIP Archives" caption="Nested ZIP Archives">}}


We will extract each nested ZIP archive and save its content in a separate folder. The following are the steps to extract nested ZIP archives in C#.

*   First, create a [FileStream][8] object to load ZIP file.
*   Then, load ZIP file using [Archive][9] class.
*   Iterate through each [ArchiveEntry][10] in [Archive.Entries][11] collection.
*   Filter the ZIP archives in the collection and for each archive perform following steps:
    *   Create a [MemoryStream][12] object and copy the archive entry into it using [ArchiveEntry.Open().CopyTo(Stream)][13] method.
    *   Create an instance of [Archive][14] class to load the nested archive.
    *   Finally, extract archive into a folder using [Archive.ExtractToDirectory(string)][15] method.

The following code sample shows how to unzip nested ZIP archives in C# .NET.

{{< gist aspose-com-gists 8824e9c135d78f07ef109019d9d9174e "extract-nested-zip.cs" >}}

The following is the screenshot of the extracted ZIP archives.



{{< figure align=center src="images/Extract-Nested-ZIP-Archives.png" alt="Extracting nested ZIP archives in C# .NET" caption="Unzipped Nested Archives">}}


## Get a Free API License

You can get [a free temporary license][16] to use Aspose.ZIP for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to extract nested ZIP archives in C#. The step-by-step guide and code sample have demonstrated how to unzip each nested archive into a separate folder. Besides, you can visit [documentation][17] to explore other features of Aspose.ZIP for .NET. Also, you can ask your questions via our [forum][18].

## See Also

*   [Add Files or Folders to ZIP Archives in C#][19]
*   [Unzip Files in ZIP Archives using C#][20]
*   [Merge Multiple ZIP or TAR Archives in C#][21]
*   [Create Executable Self-extracting Archive in C#][22]




[1]: https://docs.fileformat.com/compression/zip/
[2]: https://docs.fileformat.com/compression/zip/
[3]: #API-to-Extract-Nested-ZIP-Archives
[4]: #Unzip-Nested-ZIP-Archives
[5]: https://products.aspose.com/zip/net/
[6]: https://downloads.aspose.com/zip/net/
[7]: https://www.nuget.org/packages/Aspose.ZIP
[8]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream
[9]: https://apireference.aspose.com/zip/net/aspose.zip/archive
[10]: https://apireference.aspose.com/zip/net/aspose.zip/archiveentry
[11]: https://apireference.aspose.com/zip/net/aspose.zip/archive/properties/entries
[12]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream
[13]: https://docs.microsoft.com/en-gb/dotnet/api/system.io.stream.copyto?view=net-6.0#System_IO_Stream_CopyTo_System_IO_Stream_
[14]: https://apireference.aspose.com/zip/net/aspose.zip/archive
[15]: https://apireference.aspose.com/zip/net/aspose.zip/archive/methods/extracttodirectory
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/zip/net/
[18]: https://forum.aspose.com/
[19]: https://blog.aspose.com/2020/04/22/create-zip-archives-add-files-or-folders-to-zip-in-csharp-asp.net/
[20]: https://blog.aspose.com/2020/04/23/unzip-files-in-password-protected-zip-archives-in-csharp-asp.net/
[21]: https://blog.aspose.com/2022/01/06/merge-zip-and-tar-files-in-csharp/
[22]: https://blog.aspose.com/2022/01/10/create-self-extracting-archive-in-csharp/




