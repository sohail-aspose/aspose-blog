---
title: 'Read Emails from Shared Mailbox on Exchange Server in C#'
date: Sat, 05 Mar 2022 05:24:00 +0000
draft: false
url: /2022/03/05/read-emails-from-shared-mailbox-on-exchange-server-in-csharp/
author: 'Usman Aziz'
summary: ''
tags: ['Access Shared Mailbox with EWS in CSharp', 'DotNet API to Read Emails from Shared Mailbox', 'Read Emails from a Shared Mailbox with EWS in Csharp']
categories: ['Aspose.Total Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Read Emails from Shared Mailbox on Exchange Server in C#">}}


[Microsoft Exchange Server](https://en.wikipedia.org/wiki/Microsoft_Exchange_Server) provides a bunch of useful features to create, send, and manage emails. One of these features is a shared mailbox that can be accessed by multiple users. While working with MS Exchange Server from within your .NET applications, you may need to access emails from a shared mailbox. So in this article, you will learn **how to read email messages from a shared mailbox on MS Exchange Server using C# .NET**.

*   [.NET API to Read Emails from Shared Mailbox](#API-to-Create-Folders-in-MS-Exchange-Server)
*   [Read Emails from a Shared Mailbox](#Read-Emails-from-a-Shared-Mailbox)

## C# .NET API to Read Emails from Shared Mailbox on Exchange Server {#API-to-Create-Folders-in-MS-Exchange-Server}

[Aspose.Email for .NET](https://products.aspose.com/email/net/) is an email processing API that provides a range of features to create, send, and process emails. In addition, it allows you to work with MS Outlook and Exchange Server without writing complex code. We will use this API to read emails from the shared mailboxes on MS Exchange Server. You can either [download](https://downloads.aspose.com/email/net) the API’s DLL or install it from [NuGet](https://www.nuget.org/packages/Aspose.Email/) using the following command.

```
PM> Install-Package Aspose.Email
```

## Read Emails from a Shared Mailbox on Exchange Server in C# {#Read-Emails-from-a-Shared-Mailbox}

The following are the steps to read emails from a shared mailbox on MS Exchange Server with an EWS client in C#.

*   Specify the network credentials.
*   Connect to Exchange Server and get the instance of the EWS client into an [IEWSClient](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient) object.
*   Get emails into an array from the desired folder using [IEWSClient.ListItems(String, String)](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice.iewsclient/listitems/methods/3) method.
*   Loop through each email in the array and perform the following steps:
    *   Fetch each message into a [MapiMessage](https://apireference.aspose.com/email/net/aspose.email.mapi/mapimessage) object using [IEWSClient.FetchItem(String)](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/fetchitem) method.
    *   Read message's details using _MapiMessage_ object such as [MapiMessage.Subject](https://apireference.aspose.com/email/net/aspose.email.mapi/mapimessageitembase/properties/subject) property.

The following code sample shows how to read email messages from a shared mailbox on MS Exchange Server in C#.

{{< gist aspose-com-gists d761d651a93cbc11e1faec93f2e29be8 "read-emails-from-shared-mailbox.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license](https://purchase.aspose.com/temporary-license) to use Aspose.Email for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to read email messages from a shared mailbox on Microsoft Exchange Server in C#. To integrate this feature into your .NET applications, you can simply install the API and use the provided code sample. In addition, you can read about other features of Aspose.Email for .NET from the [documentation](https://docs.aspose.com/email/net/). Also, you can ask your questions via our [forum](https://forum.aspose.com/).

## See Also

*   [Read Emails from MS Exchange Server using C#](https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/)




