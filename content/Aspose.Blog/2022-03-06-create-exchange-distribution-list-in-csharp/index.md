---
title: 'Create Exchange Distribution List in C# .NET'
date: Sun, 06 Mar 2022 18:08:00 +0000
draft: false
url: /2022/03/06/create-exchange-distribution-list-in-csharp/
author: ''Usman Aziz''
summary: '[MS Exchange Server][1] provides the feature of creating distribution lists or groups. These distribution lists allow you to send emails to a group of people without requiring you to enter individual email addresses. In this article, you will learn **how to create a distribution list on MS Exchange Server in C# .NET**. Furthermore, we will cover how to fetch a distribution list programmatically.'
tags: ['Create an MS Exchange Distribution List Csharp', 'Fetch a Distribution List from MS Exchange Server Cshapr', 'Work with Exchange Distribution List in CSharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Create Exchange Distribution List in C# .NET">}}


[MS Exchange Server][2] provides the feature of creating distribution lists or groups. These distribution lists allow you to send emails to a group of people without requiring you to enter individual email addresses. In this article, you will learn **how to create a distribution list on MS Exchange Server in C# .NET**. Furthermore, we will cover how to fetch a distribution list programmatically.

*   [.NET API to Create Distribution List on MS Exchange Server][3]
*   [Create an MS Exchange Distribution List][4]
*   [Fetch a Distribution List from MS Exchange Server][5]

## C# .NET API to Create Distribution List on MS Exchange Server {#API-to-Create-Distribution-List-on-MS-Exchange-Server}

To create the distribution lists on MS Exchange Server, we will use [Aspose.Email for .NET][6]. It is a powerful API to create, send, and process emails from within .NET applications. In addition, it allows you to work with MS Outlook and Exchange Server seamlessly. You can either [download][7] the API’s DLL or install it from [NuGet][8] using the following command.

```
PM> Install-Package Aspose.Email
```

## Create an MS Exchange Distribution List in C# {#Create-an-MS-Exchange-Distribution-List}

The following are the steps to create a distribution list on MS Exchange Server in C#.

*   First, specify the network credentials.
*   Then, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient][9] object.
*   Create an instance of [ExchangeDistributionList][10] class.
*   Set display name of list using [ExchangeDistributionList.DisplayName][11] property.
*   Create an instance of [MailAddressCollection][12] class and add members to the collection.
*   Finally, create distribution list using [IEWSClient.CreateDistributionList(ExchangeDistributionList, MailAddressCollection)][13] method.

The following code sample shows how to create an MS Exchange distribution list in C#.

{{< gist aspose-com-gists 5dcd8815c04f506f518ca26c77afd0d0 "create-distribution-list.cs" >}}

## Fetch a Distribution List from MS Exchange Server in C# {#Fetch-a-Distribution-List-from-MS-Exchange-Server}

Now, let's see how to fetch a distribution list from MS Exchange Server programmatically in C#.

*   Specify the network credentials.
*   Connect to Exchange Server and get the instance of the EWS client into an [IEWSClient][14] object.
*   Get distribution list into an [ExchangeDistributionList][15] array using [IEWSClient.ListDistributionLists()][16] method.
*   Loop through each distribution list in the array.
*   Use [IEWSClient.FetchDistributionList(ExchangeDistributionList)][17] method to fetch the members of the distribution list.

The following code sample shows how to fetch distribution lists from MS Exchange Server in C#.

{{< gist aspose-com-gists 5dcd8815c04f506f518ca26c77afd0d0 "fetch-distribution-list.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][18] to use Aspose.Email for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to create distribution lists on MS Exchange Server in C#. Furthermore, you have seen how to fetch MS Exchange distribution lists programmatically. Besides, you can read about other features of Aspose.Email for .NET from the [documentation][19]. Also, you can post your queries to our [forum][20].

## See Also

*   [Read Emails from MS Exchange Server using C#][21]




[1]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[2]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[3]: #API-to-Create-Distribution-List-on-MS-Exchange-Server
[4]: #Create-an-MS-Exchange-Distribution-List
[5]: #Fetch-a-Distribution-List-from-MS-Exchange-Server
[6]: https://products.aspose.com/email/net/
[7]: https://downloads.aspose.com/email/net
[8]: https://www.nuget.org/packages/Aspose.Email/
[9]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[10]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange/exchangedistributionlist
[11]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange/exchangedistributionlist/properties/displayname
[12]: https://apireference.aspose.com/email/net/aspose.email/mailaddresscollection
[13]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/createdistributionlist
[14]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[15]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange/exchangedistributionlist
[16]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/listdistributionlists
[17]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/fetchdistributionlist
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/email/net/
[20]: https://forum.aspose.com/
[21]: https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/




