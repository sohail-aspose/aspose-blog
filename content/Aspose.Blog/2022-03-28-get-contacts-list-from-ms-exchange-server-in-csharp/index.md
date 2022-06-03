---
title: 'Get Contacts List from Microsoft Exchange Server in C#'
date: Mon, 28 Mar 2022 14:30:13 +0000
draft: false
url: /2022/03/28/get-contacts-list-from-ms-exchange-server-in-csharp/
author: ''Usman Aziz''
summary: '[Microsoft Exchange Server][1] is a well-known platform for email, calendaring and other collaboration services. Often you may need to connect to your MS Exchange Server and retrieve the list of contacts programmatically. To achieve that, this article shows **how to get the contacts list from Microsoft Exchange Server in C# .NET**.'
tags: ['Csharp DotNET API to Retrieve Contacts from MS Exchange Server', 'Get Contacts List from MS Exchange Server in Csharp', 'Get a Contact using ID from Exchange Server Csharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Get Contacts List from Microsoft Exchange Server in C#">}}


[Microsoft Exchange Server][2] is a well-known platform for email, calendaring and other collaboration services. Often you may need to connect to your MS Exchange Server and retrieve the list of contacts programmatically. To achieve that, this article shows **how to get the contacts list from Microsoft Exchange Server in C# .NET**.

*   [C# .NET API to Retrieve Contacts from MS Exchange Server][3]
*   [Get Contacts List from MS Exchange Server][4]
*   [Get a Contact using ID][5]

## C# .NET API to Get Contacts List from MS Exchange Server {#API-to-Access-Contacts-on-Exchange-Server}

To retrieve the contacts from Microsoft Exchange Server, we will use [Aspose.Email for .NET][6]. It is a powerful API that provides a range of features to implement email client applications. Also, it allows you to connect to and work with MS Exchange Server seamlessly. You can either [download][7] the API's DLL or install it from [NuGet][8] using the following command.

```
PM> Install-Package Aspose.Email
```

## Retrieve Contacts List from MS Exchange Server in C# {#Get-Contacts-List-from-MS-Exchange-Server}

The following are the steps to get the contacts list from Microsoft Exchange Server in C#.

*   First, initialize [IEWSClient][9] object using username, password, domain, and mailbox URI.
*   Then, call [IEWSClient.GetContacts(EWSClient.MailboxInfo.ContactsUri)][10] method to get contacts in an array.
*   Loop through each contact in array and fetch its details.

The following code sample shows how to get the contacts list from Microsoft Exchange Server in C#.

{{< gist aspose-com-gists 0879a1e9f06933f3d1105ef0dde6e026 "get-contacts-list.cs" >}}

## Get a Contact from MS Exchange Server by ID {#Get-a-Contact-using-ID}

Aspose.Email for .NET also allows you to retrieve a contact using its ID. For this, you must know the contact ID in advance. The following are the steps to retrieve a contact from MS Exchange Server in C#.

*   First, initialize [IEWSClient][11] object using username, password, domain, and mailbox URI.
*   Then, call [IEWSClient.GetContact()][12] method and get contact in a [Contact][13] object.
*   Use or manipulate the contact as required.

The following code sample shows how to retrieve a particular contact from Microsoft Exchange Server in C#.

{{< gist aspose-com-gists 0879a1e9f06933f3d1105ef0dde6e026 "get-contact.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

Get a [free temporary license][14] and use Aspose.Email for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to get the contacts list from Microsoft Exchange Server in C#. Furthermore, you have seen how to retrieve a contact by its ID programmatically. Apart from that, you can explore the other features of Aspose.Email for .NET using the [documentation][15]. Also, you can ask your questions via our [forum][16].

## See Also

*   [Create and Send Outlook Emails using C#][17]




[1]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[2]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[3]: #API-to-Access-Contacts-on-Exchange-Server
[4]: #Get-Contacts-List-from-MS-Exchange-Server
[5]: #Get-a-Contact-using-ID
[6]: https://products.aspose.com/email/net
[7]: https://downloads.aspose.com/email/net
[8]: https://www.nuget.org/packages/Aspose.Email/
[9]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[10]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/getcontacts
[11]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[12]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice.iewsclient/getcontact/methods/2
[13]: https://apireference.aspose.com/email/net/aspose.email.personalinfo/contact
[14]: https://purchase.aspose.com/temporary-license
[15]: https://docs.aspose.com/email/net/
[16]: https://forum.aspose.com/
[17]: https://blog.aspose.com/2020/01/23/create-send-outlook-email-eml-msg-csharp-net-core/




