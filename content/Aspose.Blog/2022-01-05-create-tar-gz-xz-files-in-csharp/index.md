---
title: 'Create TAR.GZ and TAR.XZ Files in C#'
date: Wed, 05 Jan 2022 03:29:00 +0000
draft: false
url: /2022/01/05/create-tar-gz-xz-files-in-csharp/
author: ''Usman Aziz''
summary: "[TAR][1] is a popular UNIX-based archiving format that is used to package multiple files including audios, videos, installers, etc. On the other hand, GNU is a data compression algorithm to compress large files before sharing. The TAR.GZ is the combination of TAR's archiving and GNU's compression. Similarly, [XZ Utils][2] also provides compression of TAR archives as TAR.XZ format. In this article, you will learn **how to compress TAR archives and create TAR.GZ and TAR.XZ files in C#**."
tags: ['Compress TAR Archives in Csharp', 'Create a TAR GZ File in Csharp', 'Create a TAR XZ File in Csharp']
categories: ['Aspose.ZIP Product Family']
---



{{< figure align=center src="images/Create-Archive.jpg" alt="Create TAR.GZ and TAR.XZ Files in C#">}}


[TAR][3] is a popular UNIX-based archiving format that is used to package multiple files including audios, videos, installers, etc. On the other hand, GNU is a data compression algorithm to compress large files before sharing. The TAR.GZ is the combination of TAR's archiving and GNU's compression. Similarly, [XZ Utils][4] also provides compression of TAR archives as TAR.XZ format. In this article, you will learn **how to compress TAR archives and create TAR.GZ and TAR.XZ files in C#**.

*   [C# API to Compress TAR Archives][5]
*   [Create a TAR.GZ File in C#][6]
*   [Create a TAR.XZ File in C#][7]

## C# .NET API to Create TAR.GZ and TAR.XZ {#API-to-Create-tar-gz-Archive}

[Aspose.ZIP for .NET][8] is a powerful API that allows you to create archives seamlessly from within your .NET applications. Furthermore, it lets you decompress and extract the archives of popular formats including ZIP, TAR, GZIP, BZ2, 7Zip, and RAR. We will use this API to create compressed TAR archives (**.tar.gz** and **.tar.xz**). You can either [download][9] the API's DLL or install it directly using [NuGet][10].

```
PM> Install-Package Aspose.Zip
```

## Create a TAR.GZ File in C# {#Create-a-TAR-GZ-File}

The following are the steps to create a compressed TAR file (tar.gz) in C#.

*   Create an object of [TarArchive][11] class.
*   Add files to archive using [TarArchive.CreateEntry(string, string)][12] method.
*   Save the archive as TAR.GZ using [TarArchive.SaveGzipped(string)][13] method.

The following code sample shows how to create a TAR.GZ file in C#.

{{< gist aspose-com-gists 7d70833d03a4a84b810f2b641c30547d "create-tar-gz.cs" >}}

## Create a TAR.XZ File in C# {#Create-a-TAR-XZ-File}

[XZ Utils][14] is a popular utility that provides compression and decompression services. It compresses the TAR archives into TAR.XZ format. Aspose.ZIP for .NET also supports compression of TAR archives into TAR.XZ. The following are the steps to create a **.tar.xz** file in C#.

*   Create a new [FileStream][15] object for **.tar.xz** file.
*   Create an object of [TarArchive][16] class.
*   Add files to archive using [TarArchive.CreateEntry(string, string)][17] method.
*   Save archive as TAR.XZ using [TarArchive.SaveXzCompressed(Stream)][18] method.

The following code sample shows how to compress TAR into TAR.XZ format in C#.

{{< gist aspose-com-gists 7d70833d03a4a84b810f2b641c30547d "create-tar-xz.cs" >}}

## Get a Free API License

You can [get a free temporary license][19] in order to use the API without evaluation limitations.

## Conclusion

The compression and decompression of TAR archives are commonly performed on Unix/Linux operating systems. In this article, you have learned how to compress TAR archives and create TAR.GZ and TAR.XZ files in C#. You can simply install the API and integrate the provided code samples in your .NET applications to compress TAR archives. Furthermore, you can visit the [documentation][20] to explore more about Aspose.ZIP for .NET. Also, you can post your queries to our [forum][21].

## See Also

*   [Add Files or Folders to ZIP Archives in C#][22]
*   [Unzip Files in ZIP Archives using C#][23]




[1]: https://docs.fileformat.com/compression/tar/
[2]: https://en.wikipedia.org/wiki/XZ_Utils
[3]: https://docs.fileformat.com/compression/tar/
[4]: https://en.wikipedia.org/wiki/XZ_Utils
[5]: #API-to-Create-tar-gz-Archive
[6]: #Create-a-TAR-GZ-File
[7]: #Create-a-TAR-XZ-File
[8]: https://products.aspose.com/zip/net/
[9]: https://downloads.aspose.com/zip/net/
[10]: https://www.nuget.org/packages/Aspose.ZIP
[11]: https://apireference.aspose.com/zip/net/aspose.zip.tar/tararchive
[12]: https://apireference.aspose.com/zip/net/aspose.zip.tar.tararchive/createentry/methods/2
[13]: https://apireference.aspose.com/zip/net/aspose.zip.tar.tararchive/savegzipped/methods/1
[14]: https://en.wikipedia.org/wiki/XZ_Utils
[15]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream
[16]: https://apireference.aspose.com/zip/net/aspose.zip.tar/tararchive
[17]: https://apireference.aspose.com/zip/net/aspose.zip.tar.tararchive/createentry/methods/2
[18]: https://apireference.aspose.com/zip/net/aspose.zip.tar/tararchive/methods/savexzcompressed
[19]: https://purchase.aspose.com/temporary-license
[20]: https://docs.aspose.com/zip/net/getting-started/
[21]: https://forum.aspose.com/
[22]: https://blog.aspose.com/2020/04/22/create-zip-archives-add-files-or-folders-to-zip-in-csharp-asp.net/
[23]: https://blog.aspose.com/2020/04/23/unzip-files-in-password-protected-zip-archives-in-csharp-asp.net/




