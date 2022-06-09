---
title: 'Manage Inbox Rules on Exchange Server in C#'
seoTitle: "C# Create and Update Inbox Rules with EWS on Exchange Server | .NET"
description: "Use .NET EWS API to manage inbox rules on Exchange Server using C#. Create and update inbox rules with EWS on Exchange Server programmatically."
date: Sun, 13 Mar 2022 06:06:00 +0000
draft: false
url: /2022/03/13/manage-inbox-rules-on-exchange-server-in-csharp/
author: Usman Aziz
summary: '[Microsoft Exchange Server][1] allows you to define different rules for the inbox, which are applied to the messages such as moving a message to a folder, deleting a message, etc. While working with the Exchange services from within .NET applications, you may need to manage inbox rules programmatically. In this article, you will learn **how to create and update inbox rules on MS Exchange Server in C# .NET**.'
tags: ['Create Inbox Rules on Exchange Server Csharp', 'DotNet API to Manage Inbox Rules on Exchange Server', 'DotNet EWS API', 'Update Inbox Rules on Exchange Server Csharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Manage Inbox Rules on Exchange Server in C#">}}


[Microsoft Exchange Server][2] allows you to define different rules for the inbox, which are applied to the messages such as moving a message to a folder, deleting a message, etc. While working with the Exchange services from within .NET applications, you may need to manage inbox rules programmatically. In this article, you will learn **how to create and update inbox rules on MS Exchange Server in C# .NET**.

*   [.NET API to Manage Inbox Rules on Exchange Server][3]
*   [Create Inbox Rules on Exchange Server][4]
*   [Update Inbox Rules on Exchange Server][5]

## .NET API to Manage Inbox Rules on Exchange Server {#API-to-Manage-Inbox-Rules-on-Exchange-Server}

To create and update inbox rules on MS Exchange Server, we will use [Aspose.Email for .NET][6]. The API makes it quite easier to seamlessly work with MS Exchange Server. You can either [download][7] the API’s DLL or install it from [NuGet][8] using the following command.

```
PM> Install-Package Aspose.Email
```

## Create Inbox Rules on Exchange Server in C# {#Create-Inbox-Rules-on-Exchange-Server}

Aspose.Email for .NET uses Exchange Web Services (EWS) to work with inbox rules on Exchange Server. The following are the steps to create inbox rules on Exchange Server in C#.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient][9] object.
*   Then, create an object of [InboxRule][10] class.
*   Set rule's name using [InboxRule.DisplayName][11] property.
*   Create an instance of [RulePredicates][12] class and specify the conditions.
*   Assign _RulePredicates_ instance to [InboxRule.Conditions][13] property.
*   Create an instance of [RuleActions][14] class and set actions.
*   Assign _RuleAction_ instance to [InboxRule.Actions][15] property.
*   Finally, call [IEWSClient.CreateInboxRule(InboxRule)][16] to create the rule.

The following code sample shows how to create an inbox rule on Exchange Server in C#.

{{< gist aspose-com-gists 573e3e9dd326e62aca89590d74f43998 "create-inbox-rule.cs" >}}

## Update Inbox Rules on Exchange Server in C# {#Update-Inbox-Rules-on-Exchange-Server}

The following are the steps to fetch and update an existing inbox rule on Exchange Server in C#.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient][17] object.
*   Then, call the [IEWSClient.GetInboxRules()][18] method to get all the rules in an [InboxRule][19] array.
*   Loop through each _InboxRule_ in the array.
*   Filter the required rules based on some conditions.
*   Update the rule's conditions or actions.
*   Finally, call [IEWSClient.UpdateInboxRule(InboxRule)][20] method to update the inbox rule.

The following code sample shows how to update an inbox rule on MS Exchange Server in C#.

{{< gist aspose-com-gists 573e3e9dd326e62aca89590d74f43998 "update-inbox-rule.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][21] to use Aspose.Email for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to work with inbox rules on Microsoft Exchange Server from within .NET applications. With the help of code samples, you have seen how to add or update inbox rules on Exchange Server in C#. Besides, you can explore the [documentation][22] to read more about Aspose.Email for .NET. In addition, you can post your queries to our [forum][23].

## See Also

*   [Read Emails from MS Exchange Server using C#][24]




[1]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[2]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[3]: #API-to-Manage-Inbox-Rules-on-Exchange-Server
[4]: #Create-Inbox-Rules-on-Exchange-Server
[5]: #Update-Inbox-Rules-on-Exchange-Server
[6]: https://products.aspose.com/email/net/
[7]: https://downloads.aspose.com/email/net
[8]: https://www.nuget.org/packages/Aspose.Email/
[9]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[10]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange/inboxrule
[11]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange/inboxrule/properties/displayname
[12]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange/rulepredicates
[13]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange/inboxrule/properties/conditions
[14]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange/ruleactions
[15]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange/inboxrule/properties/actions
[16]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/createinboxrule
[17]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[18]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/getinboxrules
[19]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange/inboxrule
[20]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/updateinboxrule
[21]: https://purchase.aspose.com/temporary-license
[22]: https://docs.aspose.com/email/net/
[23]: https://forum.aspose.com/
[24]: https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/




