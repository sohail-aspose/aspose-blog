---
title: 'Unzip Files in ZIP Archives using C#'
seoTitle: "C# Unzip Files Programmatically | Extract Protected ZIP | C# ZIP Extractor"
description: "Unzip files in C#. Extract password-protected ZIP files in C#. Extract ZIP archive and unzip single or multiple files in ASP.NET. C# ZIP extractor library."
date: Thu, 23 Apr 2020 16:04:07 +0000
draft: false
url: /2020/04/23/unzip-files-in-password-protected-zip-archives-in-csharp-asp.net/
author: Usman Aziz
summary: ''
tags: ['Extract ZIP archive in Csharp', 'Unzip files in CSharp', 'Unzip password-protected ZIP Files in Csharp', 'unzip single or multiple files in Csharp']
categories: ['Aspose.ZIP Product Family']
---



{{< figure align=center src="images/Unzip-Files-in-C.jpg" alt="Unzip Files in C#">}}


In the previous [post][1], you have learned different ways of zipping files and folders into [ZIP][2] archives using [Aspose.ZIP for .NET][3]. In this post, I'll show you how to **extract or unzip files in ZIP archives using [C#][4]**. We'll also cover how to **extract password-protected or AES encrypted ZIP archives programmatically**. This article is divided into the following sections:

*   [C# API to Unzip Files][5]
*   [Unzip files in ZIP archives in C#][6]
*   [Unzip password-protected ZIP files][7]
*   [Extract AES encrypted ZIP files in C#][8]

## C# API to Unzip Files {#CSharp-API-to-Unzip-Files}

Before we start, make sure you have [downloaded][9] and referenced Aspose.ZIP for .NET or installed its package using [NuGet Package Manager][10] in your project.

## Unzip ZIP Files using C# {#Unzip-files-in-ZIP-archives-in-CSharp}

The process of unzipping ZIP files could be achieved in two way:

*   Unzip each file in ZIP separately
*   Unzip files into a specified folder

In the first method, you can explicitly access and unzip each file in the ZIP archive. Furthermore, you can print the progress of the extraction process. Whereas, the second method simply unzips the files into the specified folder.

### Extract Each File in Archive Separately

The following are the steps to access and extract files and print the extraction progress in C#:

*   Open the ZIP archive into a [FileStream][11] object.
*   Create and initialize [Archive][12]'s instance with the _FileStream_ object.
*   Access files in the ZIP using [Archive.Entries][13] collection.
*   Set [ArchiveEntry.ExtractionProgressed][14] event handler to print the extraction progress.
*   Extract/unzip files using [ArchiveEntry.Extract(string)][15] method.

The following code sample shows how to extract files in a ZIP archive using C#.

{{< gist aspose-com-gists 5035e16331e147a3dc2b2261dc14d167 "unzip-files-in-zip-archive.cs" >}}

### Extract Files into a Folder

The following steps are used to extract files into a specific folder in C#.

*   Open the ZIP archive using the [FileStream][16] class.
*   Create an instance of [Archive][17] class and initialize it with ZIP's _FileStream_ object.
*   Unzip files using [Archive.ExtractToDirectory(string)][18] method.

The following C# code sample unzips files into a folder.

{{< gist aspose-com-gists 5035e16331e147a3dc2b2261dc14d167 "unzip-files-to-folder.cs" >}}

## Unzip Password-Protected ZIP Files in C# {#Unzip-password-protected-ZIP-files-in-CSharp}

You can also unzip a password-protected ZIP archive using Aspose.ZIP for .NET. For this, you only need to specify the password using the [ArchiveLoadOptions][19] class that will be passed as a second parameter to the _Archive_'s constructor.

The following is the sample code to unzip a password-protected ZIP file.

{{< gist aspose-com-gists 5035e16331e147a3dc2b2261dc14d167 "unzip-password-protected-zip-files.cs" >}}

## Extract AES Encrypted ZIP Files in C# {#Unzip-AES-encrypted-ZIP-files-in-CSharp}

A ZIP archive can also be encrypted with AES encryption. Aspose.ZIP for .NET supports encrypting archives with AES128, AES192, and AES256 encryption methods. Unzipping an AES encrypted ZIP file is similar to unzipping password-protected ZIP files. Just specify the decryption password using [ArchiveLoadOptions][20] class and rest will be taken care of by the API.

The following code sample shows how to unzip AES encrypted ZIP files in C#.

{{< gist aspose-com-gists 5035e16331e147a3dc2b2261dc14d167 "unzip-aes-encrypted-zip-files.cs" >}}

## Get a Free API License

You can use Aspose.ZIP for .NET without evaluation limitations by getting [a free temporary license][21].

## Conclusion

In this article, you have learned how to unzip ZIP files using C#. Furthermore, you have seen how to unzip files in password-protected ZIP archives. The code samples have also demonstrated how to extract files in an encrypted ZIP archive in C#. You can explore more about Aspose.ZIP for .NET using [documentation][22].

## Related Articles

*   [ZIP single or multiple files in C#][23]
*   [Merge Multiple ZIP or TAR Archives in C#][24]
*   [Create TAR.GZ and TAR.XZ Files in C#][25]




[1]: https://blog.aspose.com/2020/04/22/create-zip-archives-add-files-or-folders-to-zip-in-csharp-asp.net/
[2]: https://docs.fileformat.com/compression/zip/
[3]: https://products.aspose.com/zip/net
[4]: https://docs.fileformat.com/programming/cs/
[5]: #CSharp-API-to-Unzip-Files
[6]: #Unzip-files-in-ZIP-archives-in-CSharp
[7]: #Unzip-password-protected-ZIP-files-in-CSharp
[8]: #Unzip-AES-encrypted-ZIP-files-in-CSharp
[9]: https://downloads.aspose.com/zip/net
[10]: https://www.nuget.org/packages/Aspose.ZIP
[11]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream?view=netframework-4.8
[12]: https://apireference.aspose.com/zip/net/aspose.zip/archive
[13]: https://apireference.aspose.com/zip/net/aspose.zip/archive/properties/entries
[14]: https://apireference.aspose.com/zip/net/aspose.zip/archiveentry/events/extractionprogressed
[15]: https://apireference.aspose.com/zip/net/aspose.zip/archiveentry/methods/extract
[16]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream?view=netframework-4.8
[17]: https://apireference.aspose.com/zip/net/aspose.zip/archive
[18]: https://apireference.aspose.com/zip/net/aspose.zip/archive/methods/extracttodirectory
[19]: https://apireference.aspose.com/zip/net/aspose.zip/archiveloadoptions
[20]: https://apireference.aspose.com/zip/net/aspose.zip/archiveloadoptions
[21]: https://purchase.aspose.com/temporary-license
[22]: https://docs.aspose.com/zip/net
[23]: https://blog.aspose.com/2020/04/22/create-zip-archives-add-files-or-folders-to-zip-in-csharp-asp.net/
[24]: https://blog.aspose.com/2022/01/06/merge-zip-and-tar-files-in-csharp/
[25]: https://blog.aspose.com/2022/01/05/create-tar-gz-xz-files-in-csharp/





