---
title: 'Add and Remove Members in MS Exchange Distribution Lists in C#'
seoTitle: "C# Add and Remove Members in MS Exchange Distribution List | .NET API"
description: "Use .NET EWS API to work with members in MS Exchange distribution list in C#. Add or remove members from distribution lists programmatically."
date: Thu, 07 Apr 2022 04:25:00 +0000
draft: false
url: /2022/04/07/manage-members-in-exchange-distribution-list-in-csharp/
author: Usman Aziz
summary: 'While working with [MS Exchange Server][1] from within .NET applications, you may need to work with distribution lists. In the [previous post][2], you have seen how to create and fetch Exchange distribution lists. In this article, you will learn **how to add or remove members in MS Exchange distribution lists programmatically in C# .NET**.'
tags: ['Add Members to MS Exchange Distribution Lists in Csharp', 'DotNet API to Manage Members of Exchange Distribution Lists', 'DotNet EWS API', 'Remove Members from MS Exchange Distribution Lists in Csharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Add and Remove Members from MS Exchange Distribution Lists in C#">}}


While working with [MS Exchange Server][3] from within .NET applications, you may need to work with distribution lists. In the [previous post][4], you have seen how to create and fetch Exchange distribution lists. In this article, you will learn **how to add or remove members in MS Exchange distribution lists programmatically in C# .NET**.

*   [.NET API to Manage Members of Exchange Distribution Lists][5]
*   [Add Members to MS Exchange Distribution Lists][6]
*   [Remove Members from MS Exchange Distribution Lists][7]

## .NET API to Manage Members of Exchange Distribution Lists {#API-to-Manage-Members-of-Exchange-Distribution-Lists}

To work with members of distribution lists on MS Exchange Server, we will use [Aspose.Email for .NET][8]. It is a well-known API to create email client applications and work with MS Exchange Server. You can either [download][9] the API’s DLL or install it from [NuGet][10] using the following command.

```
PM> Install-Package Aspose.Email
```

## Add Members to MS Exchange Distribution Lists in C# {#Add-Members-to-MS-Exchange-Distribution-Lists}

The following are the steps to add members to MS Exchange distribution list in C# .NET.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient][11] object.
*   Then, get distribution lists into an [ExchangeDistributionList][12] array using [IEWSClient.ListDistributionLists()][13] method.
*   After that, create an instance of [MailAddressCollection][14] class and add members to the collection.
*   Finally, add members to the specific distribution list using [IEWSClient.AddToDistributionList(ExchangeDistributionList, MailAddressCollection)][15] method.

The following code sample shows how to add members to an Exchange distribution list in C#.

{{< gist aspose-com-gists d2e7147cd939cf4f09e6d5f5626d1b38 "add-members-to-list.cs" >}}

## Remove Members from MS Exchange Distribution Lists in C# {#Remove-Members-from-MS-Exchange-Distribution-Lists}

The following are the steps to remove members from MS Exchange distribution list using C# .NET.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient][16] object.
*   Then, get distribution lists into an [ExchangeDistributionList][17] array using [IEWSClient.ListDistributionLists()][18] method.
*   After that, get the reference of a particular list using [IEWSClient.FetchDistributionList(ExchangeDistributionList)][19] method.
*   Then, create an instance of [MailAddressCollection][20] class and add members to be deleted.
*   Finally, delete members from distribution list using [IEWSClient.DeleteFromDistributionList(ExchangeDistributionList, MailAddressCollection)][21] method.

The following code sample shows how to delete members from Exchange distribution lists in C#.

{{< gist aspose-com-gists d2e7147cd939cf4f09e6d5f5626d1b38 "remove-members-from-list.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][22] to use Aspose.Email for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to manage members in distribution lists on Microsoft Exchange Server. Particularly, you have seen how to add or remove members from Exchange distribution lists programmatically in C#. Alongside, you can explore the [documentation][23] to read more about Aspose.Email for .NET. Also, you can ask your questions via our [forum][24].

## See Also

*   [Read Emails from MS Exchange Server using C#][25]




[1]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[2]: https://blog.aspose.com/2022/03/06/create-exchange-distribution-list-in-csharp/
[3]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[4]: https://blog.aspose.com/2022/03/06/create-exchange-distribution-list-in-csharp/
[5]: #API-to-Manage-Members-of-Exchange-Distribution-Lists
[6]: #Add-Members-to-MS-Exchange-Distribution-Lists
[7]: #Remove-Members-from-MS-Exchange-Distribution-Lists
[8]: https://products.aspose.com/email/net/
[9]: https://downloads.aspose.com/email/net
[10]: https://www.nuget.org/packages/Aspose.Email/
[11]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[12]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange/exchangedistributionlist
[13]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/listdistributionlists
[14]: https://apireference.aspose.com/email/net/aspose.email/mailaddresscollection
[15]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/addtodistributionlist
[16]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[17]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange/exchangedistributionlist
[18]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/listdistributionlists
[19]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/fetchdistributionlist
[20]: https://apireference.aspose.com/email/net/aspose.email/mailaddresscollection
[21]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/deletefromdistributionlist
[22]: https://purchase.aspose.com/temporary-license
[23]: https://docs.aspose.com/email/net/
[24]: https://forum.aspose.com/
[25]: https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/




