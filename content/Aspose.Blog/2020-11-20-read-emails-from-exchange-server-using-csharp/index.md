---
title: 'Read Emails from MS Exchange Server using C#'
seoTitle: "C# Read Emails from MS Exchange Server | .NET Email API"
description: "Use .NET Exchange Server API to read email messages from MS Exchange Server using C#. Connect to your Exchange Server using EWS or IMAP."
date: Fri, 20 Nov 2020 17:15:45 +0000
draft: false
url: /2020/11/20/read-emails-from-exchange-server-using-csharp/
author: Usman Aziz
summary: '[Microsoft Exchange Server][1] is a platform that lets you manage contacts, emails, calendars, schedules and provides several collaboration features. With MS Exchange Server, you can deploy your own mail server without relying on third parties. MS Exchange Server can also be accessed from within your web, desktop, or mobile applications via web services. Thus, you can perform the mailing and calendering operations in your applications. In this article, you are going to learn **how to connect to an Exchange Server and read emails using C#**.'
tags: ['connect to ms exchange server', 'read email from exchange server csharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Read Emails from MS Exchange Server using C#">}}


[Microsoft Exchange Server][2] is a platform that lets you manage contacts, emails, calendars, schedules and provides several collaboration features. With MS Exchange Server, you can deploy your own mail server without relying on third parties. MS Exchange Server can also be accessed from within your web, desktop, or mobile applications via web services. Thus, you can perform the mailing and calendering operations in your applications. In this article, you are going to learn **how to connect to an Exchange Server and read emails using [C#][3]**.

*   [C# Exchange Server API][4]
*   [Connect to MS Exchange Server][5]
*   [Read Emails from Exchange Server using EWS][6]
*   [Read Emails from Exchange Server using IMAP][7]

## C# Exchange Server API - Free Download {#CSharp-Exchange-Server-API}

[Aspose.Email for .NET][8] provides easy to use API in order to work with MS Exchange Server. It lets you connect to your mail server using Exchange Web Service (EWS) or Internet Message Access Protocol (IMAP). Once you are connected, you can access items in a mailbox within a few steps. You can install Aspose.Email for .NET via [NuGet][9] or [download][10] its DLL.

```
PM> Install-Package Aspose.Email
```

## Connect to an Exchange Server using C# {#Connect-to-an-Exchange-Server-using-CSharp}

Aspose.Email for .NET provides two ways to connect to an instance of Exchange Server: EWS and IMAP. The following sections provide the steps of how to establish a connection using either of the ways.

### Connect to an Exchange Server via EWS

The following are steps to connect to an MS Exchange Server using Aspose.Email for .NET.

*   Use [NetworkCredential][11] class to set credentials including username, password, and domain.
*   Get [IEWSClient][12] object returned by [EWSClient.GetEWSClient(String, ICredentials)][13] method.
*   Use _IEWSClient_ object to perform further operations.

The following code sample shows how to connect to Exchange Server via EWS using C#.

{{< gist aspose-com-gists 6e5185a63aec6fd70d83098e82b06a32 "Examples-CSharp-Exchange_EWS-ConnectingToExchangeServerUsingEWS-ConnectingToExchangeServerUsingEWS.cs" >}}

### Connect to an Exchange Server via IMAP

In order to connect to an Exchange Server via IMAP, make sure that IMAP services are enabled on your server. Once done, follow the below steps to connect to the Exchange Server.

*   Create an instance of [ImapClient][14] class and provide host, username, and password to its constructor.
*   Set security options using [ImapClient.SecurityOptions][15] property.
*   Access the items in the mailbox using the _ImapClient_ object.

The following code sample shows how to access Exchange Server via IMAP using C#.

{{< gist aspose-com-gists 07dd20cac9bac531178efbea38ea9b32 "connect-exchange-server-imap.cs" >}}

## Read Emails from Exchange Server using EWS in C# {#Read-Emails-from-Exchange-Server-using-EWS}

The following are the steps to read email messages from Exchange Server using EWS.

*   Create an instance of the IEWSClient.
*   Use [IEWSClient.ListMessage(String)][16] method to access the email collection.
*   Loop through the email collection to get details of each email message.

The following code sample shows how to read emails from Exchange Server in C#.

{{< gist aspose-email 9e8fbeb51a8cbc4129dc71ca8cd55f0b "Examples-CSharp-Exchange_EWS-ListingMessagesUsingEWS-ListingMessagesUsingEWS.cs" >}}

## Read Emails from Exchange Server using IMAP {#Read-Emails-from-Exchange-Server-using-IMAP}

The following are the steps to read emails from Exchange Server using IMAP.

*   Create an instance of [ImapClient][17] class and provide host, username, and password to its constructor.
*   Set security options using [ImapClient.SecurityOptions][18] property.
*   Select a folder such as inbox, sent, etc using [ImapClient.SelectFolder()][19] method.
*   Use [ImapClient.ListMessages()][20] method to get the email collection.
*   Loop through the email collection to access each message.

The following code sample shows how to read emails from Exchange Server using IMAP.

{{< gist aspose-com-gists 6e5185a63aec6fd70d83098e82b06a32 "Examples-CSharp-Exchange_EWS-ConnectExchangeServerUsingIMAP-ConnectExchangeServerUsingIMAP.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try the API without evaluation limitations for free. [Get a free temporary license][21] now.

## Live Demo

*   [Email Viewer][22]

## Conclusion

In this article, you have learned how to connect to MS Exchange Server and read email messages using C#. Furthermore, the code samples have shown how to access Exchange Server using EWS and IMAP clients. You can explore more about the C# Email API using [documentation][23].

## See Also

*   [Create and Send Emails using C#][24]




[1]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[2]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[3]: https://docs.fileformat.com/programming/cs/
[4]: #CSharp-Exchange-Server-API
[5]: #Connect-to-an-Exchange-Server-using-CSharp
[6]: #Read-Emails-from-Exchange-Server-using-EWS
[7]: #Read-Emails-from-Exchange-Server-using-IMAP
[8]: https://products.aspose.com/email/net
[9]: https://www.nuget.org/packages/Aspose.email
[10]: https://downloads.aspose.com/email/net
[11]: https://docs.microsoft.com/en-gb/dotnet/api/system.net.networkcredential?view=net-5.0
[12]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[13]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice.ewsclient/getewsclient/methods/2
[14]: https://apireference.aspose.com/email/net/aspose.email.clients.imap/imapclient
[15]: https://apireference.aspose.com/email/net/aspose.email.clients/emailclient/properties/securityoptions
[16]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice.iewsclient/listmessages/methods/2
[17]: https://apireference.aspose.com/email/net/aspose.email.clients.imap/imapclient
[18]: https://apireference.aspose.com/email/net/aspose.email.clients/emailclient/properties/securityoptions
[19]: https://apireference.aspose.com/email/net/aspose.email.clients.imap.imapclient/selectfolder/methods/2
[20]: https://apireference.aspose.com/email/net/aspose.email.clients.imap/imapclient/methods/listmessages
[21]: https://purchase.aspose.com/temporary-license
[22]: http://products.aspose.app/email/viewer
[23]: https://docs.aspose.com/email/net/getting-started/
[24]: https://blog.aspose.com/2020/01/23/create-send-outlook-email-eml-msg-csharp-net-core/





