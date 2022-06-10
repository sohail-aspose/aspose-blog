---
title: 'Create 7z (7-Zip) Archives Programmatically using C# .NET'
seoTitle: "Create 7zip Archive using C# .NET | Create AES Encrypted 7z Files in C#"
description: "Create 7zip (.7z) archive programmatically using C# or VB.NET. Apply AES encryption to 7zip archives and set a password for file in 7zip archives using C#."
date: Wed, 06 May 2020 17:15:21 +0000
draft: false
url: /2020/05/06/create-7zip-archives-programmatically-using-csharp-asp.net/
author: Usman Aziz
summary: ''
tags: ['create 7z archive using csharp', 'create 7zip archive using csharp', 'create encrypted 7zip archive using csharp']
categories: ['Aspose.ZIP Product Family']
---



{{< figure align=center src="images/Create-7Zip-Archive-in-C.jpg" alt="Create 7Zip Archive in C#">}}


In the [previous post][1], I have discussed different ways of creating [ZIP][2] archives using [C#][3]. The article also covered how to create encrypted and password-protected ZIP archives. Besides ZIP format, there are some other commonly used archive formats such as [7z][4], [tar][5], [RAR][6], etc. Among these, 7z archive format is based on open-source architecture and it is used to compress files and folders with a high compression ratio. It also supports 256-bit AES encryption and allows encrypting the files' names as well. In this article, I'll demonstrate how to create 7z (7-Zip) archives programmatically using C#.

This article is divided into the following sections:

*   [Create a 7z (7-Zip) Archive using C#][7]
*   [Create an AES Encrypted 7z Archive using C#][8]
*   [Set Different Passwords for 7z Entries using C#][9]

All the steps and code samples in this article are based on [Aspose.ZIP for .NET][10]. Therefore, make sure you have installed the API using either of the following methods:

*   Install using [NuGet Package Manager][11].
*   [Download][12] DLL and add its reference to the project.

## Create 7z (7-Zip) Archive using C# {#Create-a-7z-7Zip-Archive-using-Csharp}

There could be two possible scenarios of compressing files into a 7z archive. Either you have only a single file or there could be a bunch of files to be compressed. You can deal with both of the scenarios explicitly.

### Create 7z Archive with Single Entry

The following are the steps to create a 7z archive with a single entry.

*   Open a new [FileStream][13] to create a 7z file.
*   Create an instance of the [SevenZipArchive][14] class.
*   Add file to the archive using [SevenZipArchive.CreateEntry(String, String, Boolean, SevenZipEntrySettings)][15] method.
*   Create and save archive using [SevenZipArchive.Save(Stream)][16] method.

The following code sample shows how to create a 7z (7-Zip) archive using C#.

{{< gist aspose-com-gists 42ee14864d84aeae8619284450c3d628 "Examples-CSharp-WorkingWithSevenZip-CreateSevenZipEntry-CreateSevenZipEntry.cs" >}}

### Create 7z Archive with Multiple Entries

In this case, you can put the files in a folder and pass the folder's path to [SevenZipArchive.CreateEntries()][17] method. The following are steps to add multiple file entries to a 7z archive.

*   Create an instance of the [SevenZipArchive][18] class.
*   Pass the folder's path to [SevenZipArchive.CreateEntries(String, Boolean)][19] method.
*   Call [SevenZipArchive.Save(String)][20] method.

The following code sample shows how to create a 7z archive with multiple entries using C#.

{{< gist aspose-com-gists 42ee14864d84aeae8619284450c3d628 "Examples-CSharp-WorkingWithSevenZip-CreateSevenZipEntries-CreateSevenZipEntries.cs" >}}

## Create an AES Encrypted 7z Archive using C# {#Create-an-AES-Encrypted-7z-Archive-using-Csharp}

7z format supports AES encryption to secure the files. In order to encrypt a 7z file, the [SevenZipAESEncryptionSettings][21] class is used. The following code sample shows how to create an AES encrypted 7z archive using C#.

{{< gist aspose-com-gists 42ee14864d84aeae8619284450c3d628 "Examples-CSharp-WorkingWithSevenZip-AESEncryptionSettings-AESEncryptionSettings.cs" >}}

## Set Different Passwords for 7z Entries using C# {#Set-Different-Password-for-7z-Entries-using-Csharp}

7z format also allows you to specify a different password for every file entry. For instance, if you are going to compress two files in a 7z archive, you can specify a different password for each file. The following are the steps to set different passwords for 7z entries.

*   Create a new [FileStream][22] for the 7z archive file.
*   Access every file entry using the [FileInfo][23] class.
*   Create an instance of the [SevenZipArchive][24] class.
*   Create entry into 7z archive using [SevenZipArchive.CreateEntry(String, FileInfo, Boolean, SevenZipEntrySettings)][25]
*   Save the archive using [SevenZipArchive.Save(Stream)][26] method.

The following code sample shows how to set a password for every entry in a 7z archive.

{{< gist aspose-com-gists 42ee14864d84aeae8619284450c3d628 "Examples-CSharp-WorkingWithSevenZip-EntriesWithDifferentPasswords-EntriesWithDifferentPasswords.cs" >}}

## Conclusion

In this article, we have learned how to create 7z archives programmatically using C#. In addition, we have seen how to create AES encrypted 7z files and set a password for every file entry. You can learn more about compression/decompression of files from [here][27].

## Related Articles

*   [ZIP Files and Folders using C#][28]
*   [Unzip Files in ZIP Archives using C#][29]




[1]: https://blog.aspose.com/2020/04/22/create-zip-archives-add-files-or-folders-to-zip-in-csharp-asp.net/
[2]: https://docs.fileformat.com/compression/zip/
[3]: https://docs.fileformat.com/programming/cs/
[4]: https://docs.fileformat.com/compression/7z/
[5]: https://docs.fileformat.com/compression/tar/
[6]: https://docs.fileformat.com/compression/rar/
[7]: #Create-a-7z-7Zip-Archive-using-Csharp
[8]: #Create-an-AES-Encrypted-7z-Archive-using-Csharp
[9]: #Set-Different-Password-for-7z-Entries-using-Csharp
[10]: https://products.aspose.com/zip/net
[11]: http://nuget.org/packages/Aspose.zip
[12]: https://downloads.aspose.com/zip/net
[13]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream
[14]: https://apireference.aspose.com/zip/net/aspose.zip.sevenzip/sevenziparchive
[15]: https://apireference.aspose.com/zip/net/aspose.zip.sevenzip.sevenziparchive/createentry/methods/3
[16]: https://apireference.aspose.com/zip/net/aspose.zip.sevenzip/sevenziparchive/methods/save
[17]: https://apireference.aspose.com/zip/net/aspose.zip.sevenzip.sevenziparchive/createentries/methods/1
[18]: https://apireference.aspose.com/zip/net/aspose.zip.sevenzip/sevenziparchive
[19]: https://apireference.aspose.com/zip/net/aspose.zip.sevenzip.sevenziparchive/createentries/methods/1
[20]: https://apireference.aspose.com/zip/net/aspose.zip.sevenzip.sevenziparchive/save/methods/1
[21]: https://apireference.aspose.com/zip/net/aspose.zip.saving/sevenzipaesencryptionsettings
[22]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream
[23]: https://docs.microsoft.com/en-us/dotnet/api/system.io.fileinfo
[24]: https://apireference.aspose.com/zip/net/aspose.zip.sevenzip/sevenziparchive
[25]: https://apireference.aspose.com/zip/net/aspose.zip.sevenzip/sevenziparchive/methods/createentry
[26]: https://apireference.aspose.com/zip/net/aspose.zip.sevenzip/sevenziparchive/methods/save
[27]: https://docs.aspose.com/display/zipnet/Product+Overview
[28]: https://blog.aspose.com/2020/04/22/create-zip-archives-add-files-or-folders-to-zip-in-csharp-asp.net/
[29]: https://blog.aspose.com/2020/04/23/unzip-files-in-password-protected-zip-archives-in-csharp-asp.net/





