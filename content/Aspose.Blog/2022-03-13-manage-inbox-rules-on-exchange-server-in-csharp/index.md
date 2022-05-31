---
title: 'Manage Inbox Rules on Exchange Server in C#'
date: Sun, 13 Mar 2022 06:06:00 +0000
draft: false
url: /2022/03/13/manage-inbox-rules-on-exchange-server-in-csharp/
author: 'Usman Aziz'
summary: '[Microsoft Exchange Server](https://en.wikipedia.org/wiki/Microsoft_Exchange_Server) allows you to define different rules for the inbox, which are applied to the messages such as moving a message to a folder, deleting a message, etc. While working with the Exchange services from within .NET applications, you may need to manage inbox rules programmatically. In this article, you will learn **how to create and update inbox rules on MS Exchange Server in C# .NET**.'
tags: ['Create Inbox Rules on Exchange Server Csharp', 'DotNet API to Manage Inbox Rules on Exchange Server', 'DotNet EWS API', 'Update Inbox Rules on Exchange Server Csharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Manage Inbox Rules on Exchange Server in C#">}}


[Microsoft Exchange Server](https://en.wikipedia.org/wiki/Microsoft_Exchange_Server) allows you to define different rules for the inbox, which are applied to the messages such as moving a message to a folder, deleting a message, etc. While working with the Exchange services from within .NET applications, you may need to manage inbox rules programmatically. In this article, you will learn **how to create and update inbox rules on MS Exchange Server in C# .NET**.

*   [.NET API to Manage Inbox Rules on Exchange Server](#API-to-Manage-Inbox-Rules-on-Exchange-Server)
*   [Create Inbox Rules on Exchange Server](#Create-Inbox-Rules-on-Exchange-Server)
*   [Update Inbox Rules on Exchange Server](#Update-Inbox-Rules-on-Exchange-Server)

## .NET API to Manage Inbox Rules on Exchange Server {#API-to-Manage-Inbox-Rules-on-Exchange-Server}

To create and update inbox rules on MS Exchange Server, we will use [Aspose.Email for .NET](https://products.aspose.com/email/net/). The API makes it quite easier to seamlessly work with MS Exchange Server. You can either [download](https://downloads.aspose.com/email/net) the API’s DLL or install it from [NuGet](https://www.nuget.org/packages/Aspose.Email/) using the following command.

```
PM> Install-Package Aspose.Email
```

## Create Inbox Rules on Exchange Server in C# {#Create-Inbox-Rules-on-Exchange-Server}

Aspose.Email for .NET uses Exchange Web Services (EWS) to work with inbox rules on Exchange Server. The following are the steps to create inbox rules on Exchange Server in C#.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient) object.
*   Then, create an object of [InboxRule](https://apireference.aspose.com/email/net/aspose.email.clients.exchange/inboxrule) class.
*   Set rule's name using [InboxRule.DisplayName](https://apireference.aspose.com/email/net/aspose.email.clients.exchange/inboxrule/properties/displayname) property.
*   Create an instance of [RulePredicates](https://apireference.aspose.com/email/net/aspose.email.clients.exchange/rulepredicates) class and specify the conditions.
*   Assign _RulePredicates_ instance to [InboxRule.Conditions](https://apireference.aspose.com/email/net/aspose.email.clients.exchange/inboxrule/properties/conditions) property.
*   Create an instance of [RuleActions](https://apireference.aspose.com/email/net/aspose.email.clients.exchange/ruleactions) class and set actions.
*   Assign _RuleAction_ instance to [InboxRule.Actions](https://apireference.aspose.com/email/net/aspose.email.clients.exchange/inboxrule/properties/actions) property.
*   Finally, call [IEWSClient.CreateInboxRule(InboxRule)](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/createinboxrule) to create the rule.

The following code sample shows how to create an inbox rule on Exchange Server in C#.

\[gist id="573e3e9dd326e62aca89590d74f43998" file="create-inbox-rule.cs"\]

## Update Inbox Rules on Exchange Server in C# {#Update-Inbox-Rules-on-Exchange-Server}

The following are the steps to fetch and update an existing inbox rule on Exchange Server in C#.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient) object.
*   Then, call the [IEWSClient.GetInboxRules()](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/getinboxrules) method to get all the rules in an [InboxRule](https://apireference.aspose.com/email/net/aspose.email.clients.exchange/inboxrule) array.
*   Loop through each _InboxRule_ in the array.
*   Filter the required rules based on some conditions.
*   Update the rule's conditions or actions.
*   Finally, call [IEWSClient.UpdateInboxRule(InboxRule)](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/updateinboxrule) method to update the inbox rule.

The following code sample shows how to update an inbox rule on MS Exchange Server in C#.

\[gist id="573e3e9dd326e62aca89590d74f43998" file="update-inbox-rule.cs"\]

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license](https://purchase.aspose.com/temporary-license) to use Aspose.Email for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to work with inbox rules on Microsoft Exchange Server from within .NET applications. With the help of code samples, you have seen how to add or update inbox rules on Exchange Server in C#. Besides, you can explore the [documentation](https://docs.aspose.com/email/net/) to read more about Aspose.Email for .NET. In addition, you can post your queries to our [forum](https://forum.aspose.com/).

## See Also

*   [Read Emails from MS Exchange Server using C#](https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/)



