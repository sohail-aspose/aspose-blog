---
title: 'Read Emails from Shared Mailbox on Exchange Server in C#'
seoTitle: "C# Read Emails from Shared Mailbox in MS Exchange Server | EWS API"
description: "Use .NET EWS API to read emails from a shared mailbox on Microsoft Exchange Server programmatically using C#. Retrieve messages with the EWS client."
date: Sat, 05 Mar 2022 05:24:00 +0000
draft: false
url: /2022/03/05/read-emails-from-shared-mailbox-on-exchange-server-in-csharp/
author: Usman Aziz
summary: ''
tags: ['Access Shared Mailbox with EWS in CSharp', 'DotNet API to Read Emails from Shared Mailbox', 'Read Emails from a Shared Mailbox with EWS in Csharp']
categories: ['Aspose.Total Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Read Emails from Shared Mailbox on Exchange Server in C#">}}


[Microsoft Exchange Server][1] provides a bunch of useful features to create, send, and manage emails. One of these features is a shared mailbox that can be accessed by multiple users. While working with MS Exchange Server from within your .NET applications, you may need to access emails from a shared mailbox. So in this article, you will learn **how to read email messages from a shared mailbox on MS Exchange Server using C# .NET**.

*   [.NET API to Read Emails from Shared Mailbox][2]
*   [Read Emails from a Shared Mailbox][3]

## C# .NET API to Read Emails from Shared Mailbox on Exchange Server {#API-to-Create-Folders-in-MS-Exchange-Server}

[Aspose.Email for .NET][4] is an email processing API that provides a range of features to create, send, and process emails. In addition, it allows you to work with MS Outlook and Exchange Server without writing complex code. We will use this API to read emails from the shared mailboxes on MS Exchange Server. You can either [download][5] the API’s DLL or install it from [NuGet][6] using the following command.

```
PM> Install-Package Aspose.Email
```

## Read Emails from a Shared Mailbox on Exchange Server in C# {#Read-Emails-from-a-Shared-Mailbox}

The following are the steps to read emails from a shared mailbox on MS Exchange Server with an EWS client in C#.

*   Specify the network credentials.
*   Connect to Exchange Server and get the instance of the EWS client into an [IEWSClient][7] object.
*   Get emails into an array from the desired folder using [IEWSClient.ListItems(String, String)][8] method.
*   Loop through each email in the array and perform the following steps:
    *   Fetch each message into a [MapiMessage][9] object using [IEWSClient.FetchItem(String)][10] method.
    *   Read message's details using _MapiMessage_ object such as [MapiMessage.Subject][11] property.

The following code sample shows how to read email messages from a shared mailbox on MS Exchange Server in C#.

{{< gist aspose-com-gists d761d651a93cbc11e1faec93f2e29be8 "read-emails-from-shared-mailbox.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][12] to use Aspose.Email for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to read email messages from a shared mailbox on Microsoft Exchange Server in C#. To integrate this feature into your .NET applications, you can simply install the API and use the provided code sample. In addition, you can read about other features of Aspose.Email for .NET from the [documentation][13]. Also, you can ask your questions via our [forum][14].

## See Also

*   [Read Emails from MS Exchange Server using C#][15]




[1]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[2]: #API-to-Create-Folders-in-MS-Exchange-Server
[3]: #Read-Emails-from-a-Shared-Mailbox
[4]: https://products.aspose.com/email/net/
[5]: https://downloads.aspose.com/email/net
[6]: https://www.nuget.org/packages/Aspose.Email/
[7]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[8]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice.iewsclient/listitems/methods/3
[9]: https://apireference.aspose.com/email/net/aspose.email.mapi/mapimessage
[10]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/fetchitem
[11]: https://apireference.aspose.com/email/net/aspose.email.mapi/mapimessageitembase/properties/subject
[12]: https://purchase.aspose.com/temporary-license
[13]: https://docs.aspose.com/email/net/
[14]: https://forum.aspose.com/
[15]: https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/




