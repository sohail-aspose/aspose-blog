---
title: 'Convert RAR Files to ZIP Archive in C#'
seoTitle: "Convert RAR to ZIP in C# .NET | RAR to ZIP Converter Library"
description: "Use .NET archiving API to convert RAR files to ZIP archive in C#. Download the library and embed the provided source code for RAR to ZIP conversion in .NET."
date: Fri, 14 Jan 2022 09:50:47 +0000
draft: false
url: /2022/01/14/convert-rar-files-to-zip-in-csharp/
author: Usman Aziz
summary: '[RAR][1] is a commonly used archive file format that supports lossless compression of data. Often, people prefer RAR over [ZIP][2] because it provides a better compression rate and keeps the archive size smaller. However, in certain cases, you may need to convert RAR files to ZIP archives. To achieve that, this article covers **how to convert a RAR file to ZIP programmatically in C#**.'
tags: ['Convert RAR to ZIP', 'Convert RAR to ZIP Csharp', 'Convert RAR to ZIP Programmatically', 'Dotnet RAR to ZIP Converter']
categories: ['Aspose.ZIP Product Family']
---



{{< figure align=center src="images/Convert-RAR-to-ZIP.png" alt="Convert RAR Files to ZIP Archive in C#">}}


[RAR][3] is a commonly used archive file format that supports lossless compression of data. Often, people prefer RAR over [ZIP][4] because it provides a better compression rate and keeps the archive size smaller. However, in certain cases, you may need to convert RAR files to ZIP archives. To achieve that, this article covers **how to convert a RAR file to ZIP programmatically in C#**.

*   [.NET API for RAR to ZIP Conversion][5]
*   [Convert a RAR File to ZIP Archvie][6]

## C# .NET API for RAR to ZIP Conversion {#API-for-RAR-to-ZIP-Conversion}

[Aspose.ZIP for .NET][7] is a powerful archiving API that supports the creation and manipulation of popular archive formats. We will utilize this API to convert the RAR files to ZIP format. To use the API, you can install it from [NuGet][8] or download its DLL from the [downloads section][9].

```
PM> Install-Package Aspose.Zip
```

## Convert a RAR File to ZIP in C# {#Convert-a-RAR-File-to-ZIP}

The RAR files can be converted to ZIP format within a few steps using Aspose.ZIP for .NET. The following are the steps to convert a RAR file to a ZIP archive in C#.

*   Create an instance of [Archive][10] class for ZIP archive.
*   Load the RAR archive using [RarArchive][11] class.
*   Loop through the entries of RAR archive using [RarArchive.Entries][12] collection.
*   For each entry in RAR, perform the following steps:
    
    *   Extract the entry to [MemoryStream][13] object using [RarArchive.Entries\[int\].Extract(MemoryStream)][14] method.
    
    *   Add the entry to ZIP using [Archive.CreateEntry(String, MemoryStream)][15] method.
*   Finally, save the resultant ZIP archive using [Archive.Save(String)][16] method.

The following code sample shows how to convert a RAR file to ZIP format in C#.

{{< gist aspose-com-gists 9d4019d37d8b0b33d7e992bf09ace706 "convert-rar-to-zip.cs" >}}

## Get a Free API License

You can get [a free temporary license][17] to use Aspose.ZIP for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to convert a RAR archive to ZIP format programmatically in C#. The step-by-step guide and code sample have demonstrated the conversion of a RAR file to a ZIP archive within a few steps. You can read the [documentation][18] of Aspose.ZIP for .NET to explore other features. Moreover, you can share your queries with us via our [forum][19].

## See Also

*   [Add Files or Folders to ZIP Archives in C#][20]
*   [Unzip Files in ZIP Archives using C#][21]
*   [Merge Multiple ZIP or TAR Archives in C#][22]
*   [Create Executable Self-extracting Archive in C#][23]




[1]: https://docs.fileformat.com/compression/rar/
[2]: https://docs.fileformat.com/compression/zip/
[3]: https://docs.fileformat.com/compression/rar/
[4]: https://docs.fileformat.com/compression/zip/
[5]: #API-for-RAR-to-ZIP-Conversion
[6]: #Convert-a-RAR-File-to-ZIP
[7]: https://products.aspose.com/zip/net/
[8]: https://www.nuget.org/packages/Aspose.ZIP
[9]: https://downloads.aspose.com/zip/net/
[10]: https://apireference.aspose.com/zip/net/aspose.zip/archive
[11]: https://apireference.aspose.com/zip/net/aspose.zip.rar/rararchive
[12]: https://apireference.aspose.com/zip/net/aspose.zip.rar/rararchive/properties/entries
[13]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream
[14]: https://apireference.aspose.com/zip/net/aspose.zip.rar/rararchiveentry/methods/extract
[15]: https://apireference.aspose.com/zip/net/aspose.zip.archive/createentry/methods/1
[16]: https://apireference.aspose.com/zip/net/aspose.zip/archive/methods/save
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/zip/net/
[19]: https://forum.aspose.com/
[20]: https://blog.aspose.com/2020/04/22/create-zip-archives-add-files-or-folders-to-zip-in-csharp-asp.net/
[21]: https://blog.aspose.com/2020/04/23/unzip-files-in-password-protected-zip-archives-in-csharp-asp.net/
[22]: https://blog.aspose.com/2022/01/06/merge-zip-and-tar-files-in-csharp/
[23]: https://blog.aspose.com/2022/01/10/create-self-extracting-archive-in-csharp/




