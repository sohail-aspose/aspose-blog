---
title: 'Read Outlook MSG Files in C#'
seoTitle: "Read Outlook MSG Files in C# .NET | Fetch MSG Attachments in C#"
description: "Use .NET Email API to read MS Outlook MSG files in C# from within your .NET applications. Fetch and download attachments in an MSG file programmatically."
date: Tue, 18 Jan 2022 12:27:08 +0000
draft: false
url: /2022/01/18/read-outlook-msg-emails-in-csharp/
author: Usman Aziz
summary: '[MSG][1] is a popular file format used by MS Outlook to store email messages, contacts, appointments, etc. While working with email automation from within your .NET applications, you may need to read MSG files. To accomplish that, this article covers **how to parse and read Outlook MSG files in C#**. Moreover, we will demonstrate how to fetch attachments from an MSG file programmatically.'
tags: ['Dotnet API to Parse and Read MSG Files', 'Dotnet Email Library', 'Get Email Attachments in MSG File in Csharp', 'Read an Outlook MSG Email in Csharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Read-Outlook-MSG-Files.png" alt="Read Outlook MSG File in C#">}}


[MSG][2] is a popular file format used by MS Outlook to store email messages, contacts, appointments, etc. While working with email automation from within your .NET applications, you may need to read MSG files. To accomplish that, this article covers **how to parse and read Outlook MSG files in C#**. Moreover, we will demonstrate how to fetch attachments from an MSG file programmatically.

*   [.NET API to Parse and Read MSG Files][3]
*   [Parse and Read an Outlook MSG File][4]
*   [Get Attachments from MSG File][5]

## C# .NET API to Parse and Read MSG Files {#API-to-Parse-and-Read-MSG-Files}

[Aspose.Email for .NET][6] is a powerful .NET API that provides a wide range of features to implement email client applications. It supports creating, sending, reading, and manipulating email messages seamlessly. We will use this API to parse and read MSG files and extract their attachments. You can either install the API from [NuGet][7] or [download][8] its DLL.

```
PM> Install-Package Aspose.Email
```

## Parse and Read an Outlook MSG File in C# {#Read-an-Outlook-MSG-Email}

Aspose.Email for .NET allows reading all the essential data from an MSG file such as sender, recepients, email body, etc. Let's see how to read this data from an MSG file in C#.

*   Load MSG file using [MailMessage.Load(String)][9] method.
*   Read the data using following properties:
    *   [MailMessage.Subject][10]
    *   [MailMessage.To][11]
    *   [MailMessage.From][12]
    *   [MailMessage.Body][13]
    *   [etc][14].

The following code sample shows how to read an Outlook MSG file in C#.

{{< gist aspose-com-gists 15d4d3b09aa68953fc2c7106aa764aab "read-msg-file.cs" >}}

## Get Attachments from MSG File in C# {#Get-Email-Attachments-in-MSG-File}

Aspose.Email for .NET also allows you to fetch attachments from an MSG file. The following steps show how to fetch and save the attachments of an MSG file in C#.

*   Load MSG file using [MailMessage.Load(String)][15] method.
*   Loop through each [Attachment][16] in the collection using [MailMessage.Attachments][17] property.
*   Save each attachment to disk using [Attachment.Save()][18] method.

The following code sample shows how to get and save attachments of an MSG file in C#.

{{< gist aspose-com-gists 15d4d3b09aa68953fc2c7106aa764aab "read-msg-attachments.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Email for .NET without evaluation limitations by [getting a temporary license][19].

## Conclusion

In this article, you have learned how to read Outlook MSG files programmatically in C#. Moreover, you have seen how to fetch attachments in an MSG file and save them on disk. To explore more about Aspose.Email for .NET, you can visit [documentation][20]. Also, in case of any questions or queries, feel free to let us know via our [forum][21].

## See Also

*   [Create and Send Outlook Emails using C#][22]




[1]: https://docs.fileformat.com/email/msg/
[2]: https://docs.fileformat.com/email/msg/
[3]: #API-to-Parse-and-Read-MSG-Files
[4]: #Read-an-Outlook-MSG-Email
[5]: #Get-Email-Attachments-in-MSG-File
[6]: https://products.aspose.com/email/net/
[7]: https://www.nuget.org/packages/Aspose.Email
[8]: https://downloads.aspose.com/email/net/
[9]: https://apireference.aspose.com/email/net/aspose.email.mailmessage/load/methods/2
[10]: https://apireference.aspose.com/email/net/aspose.email/mailmessage/properties/subject
[11]: https://apireference.aspose.com/email/net/aspose.email/mailmessage/properties/to
[12]: https://apireference.aspose.com/email/net/aspose.email/mailmessage/properties/from
[13]: https://apireference.aspose.com/email/net/aspose.email/mailmessage/properties/body
[14]: https://apireference.aspose.com/email/net/aspose.email/mailmessage/properties/index
[15]: https://apireference.aspose.com/email/net/aspose.email.mailmessage/load/methods/2
[16]: https://apireference.aspose.com/email/net/aspose.email/attachment
[17]: https://apireference.aspose.com/email/net/aspose.email/mailmessage/properties/attachments
[18]: https://apireference.aspose.com/email/net/aspose.email.attachmentbase/save/methods/1
[19]: https://purchase.aspose.com/temporary-license
[20]: https://docs.aspose.com/email/net/
[21]: https://forum.aspose.com/
[22]: https://blog.aspose.com/2020/01/23/create-send-outlook-email-eml-msg-csharp-net-core/




