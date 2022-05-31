---
title: 'Read Outlook MSG Files in C#'
date: Tue, 18 Jan 2022 12:27:08 +0000
draft: false
url: /2022/01/18/read-outlook-msg-emails-in-csharp/
author: 'Usman Aziz'
summary: '[MSG](https://docs.fileformat.com/email/msg/) is a popular file format used by MS Outlook to store email messages, contacts, appointments, etc. While working with email automation from within your .NET applications, you may need to read MSG files. To accomplish that, this article covers **how to parse and read Outlook MSG files in C#**. Moreover, we will demonstrate how to fetch attachments from an MSG file programmatically.'
tags: ['Dotnet API to Parse and Read MSG Files', 'Dotnet Email Library', 'Get Email Attachments in MSG File in Csharp', 'Read an Outlook MSG Email in Csharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Read-Outlook-MSG-Files.png" alt="Read Outlook MSG File in C#">}}


[MSG](https://docs.fileformat.com/email/msg/) is a popular file format used by MS Outlook to store email messages, contacts, appointments, etc. While working with email automation from within your .NET applications, you may need to read MSG files. To accomplish that, this article covers **how to parse and read Outlook MSG files in C#**. Moreover, we will demonstrate how to fetch attachments from an MSG file programmatically.

*   [.NET API to Parse and Read MSG Files](#API-to-Parse-and-Read-MSG-Files)
*   [Parse and Read an Outlook MSG File](#Read-an-Outlook-MSG-Email)
*   [Get Attachments from MSG File](#Get-Email-Attachments-in-MSG-File)

## C# .NET API to Parse and Read MSG Files {#API-to-Parse-and-Read-MSG-Files}

[Aspose.Email for .NET](https://products.aspose.com/email/net/) is a powerful .NET API that provides a wide range of features to implement email client applications. It supports creating, sending, reading, and manipulating email messages seamlessly. We will use this API to parse and read MSG files and extract their attachments. You can either install the API from [NuGet](https://www.nuget.org/packages/Aspose.Email) or [download](https://downloads.aspose.com/email/net/) its DLL.

```
PM> Install-Package Aspose.Email
```

## Parse and Read an Outlook MSG File in C# {#Read-an-Outlook-MSG-Email}

Aspose.Email for .NET allows reading all the essential data from an MSG file such as sender, recepients, email body, etc. Let's see how to read this data from an MSG file in C#.

*   Load MSG file using [MailMessage.Load(String)](https://apireference.aspose.com/email/net/aspose.email.mailmessage/load/methods/2) method.
*   Read the data using following properties:
    *   [MailMessage.Subject](https://apireference.aspose.com/email/net/aspose.email/mailmessage/properties/subject)
    *   [MailMessage.To](https://apireference.aspose.com/email/net/aspose.email/mailmessage/properties/to)
    *   [MailMessage.From](https://apireference.aspose.com/email/net/aspose.email/mailmessage/properties/from)
    *   [MailMessage.Body](https://apireference.aspose.com/email/net/aspose.email/mailmessage/properties/body)
    *   [etc](https://apireference.aspose.com/email/net/aspose.email/mailmessage/properties/index).

The following code sample shows how to read an Outlook MSG file in C#.

\[gist id="15d4d3b09aa68953fc2c7106aa764aab" file="read-msg-file.cs"\]

## Get Attachments from MSG File in C# {#Get-Email-Attachments-in-MSG-File}

Aspose.Email for .NET also allows you to fetch attachments from an MSG file. The following steps show how to fetch and save the attachments of an MSG file in C#.

*   Load MSG file using [MailMessage.Load(String)](https://apireference.aspose.com/email/net/aspose.email.mailmessage/load/methods/2) method.
*   Loop through each [Attachment](https://apireference.aspose.com/email/net/aspose.email/attachment) in the collection using [MailMessage.Attachments](https://apireference.aspose.com/email/net/aspose.email/mailmessage/properties/attachments) property.
*   Save each attachment to disk using [Attachment.Save()](https://apireference.aspose.com/email/net/aspose.email.attachmentbase/save/methods/1) method.

The following code sample shows how to get and save attachments of an MSG file in C#.

\[gist id="15d4d3b09aa68953fc2c7106aa764aab" file="read-msg-attachments.cs"\]

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Email for .NET without evaluation limitations by [getting a temporary license](https://purchase.aspose.com/temporary-license).

## Conclusion

In this article, you have learned how to read Outlook MSG files programmatically in C#. Moreover, you have seen how to fetch attachments in an MSG file and save them on disk. To explore more about Aspose.Email for .NET, you can visit [documentation](https://docs.aspose.com/email/net/). Also, in case of any questions or queries, feel free to let us know via our [forum](https://forum.aspose.com/).

## See Also

*   [Create and Send Outlook Emails using C#](https://blog.aspose.com/2020/01/23/create-send-outlook-email-eml-msg-csharp-net-core/)



