---
title: 'Add and Remove Members in MS Exchange Distribution Lists in C#'
date: Thu, 07 Apr 2022 04:25:00 +0000
draft: false
url: /2022/04/07/manage-members-in-exchange-distribution-list-in-csharp/
author: 'Usman Aziz'
summary: 'While working with [MS Exchange Server](https://en.wikipedia.org/wiki/Microsoft_Exchange_Server) from within .NET applications, you may need to work with distribution lists. In the [previous post](https://blog.aspose.com/2022/03/06/create-exchange-distribution-list-in-csharp/), you have seen how to create and fetch Exchange distribution lists. In this article, you will learn **how to add or remove members in MS Exchange distribution lists programmatically in C# .NET**.'
tags: ['Add Members to MS Exchange Distribution Lists in Csharp', 'DotNet API to Manage Members of Exchange Distribution Lists', 'DotNet EWS API', 'Remove Members from MS Exchange Distribution Lists in Csharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Add and Remove Members from MS Exchange Distribution Lists in C#">}}


While working with [MS Exchange Server](https://en.wikipedia.org/wiki/Microsoft_Exchange_Server) from within .NET applications, you may need to work with distribution lists. In the [previous post](https://blog.aspose.com/2022/03/06/create-exchange-distribution-list-in-csharp/), you have seen how to create and fetch Exchange distribution lists. In this article, you will learn **how to add or remove members in MS Exchange distribution lists programmatically in C# .NET**.

*   [.NET API to Manage Members of Exchange Distribution Lists](#API-to-Manage-Members-of-Exchange-Distribution-Lists)
*   [Add Members to MS Exchange Distribution Lists](#Add-Members-to-MS-Exchange-Distribution-Lists)
*   [Remove Members from MS Exchange Distribution Lists](#Remove-Members-from-MS-Exchange-Distribution-Lists)

## .NET API to Manage Members of Exchange Distribution Lists {#API-to-Manage-Members-of-Exchange-Distribution-Lists}

To work with members of distribution lists on MS Exchange Server, we will use [Aspose.Email for .NET](https://products.aspose.com/email/net/). It is a well-known API to create email client applications and work with MS Exchange Server. You can either [download](https://downloads.aspose.com/email/net) the API’s DLL or install it from [NuGet](https://www.nuget.org/packages/Aspose.Email/) using the following command.

```
PM> Install-Package Aspose.Email
```

## Add Members to MS Exchange Distribution Lists in C# {#Add-Members-to-MS-Exchange-Distribution-Lists}

The following are the steps to add members to MS Exchange distribution list in C# .NET.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient) object.
*   Then, get distribution lists into an [ExchangeDistributionList](https://apireference.aspose.com/email/net/aspose.email.clients.exchange/exchangedistributionlist) array using [IEWSClient.ListDistributionLists()](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/listdistributionlists) method.
*   After that, create an instance of [MailAddressCollection](https://apireference.aspose.com/email/net/aspose.email/mailaddresscollection) class and add members to the collection.
*   Finally, add members to the specific distribution list using [IEWSClient.AddToDistributionList(ExchangeDistributionList, MailAddressCollection)](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/addtodistributionlist) method.

The following code sample shows how to add members to an Exchange distribution list in C#.

{{< gist aspose-com-gists d2e7147cd939cf4f09e6d5f5626d1b38 "add-members-to-list.cs" >}}

## Remove Members from MS Exchange Distribution Lists in C# {#Remove-Members-from-MS-Exchange-Distribution-Lists}

The following are the steps to remove members from MS Exchange distribution list using C# .NET.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient) object.
*   Then, get distribution lists into an [ExchangeDistributionList](https://apireference.aspose.com/email/net/aspose.email.clients.exchange/exchangedistributionlist) array using [IEWSClient.ListDistributionLists()](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/listdistributionlists) method.
*   After that, get the reference of a particular list using [IEWSClient.FetchDistributionList(ExchangeDistributionList)](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/fetchdistributionlist) method.
*   Then, create an instance of [MailAddressCollection](https://apireference.aspose.com/email/net/aspose.email/mailaddresscollection) class and add members to be deleted.
*   Finally, delete members from distribution list using [IEWSClient.DeleteFromDistributionList(ExchangeDistributionList, MailAddressCollection)](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/deletefromdistributionlist) method.

The following code sample shows how to delete members from Exchange distribution lists in C#.

{{< gist aspose-com-gists d2e7147cd939cf4f09e6d5f5626d1b38 "remove-members-from-list.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license](https://purchase.aspose.com/temporary-license) to use Aspose.Email for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to manage members in distribution lists on Microsoft Exchange Server. Particularly, you have seen how to add or remove members from Exchange distribution lists programmatically in C#. Alongside, you can explore the [documentation](https://docs.aspose.com/email/net/) to read more about Aspose.Email for .NET. Also, you can ask your questions via our [forum](https://forum.aspose.com/).

## See Also

*   [Read Emails from MS Exchange Server using C#](https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/)




