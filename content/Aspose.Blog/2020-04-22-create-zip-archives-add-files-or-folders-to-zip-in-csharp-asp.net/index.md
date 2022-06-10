---
title: 'Add Files or Folders to ZIP Archives Programmatically in C#'
seoTitle: "Create ZIP Archive in C# | ZIP Single or Multiple Files in C# | ZIP Library"
description: "C# Create ZIP files. ZIP single or multiple files. Create AES encrypted ZIP archive to compress files or folders. Create password-protected ZIP files in C#."
date: Wed, 22 Apr 2020 12:48:02 +0000
draft: false
url: /2020/04/22/create-zip-archives-add-files-or-folders-to-zip-in-csharp-asp.net/
author: Usman Aziz
summary: ''
tags: ['Add multiple files to ZIP csharp', 'Add single file to ZIP csharp', 'Create AES encrypted ZIP files', 'Create ZIP Archives in Csharp', 'Csharp ASP.NET ZIP Library']
categories: ['Aspose.ZIP Product Family']
---



{{< figure align=center src="images/Create-ZIP-in-C.jpg" alt="Create ZIP in C#">}}


The **[ZIP][1] archives** are used to compress and keep one or more files or folders into a single container. A ZIP archive encapsulates the files and folders as well as holds their metadata information. The most common usage of archiving is reducing the size of the files for storage or transmission and applying encryption for security. Apart from the file compression tools, the automated compression/extraction features are also used within various desktop and web applications for uploading, downloading, sharing, or encrypting the files. This article also targets similar scenarios and presents some easy ways of **compressing files or folders** and **creating ZIP archives** **programmatically** using **[C#][2]**.

In this article, you will learn how to perform the following ZIP archiving operations:

*   [Create a ZIP archive using C#][3]
*   [Add multiple files to a ZIP archive][4]
*   [Add folders to a ZIP archive][5]
*   [Create a password-protected ZIP archive using ZipCrypto][6]
*   [Encrypt ZIP archive with AES encryption][7]
*   [Set parallel compression mode][8]

## Prerequisite - C# ZIP Library

[Aspose.ZIP for .NET][9] is a powerful and easy to use API for zipping or unzipping files and folders within .NET applications. It also provides AES encryption techniques to encrypt the files in ZIP archives. You can install the API from [NuGet][10] or download its binaries from the [Downloads][11] section.

## Create a ZIP Archive in C# {#Create-a-ZIP-archive-using-CSharp}

The following are the steps to compress a file by adding it into a ZIP archive:

*   Create a [FileStream][12] object for the output ZIP archive.
*   Open the source file into a _FileStream_ object.
*   Create an object of [Archive][13] class.
*   Add the file into the archive using [Archive.CreateEntry(string, FileStream)][14] method.
*   Create the ZIP archive using [Archive.Save(FileStream)][15] method.

The following code sample shows how to add a file into a ZIP archive using C#.

{{< gist aspose-com-gists dea0000f742629e43ecc24f5a19ab2ac "create-zip-archive-in-csharp.cs" >}}

## Add Multiple Files into ZIP Archive in C# {#Add-multiple-files-to-a-ZIP-archive}

In case you want to add multiple files into a ZIP archive, you can do it using one of the following ways.

### ZIP Multiple Files using FileStream

In this method, the _FileStream_ class is used to add files to the ZIP archive using [Archive.CreateEntry(String, FileStream)][16] method. The following code sample shows how to add multiple files into a ZIP in C#.

{{< gist aspose-com-gists dea0000f742629e43ecc24f5a19ab2ac "add-mulitple-files-to-zip.cs" >}}

### ZIP Multiple Files using FileInfo

You can also use the [FileInfo][17] class for adding multiple files into a ZIP archive. In this method, the files will be loaded using the _FileInfo_ class and added to the ZIP archive using [Archive.CreateEntry(String, FileInfo)][18] method. The following code sample shows how to ZIP multiple files using the _FileInfo_ class in C#.

{{< gist aspose-com-gists dea0000f742629e43ecc24f5a19ab2ac "add-mulitple-files-to-zip-fileinfo.cs" >}}

### ZIP Files using Path

Instead of using _FileInfo_ or _FileStream_ classes for the ZIP entries, you can provide the file's path directly to [Archive.CreateEntry(String name, String path, Boolean openImmediately, ArchiveEntrySettings newEntrySettings)][19] method. The following code sample shows how to ZIP files using their path.

{{< gist aspose-com-gists dea0000f742629e43ecc24f5a19ab2ac "add-files-to-zip-filepath.cs" >}}

## Add Folders to a ZIP Archive in C# {#Add-folders-to-a-ZIP-archive}

You can ZIP a folder as well which could be another alternative of adding multiple files to a ZIP archive. Just put the source files into a folder and add that folder to the ZIP archive. The following are the steps to ZIP a folder:

*   Create an object of [FileStream][20] class for the output ZIP archive.
*   Create an instance of the [Archive][21] class.
*   Use the [DirectoryInfo][22] class to specify the folder to be zipped.
*   Use [Archive.CreateEntries(DirectoryInfo)][23] method to add folder into ZIP.
*   Create the ZIP archive using [Archive.Save(FileStream)][24] method.

The following code sample shows how to add a folder to ZIP in C#.

{{< gist aspose-com-gists dea0000f742629e43ecc24f5a19ab2ac "compress-folder-into-zip.cs" >}}

## Create a Password Protected ZIP using ZipCrypto in C# {#Create-a-Password-Protected-ZIP-Archive-using-ZipCrypto-in-CSharp}

You can protect the ZIP archives using passwords and apply ZipCrypto encryption. For this, the [ArchiveEntrySettings][25] class is used in the constructor of the [Archive][26] that accepts the encryption type as the second parameter.

The following code sample shows how to create a password-protected ZIP archive using ZipCrypto in C#.

{{< gist aspose-com-gists dea0000f742629e43ecc24f5a19ab2ac "create-password-protected-zip.cs" >}}

## C# Create Password Protected ZIP with AES Encryption {#Create-AES-Encrypted-ZIP-Archives-in-CSharp}

Aspose.ZIP for .NET also lets you apply AES encryption to protect the ZIP archives. You can use the following AES encryption methods:

*   AES128
*   AES192
*   AES256

In order to apply AES encryption, API offers the [AesEcryptionSettings][27] class. The following code sample shows how to create a password protected ZIP with AES encryption in C#.

{{< gist aspose-com-gists dea0000f742629e43ecc24f5a19ab2ac "encrypt-zip-with-aes-encryption.cs" >}}

## Set Parallel Compression Mode {#Set-parallel-compression-mode}

You can also configure the API for parallel compression in case of multiple entries. For this, you can specify the parallel compression mode using [ParallelOptions][28] class. Aspose.ZIP for .NET provides the following parallel compression modes.

*   Never - Do not compress in parallel.
*   Always - Do compress in parallel (beware out of memory).
*   Auto - Decide whether to use parallel compression or not upon the entries. This option may compress some entries in parallel only.

The following code sample shows how to set parallel compression mode while zipping multiple files.

{{< gist aspose-com-gists 42ee14864d84aeae8619284450c3d628 "Examples-CSharp-CompressingAndDecompressingFiles-UsingParallelismToCompressFiles-UsingParallelismToCompressFiles.cs" >}}

## Learn more about Aspose.ZIP for .NET

Explore more about our C# ZIP API using the following resources:

*   [Documentation][29]
*   [Source code examples][30]

## Conclusion

In this article, you have learned how to create ZIP archives programmatically in C#. The code samples have demonstrated how to add files and folders in the ZIP archives. In addition, we have also covered how to create password-protected ZIP archives with ZipCrypto and AES encryption methods in C#. Alongside, parallel compression of multiple entries is also discussed at the end. In case you would have any questions or queries, you can ask us via our [forum][31].

## See also

*   [Unrar or Extract Files using C#][32]
*   [Unzip Files in ZIP Archives using C#][33]
*   [Create 7z (7-Zip) Archives in C# .NET][34]
*   [Open or Extract 7z (7zip) File in C# .NET][35]
*   [Create and Extract GZip Archives using C#][36]




[1]: https://docs.fileformat.com/compression/zip/
[2]: https://docs.fileformat.com/programming/cs/
[3]: #Create-a-ZIP-archive-using-CSharp
[4]: #Add-multiple-files-to-a-ZIP-archive
[5]: #Add-folders-to-a-ZIP-archive
[6]: #Create-a-Password-Protected-ZIP-Archive-using-ZipCrypto-in-CSharp
[7]: #Create-AES-Encrypted-ZIP-Archives-in-CSharp
[8]: #Set-parallel-compression-mode
[9]: https://products.aspose.com/zip/net
[10]: https://www.nuget.org/packages/Aspose.ZIP
[11]: https://downloads.aspose.com/zip/net
[12]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream?view=netframework-4.8
[13]: https://apireference.aspose.com/zip/net/aspose.zip/archive
[14]: https://apireference.aspose.com/zip/net/aspose.zip.archive/createentry/methods/1
[15]: https://apireference.aspose.com/zip/net/aspose.zip/archive/methods/save
[16]: https://apireference.aspose.com/zip/net/aspose.zip.archive/createentry/methods/1
[17]: https://docs.microsoft.com/en-us/dotnet/api/system.io.fileinfo?view=netframework-4.8
[18]: https://apireference.aspose.com/zip/net/aspose.zip/archive/methods/createentry
[19]: https://apireference.aspose.com/zip/net/aspose.zip.archive/createentry/methods/3
[20]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream?view=netframework-4.8
[21]: https://apireference.aspose.com/zip/net/aspose.zip/archive
[22]: https://docs.microsoft.com/en-us/dotnet/api/system.io.directoryinfo?view=netframework-4.8
[23]: https://apireference.aspose.com/zip/net/aspose.zip/archive/methods/createentries
[24]: https://apireference.aspose.com/zip/net/aspose.zip/archive/methods/save
[25]: https://apireference.aspose.com/net/zip/aspose.zip.saving/archiveentrysettings
[26]: https://apireference.aspose.com/zip/net/aspose.zip/archive
[27]: https://apireference.aspose.com/zip/net/aspose.zip.saving/aesecryptionsettings
[28]: https://apireference.aspose.com/zip/net/aspose.zip.saving/paralleloptions
[29]: https://docs.aspose.com/display/zipnet/Getting+Started
[30]: https://github.com/aspose-zip/Aspose.ZIP-for-.NET
[31]: https://forum.aspose.com/
[32]: https://blog.aspose.com/2021/04/15/unrar-extract-rar-extractor-opener-in-csharp-asp.net/
[33]: https://blog.aspose.com/2020/04/23/unzip-files-in-password-protected-zip-archives-in-csharp-asp.net/
[34]: https://blog.aspose.com/2020/05/06/create-7zip-archives-programmatically-using-csharp-asp.net/
[35]: https://blog.aspose.com/2021/04/28/open-extract-7zip-7z-file-unzip-in-csharp-asp-net/
[36]: https://blog.aspose.com/2021/05/07/create-and-extract-gzip-archives-using-csharp/





