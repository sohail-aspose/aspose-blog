---
title: 'Create Executable Self-extracting Archive in C#'
date: Mon, 10 Jan 2022 09:07:24 +0000
draft: false
url: /2022/01/10/create-self-extracting-archive-in-csharp/
author: 'Usman Aziz'
summary: "A [self-extracting archive][1] (SFX or SEA) is a special type of file that contains compressed data along with executable instructions. This archive has the ability to extract the files it contains by itself. Therefore, you don't need any specific extractor or decompressor application to open self-extracting archives. In this article, you will learn **how to create executable self-extracting archives in C# from within your .NET applications**."
tags: ['Create SFX in Csharp', 'Create a Self-extracting Archive in CSharp Dotnet', 'Dotnet API to Create Self-extracting Archives', 'Executing Self-extracting Archives from Command Line']
categories: ['Aspose.ZIP Product Family']
---



{{< figure align=center src="images/Create-self-extracting-archive.jpg" alt="Create Executable Self-extracting Archive in C#">}}


A [self-extracting archive][2] (SFX or SEA) is a special type of file that contains compressed data along with executable instructions. This archive has the ability to extract the files it contains by itself. Therefore, you don't need any specific extractor or decompressor application to open self-extracting archives. In this article, you will learn **how to create executable self-extracting archives in C# from within your .NET applications**.

*   [.NET API to Create Self-extracting Archives][3]
*   [Create a Self-extracting Archive in C#][4]
*   [Executing Self-extracting Archives from Command Line][5]

## C# .NET API to Create Self-extracting Archives {#API-to-Create-Self-extracting-Archives}

To create self-extracting archives, we will use [Aspose.ZIP for .NET][6]. It is a powerful and feature-rich API that lets you automate the archiving features in .NET applications quite easily. Moreover, it supports a variety of popular archive formats such as ZIP, TAR, etc. You can [download][7] the API's DLL or install it using [NuGet][8].

```
PM> Install-Package Aspose.Zip 
```

## Create a Self-extracting Archive in C# {#Create-a-Self-extracting-Archive}

Let's start creating a self-extracting archive assuming that you have installed Aspose.ZIP for .NET. Since this will be an executable archive, its extension will be **[.exe][9]**. The following are the steps to create an executable self-extracting archive in C#.

*   First, create a new [FileStream][10] object for archive.
*   Then, create an object of [Archive][11] class.
*   Add files to the archive using [Archive.CreateEntry(string, string)][12] method.
*   Create an object of [SelfExtractorOptions][13] class to sepcify options for self-extracting archive.
*   Set options such as title, icon, etc.
*   Finally, save the self-extracting archive file using [Archive.Save(FileStream, new ArchiveSaveOptions())][14] method.

The following code sample shows how to create an executable self-extracting archive in .NET.

{{< gist aspose-com-gists affc766964fa27f6b59c8008481e2ae8 "create-sfx-archive.cs" >}}

## Executing Self-extracting Archives using Command Line {#Executing-Self-extracting-Archives-from-Command-Line}

The self-extracting archive that we have created in the previous section can be extracted by double-clicking it. However, if you want to use the command line, you can extract the archive with the following command.

```
C:\>archive.exe -autoExtract 
```

Here, **\-autoExtract** is the primary option that lets you extract the archive. In case the archive is password-protected, you can specify the password using **\-password** option, as shown in the following command.

```
C:\>archive.exe -autoExtract -password:T0p$ecret
```

The complete list of the commands to work with an executable self-extracting archive is provided in [this article][15].

## Get a Free API License

You can use Aspose.ZIP for .NET without evaluation limitations by getting [a free temporary license][16].

## Conclusion

In this article, you have learned how to create self-extracting archives (SFX or SEA) in C#. Furthermore, we have discussed how to extract a self-extracting archive using the command line. You can simply install Aspose.ZIP for .NET and embed the provided code sample in your .NET applications. Besides, you can explore more about Aspose.ZIP for .NET using its [documentation][17]. Also, you can post your queries to our [forum][18].

## See Also

*   [Add Files or Folders to ZIP Archives in C#][19]
*   [Unzip Files in ZIP Archives using C#][20]
*   [Merge Multiple ZIP or TAR Archives in C#][21]




[1]: https://en.wikipedia.org/wiki/Self-extracting_archive
[2]: https://en.wikipedia.org/wiki/Self-extracting_archive
[3]: #API-to-Create-Self-extracting-Archives
[4]: #Create-a-Self-extracting-Archive
[5]: #Executing-Self-extracting-Archives-from-Command-Line
[6]: https://products.aspose.com/zip/net/
[7]: https://downloads.aspose.com/zip/net/
[8]: https://www.nuget.org/packages/Aspose.ZIP
[9]: https://docs.fileformat.com/executable/exe/
[10]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream
[11]: https://apireference.aspose.com/zip/net/aspose.zip/archive
[12]: https://apireference.aspose.com/zip/net/aspose.zip.archive/createentry/methods/3
[13]: https://apireference.aspose.com/zip/net/aspose.zip.saving/selfextractoroptions
[14]: https://apireference.aspose.com/zip/net/aspose.zip/archive/methods/save
[15]: https://docs.aspose.com/zip/net/create-self-extracting-sfx-archive/#command-line-options-for-self-extracting-archive
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/zip/net/
[18]: https://forum.aspose.com/
[19]: https://blog.aspose.com/2020/04/22/create-zip-archives-add-files-or-folders-to-zip-in-csharp-asp.net/
[20]: https://blog.aspose.com/2020/04/23/unzip-files-in-password-protected-zip-archives-in-csharp-asp.net/
[21]: https://blog.aspose.com/2022/01/06/merge-zip-and-tar-files-in-csharp/




