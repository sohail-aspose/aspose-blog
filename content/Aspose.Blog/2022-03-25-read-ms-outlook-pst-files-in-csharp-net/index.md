---
title: 'Read MS Outlook PST Files in C# .NET'
seoTitle: "Read MS Outlook PST Files in C# .NET | Read Emails and Contacts in C#"
description: "Use .NET email processing library to parse PST files in C#. Extract emails and contacts from PST files programmatically in C#."
date: Fri, 25 Mar 2022 17:35:00 +0000
draft: false
url: /2022/03/25/read-ms-outlook-pst-files-in-csharp-net/
author: Usman Aziz
summary: "[PST (Personal Storage Table)][1] is a storage file format that is used by different Microsoft programs such as MS Outlook, Exchange, and Windows Messaging. PST files are capable of storing messages, contacts, calendars, events, etc. In certain cases, you may need to parse a PST file and extract data from it programmatically. To achieve that, this article shows **how to read MS Outlook PST files using C# .NET**. Particularly, you will learn how to extract folders' information, read emails and fetch contacts from a PST file."
tags: ['DotNet API to Read PST Files', 'Extract Contacts from a PST File in CSharp', 'Read Emails from a PST File in Csharp', 'Read an Outlook PST File in CSharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Parse-Outlook-PST-Files.png" alt="Read MS Outlook PST Files in C# .NET">}}


[PST (Personal Storage Table)][2] is a storage file format that is used by different Microsoft programs such as MS Outlook, Exchange, and Windows Messaging. PST files are capable of storing messages, contacts, calendars, events, etc. In certain cases, you may need to parse a PST file and extract data from it programmatically. To achieve that, this article shows **how to read MS Outlook PST files using C# .NET**. Particularly, you will learn how to extract folders' information, read emails and fetch contacts from a PST file.

*   [.NET API to Read Outlook PST Files][3]
*   [Read a PST File in C#][4]
*   [Read Emails from a PST File][5]
*   [Extract Contacts from a PST File][6]

## .NET API to Read Outlook PST Files {#API-to-Parse-PST-Files}

[Aspose.Email for .NET][7] is a powerful email processing API that lets you create and send emails from within .NET applications. In addition, it supports working with popular email and storage file formats. We will use this API to read folders' information, messages, and contacts from PST files. You can either [download][8] the API or install it via [NuGet][9].

```
PM> Install-Package Aspose.Email -Version 22.3.0
```

## Read an Outlook PST File in C# .NET {#Parse-a-PST-File}

The following are the steps to read a PST file and extract its information in C#.

*   Load the PST file using [PersonalStorage.FromFile()][10] method.
*   Get the folders collection in PST using [PersonalStorage.RootFolder.GetSubFolders()][11] method.
*   Retrieve the information of the folders such as name, number of items, etc.

The following code sample shows how to parse a PST file and fetch folders' information.

{{< gist aspose-com-gists 92dc646b5526487c8490842727bc5a34 "read-pst.cs" >}}

## Read Emails from a PST File in C# {#Extract-Messages-from-a-PST-File}

Emails are the major entities that are stored in PST files by MS Outlook. So let's see how to read email messages from a PST file in C#.

*   Load the PST file using [PersonalStorage.FromFile()][12] method.
*   Access the root folder using [PersonalStorage.RootFolder][13] property.
*   Get message collection using [FolderInfo.GetContents()][14] method.
*   Loop through the messages in the collection and read each message's fields.

The following code sample shows how to extract messages from a PST file in C# .NET.

{{< gist aspose-com-gists 92dc646b5526487c8490842727bc5a34 "read-emails.cs" >}}

## Extract Contacts from a PST File in C# {#Extract-Contacts-in-a-PST-File}

In certain cases, you may need to extract the contacts' information stored in a PST file. The following steps demonstrate how to access the contacts in a PST file in C#.

*   Load the PST file using [PersonalStorage.FromFile()][15] method.
*   Get reference of the contacts folder using [PersonalStorage.RootFolder.GetSubFolder("Contacts")][16] method.
*   Get collection of contacts using [FolderInfo.GetContents()][17] method.
*   Loop through the contacts collection and read each contact or save it.

The following code sample shows how to extract contacts from a PST file in C#.

{{< gist aspose-com-gists 92dc646b5526487c8490842727bc5a34 "extract-contacts.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try Aspose.Email for .NET for free by [getting a temporary license][18].

## Conclusion

In this article, you have learned how to read PST files programmatically in C# .NET. Furthermore, you have seen how to read folder information, fetch emails, and extract contacts from a PST file in C#. Besides, you can explore more about Aspose.Email for .NET using [documentation][19]. Also, you can share your questions or queries on our [forum][20].

## See Also

*   [Read Emails from MS Exchange Server using C#][21]
*   [Create and Send Outlook Emails using C# .NET or .NET Core][22]
*   [Read Emails from MS Exchange Server in C#][23]




[1]: https://docs.fileformat.com/email/pst/
[2]: https://docs.fileformat.com/email/pst/
[3]: #API-to-Parse-PST-Files
[4]: #Parse-a-PST-File
[5]: #Extract-Messages-from-a-PST-File
[6]: #Extract-Contacts-in-a-PST-File
[7]: https://products.aspose.com/email/net/
[8]: https://downloads.aspose.com/email/net/
[9]: https://www.nuget.org/packages/Aspose.Email
[10]: https://apireference.aspose.com/email/net/aspose.email.storage.pst/personalstorage/methods/fromfile
[11]: https://apireference.aspose.com/email/net/aspose.email.storage.pst/folderinfo/methods/getsubfolders
[12]: https://apireference.aspose.com/email/net/aspose.email.storage.pst/personalstorage/methods/fromfile
[13]: https://apireference.aspose.com/email/net/aspose.email.storage.pst/personalstorage/properties/rootfolder
[14]: https://apireference.aspose.com/email/net/aspose.email.storage.pst/folderinfo/methods/getcontents
[15]: https://apireference.aspose.com/email/net/aspose.email.storage.pst/personalstorage/methods/fromfile
[16]: https://apireference.aspose.com/email/net/aspose.email.storage.pst/folderinfo/methods/getsubfolder
[17]: https://apireference.aspose.com/email/net/aspose.email.storage.pst/folderinfo/methods/getcontents
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/email/net/
[20]: https://forum.aspose.com/
[21]: https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/
[22]: https://blog.aspose.com/2020/01/23/create-send-outlook-email-eml-msg-csharp-net-core/
[23]: https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/




