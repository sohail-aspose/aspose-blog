---
title: 'Move Email to a Folder on Microsoft Exchange Server in C#'
seoTitle: "C# Move Email to a Folder in MS Exchange Server | .NET API"
description: "Use .NET API to move emails to a particular folder in MS Exchange Server in C#. Move newly created email messages to a specific folder in Exchange Server."
date: Mon, 28 Feb 2022 04:45:00 +0000
draft: false
url: /2022/02/28/move-emails-to-folders-in-ms-exchange-server-csharp/
author: Usman Aziz
summary: '[Microsoft Exchange Server][1] is a widely used collaboration platform that provides email, contact management, calendaring, and other services. In the [previous post][2], we have shown you how to access and read emails from MS Exchange Server programmatically in a .NET application. However, you may also need to copy emails from one folder to another on Exchange Server. To achieve that, this article shows **how to move emails to a particular folder on MS Exchange Server in C# .NET**.'
tags: ['Microsoft Exchange Server API for CSharp', 'Microsoft Exchange Server API for DotNet', 'Move Existing Email to a Folder in MS Exchange Server Csharp', 'Move New Email to a Folder in MS Exchange Server Csharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Move Email to a Folder in Microsoft Exchange Server using C#">}}


[Microsoft Exchange Server][3] is a widely used collaboration platform that provides email, contact management, calendaring, and other services. In the [previous post][4], we have shown you how to access and read emails from MS Exchange Server programmatically in a .NET application. However, you may also need to copy emails from one folder to another on Exchange Server. To achieve that, this article shows **how to move emails to a particular folder on MS Exchange Server in C# .NET**.

*   [.NET API to Move Emails on Microsoft Exchange Server][5]
*   [Move Existing Email to a Folder on MS Exchange Server][6]
*   [Move New Email to a Folder on MS Exchange Server][7]

## C# .NET API to Move Emails on Microsoft Exchange Server {#API-to-Move-Emails-in-Microsoft-Exchange-Server}

To move the emails on MS Exchange Server, we will use [Aspose.Email for .NET][8]. The API provides simple ways to connect to and work with MS Exchange Server. You can install it via [NuGet][9] or [download][10] its DLL.

```
PM> Install-Package Aspose.Email
```

## Move Email to a Folder on MS Exchange Server in C# {#Move-Existing-Email-to-a-Folder-in-MS-Exchange-Server}

The following are the steps to move emails to a particular folder on MS Exchange Server in C#.

*   First, initialize [IEWSClient][11] object using username, password, domain and URI.
*   Then, get list of email messages in an [ExchangeMessageInfoCollection][12] object using [IEWSClient.ListMessages(IEWSClient.MailboxInfo.InboxUri)][13] method.
*   After that, loop through each [ExchangeMessageInfo][14] message and filter the required one(s).
*   Then, get the URI of message to be moved using [ExchangeMessageInfo.UniqueUri][15] property.
*   Finally, move email message using [IEWSClient.CopyItem(string URI, IEWSClient.MailboxInfo.DeletedItemsUri)][16] method.

The following code sample shows how to move an email to a folder on MS Exchange Server in C# .NET.

{{< gist aspose-com-gists 90b12211b37081e5a2630efb8906d8ff "move-email.cs" >}}

## Move New Email to a Folder on MS Exchange Server {#Move-New-Email-to-a-Folder-in-MS-Exchange-Server}

You can also move a newly created email to a particular folder in MS Exchange Server. The following are the steps to perform this operation.

*   First, initialize [IEWSClient][17] object using username, password, domain and URI.
*   Then, create a new message using [MailMessage][18] class.
*   After that, get email message's URI returned by [IEWSClient.AppendMessage(MailMessage)][19] method.
*   Finally, move email message using [IEWSClient.CopyItem(string URI, IEWSClient.MailboxInfo.OutboxUri)][20] method.

The following code sample shows how to move a new email message to a folder in MS Exchange Server.

{{< gist aspose-com-gists 90b12211b37081e5a2630efb8906d8ff "move-new-email.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][21] to use Aspose.Email for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to move emails to a particular folder in Microsoft Exchange Server using C#. Furthermore, you have seen how to move a newly created email message to a specific folder in Exchange Server. Besides, you can explore the [documentation][22] to read more about Aspose.Email for .NET. Also, you can ask your questions via our [forum][23].

## See Also

*   [Create and Send Outlook Emails using C#][24]




[1]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[2]: https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/
[3]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[4]: https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/
[5]: #API-to-Move-Emails-in-Microsoft-Exchange-Server
[6]: #Move-Existing-Email-to-a-Folder-in-MS-Exchange-Server
[7]: #Move-New-Email-to-a-Folder-in-MS-Exchange-Server
[8]: https://products.aspose.com/email/net
[9]: https://www.nuget.org/packages/Aspose.email
[10]: https://downloads.aspose.com/email/net
[11]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[12]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange/exchangemessageinfocollection
[13]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice.iewsclient/listmessages/methods/2
[14]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange/exchangemessageinfo
[15]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange/exchangemessageinfo/properties/uniqueuri
[16]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/copyitem
[17]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[18]: https://apireference.aspose.com/email/net/aspose.email/mailmessage
[19]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/appendmessage
[20]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/copyitem
[21]: https://purchase.aspose.com/temporary-license
[22]: https://docs.aspose.com/email/net/
[23]: https://forum.aspose.com/
[24]: https://blog.aspose.com/2020/01/23/create-send-outlook-email-eml-msg-csharp-net-core/




