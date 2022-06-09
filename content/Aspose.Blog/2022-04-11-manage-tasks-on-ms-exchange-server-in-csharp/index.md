---
title: 'Create, Update or Delete Tasks on MS Exchange Server in C#'
seoTitle: "C# Create, Update or Delete Tasks on MS Exchange Server | .NET EWS"
description: "Use .NET EWS API to manage tasks on MS Exchange Server in C#. Add, update or delete tasks on MS Exchange Server programmatically."
date: Mon, 11 Apr 2022 16:03:00 +0000
draft: false
url: /2022/04/11/manage-tasks-on-ms-exchange-server-in-csharp/
author: Usman Aziz
summary: 'Various people create a list of activities to be performed, which is also known as a to-do list. Such lists are usually created on a paper, text editor, spreadsheets, etc. Microsoft also provides you the feature of creating and managing to-do lists and terms them as tasks. In this article, we will cover **how to add, update, or delete tasks on MS Exchange Server programmatically in C#**.'
tags: ['Create Task on MS Exchange Server in Csharp', 'Delete Task on MS Exchange Server in Csharp', 'DotNet API to Manage Tasks on MS Exchange', 'Update Task on MS Exchange Server in Csharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Create, Update or Delete Tasks on MS Exchange Server in C#">}}


Various people create a list of activities to be performed, which is also known as a to-do list. Such lists are usually created on a paper, text editor, spreadsheets, etc. Microsoft also provides you the feature of creating and managing to-do lists and terms them as tasks. In this article, we will cover **how to add, update, or delete tasks on MS Exchange Server programmatically in C#**.

*   [.NET API to Manage Tasks on MS Exchange Server][1]
*   [Create a Task on MS Exchange Server in C#][2]
*   [Update a Task on MS Exchange Server in C#][3]
*   [Delete Tasks on MS Exchange Server in C#][4]

## .NET API to Manage Tasks on MS Exchange Server {#API-to-Manage-Tasks-on-MS-Exchange}

To create, update, or delete tasks on MS Exchange Server, we will use [Aspose.Email for .NET][5]. It is a feature-rich API to create email client applications and work with MS Exchange Server without writing complex code. You can either [download][6] the API’s DLL or install it from [NuGet][7] using the following command.

```
PM> Install-Package Aspose.Email
```

## Create a Task on MS Exchange Server in C# {#Create-Task-on-MS-Exchange-Server}

The following are the steps to create tasks on MS Exchange Server in C# .NET.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient][8] object.
*   Then, create an instance of [ExchangeTask][9] class.
*   Set properties of tasks such as subject, status, etc.
*   Finally, create task using [IEWSClient.CreateTask(IEWSClient.MailboxInfo.TasksUri, ExchangeTask)][10] method.

The following code sample shows how to create tasks on MS Exchange Server using C#.

{{< gist aspose-com-gists af8bf4d377998e3ccc9d1bbcbad8fc85 "create-task.cs" >}}

## Update Task on MS Exchange Server in C# {#Update-Task-on-MS-Exchange-Server}

You can also access and update the existing tasks on MS Exchange Server programmatically using C#. The following are the steps to perform this operation.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient][11] object.
*   Then, get lists of tasks into an [ExchangeMessageInfoCollection][12] object using [IEWSClient.ListMessages(IEWSClient.MailboxInfo.TasksUri)][13] method.
*   Loop through each [ExchangeMessageInfo][14] in the collection.
*   Fetch each [ExchangeTask][15] using [IEWSClient.FetchTask(ExchangeMessageInfo.UniqueUri)][16] method and filter the required one(s).
*   Finally, edit properties and update the task using [IEWSClient.UpdateTask(ExchangeTask)][17] method.

The following code sample shows how to update a task on MS Exchange Server in C#.

{{< gist aspose-com-gists af8bf4d377998e3ccc9d1bbcbad8fc85 "update-task.cs" >}}

## Delete Tasks on MS Exchange Server in C# {#Delete-Task-on-MS-Exchange-Server}

The following are the steps to delete tasks on MS Exchange server in C#.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient][18] object.
*   Then, get lists of tasks into an [ExchangeMessageInfoCollection][19] object using [IEWSClient.ListMessages(IEWSClient.MailboxInfo.TasksUri)][20] method.
*   Loop through each [ExchangeMessageInfo][21] in the collection.
*   Fetch each [ExchangeTask][22] using [IEWSClient.FetchTask(ExchangeMessageInfo.UniqueUri)][23] method and filter the required one(s).
*   Finally, delete the task using [IEWSClient.DeleteItem(ExchangeTask.UniqueUri, DeletionOptions.DeletePermanently)][24] method.

The following code sample shows how to delete tasks from MS Exchange Server in C#.

{{< gist aspose-com-gists af8bf4d377998e3ccc9d1bbcbad8fc85 "delete-task.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][25] to use Aspose.Email for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to manage tasks on Microsoft Exchange Server. Particularly, you have seen how to add, update, or delete tasks on MS Exchange Server programmatically in C#. Alongside, you can explore the [documentation][26] to read more about Aspose.Email for .NET. Also, you can ask your questions via our [forum][27].

## See Also

*   [Read Emails from MS Exchange Server using C#][28]




[1]: #API-to-Manage-Tasks-on-MS-Exchange
[2]: #Create-Task-on-MS-Exchange-Server
[3]: #Update-Task-on-MS-Exchange-Server
[4]: #Delete-Task-on-MS-Exchange-Server
[5]: https://products.aspose.com/email/net/
[6]: https://downloads.aspose.com/email/net
[7]: https://www.nuget.org/packages/Aspose.Email/
[8]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[9]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/exchangetask
[10]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/createtask
[11]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[12]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange/exchangemessageinfocollection
[13]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice.iewsclient/listmessages/methods/2
[14]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange/exchangemessageinfo
[15]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/exchangetask
[16]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/fetchtask
[17]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/updatetask
[18]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[19]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange/exchangemessageinfocollection
[20]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice.iewsclient/listmessages/methods/2
[21]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange/exchangemessageinfo
[22]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/exchangetask
[23]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/fetchtask
[24]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/deleteitem
[25]: https://purchase.aspose.com/temporary-license
[26]: https://docs.aspose.com/email/net/
[27]: https://forum.aspose.com/
[28]: https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/




