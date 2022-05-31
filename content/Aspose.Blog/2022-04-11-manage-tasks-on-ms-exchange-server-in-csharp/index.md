---
title: 'Create, Update or Delete Tasks on MS Exchange Server in C#'
date: Mon, 11 Apr 2022 16:03:00 +0000
draft: false
url: /2022/04/11/manage-tasks-on-ms-exchange-server-in-csharp/
author: 'Usman Aziz'
summary: 'Various people create a list of activities to be performed, which is also known as a to-do list. Such lists are usually created on a paper, text editor, spreadsheets, etc. Microsoft also provides you the feature of creating and managing to-do lists and terms them as tasks. In this article, we will cover **how to add, update, or delete tasks on MS Exchange Server programmatically in C#**.'
tags: ['Create Task on MS Exchange Server in Csharp', 'Delete Task on MS Exchange Server in Csharp', 'DotNet API to Manage Tasks on MS Exchange', 'Update Task on MS Exchange Server in Csharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Create, Update or Delete Tasks on MS Exchange Server in C#">}}


Various people create a list of activities to be performed, which is also known as a to-do list. Such lists are usually created on a paper, text editor, spreadsheets, etc. Microsoft also provides you the feature of creating and managing to-do lists and terms them as tasks. In this article, we will cover **how to add, update, or delete tasks on MS Exchange Server programmatically in C#**.

*   [.NET API to Manage Tasks on MS Exchange Server](#API-to-Manage-Tasks-on-MS-Exchange)
*   [Create a Task on MS Exchange Server in C#](#Create-Task-on-MS-Exchange-Server)
*   [Update a Task on MS Exchange Server in C#](#Update-Task-on-MS-Exchange-Server)
*   [Delete Tasks on MS Exchange Server in C#](#Delete-Task-on-MS-Exchange-Server)

## .NET API to Manage Tasks on MS Exchange Server {#API-to-Manage-Tasks-on-MS-Exchange}

To create, update, or delete tasks on MS Exchange Server, we will use [Aspose.Email for .NET](https://products.aspose.com/email/net/). It is a feature-rich API to create email client applications and work with MS Exchange Server without writing complex code. You can either [download](https://downloads.aspose.com/email/net) the API’s DLL or install it from [NuGet](https://www.nuget.org/packages/Aspose.Email/) using the following command.

```
PM> Install-Package Aspose.Email
```

## Create a Task on MS Exchange Server in C# {#Create-Task-on-MS-Exchange-Server}

The following are the steps to create tasks on MS Exchange Server in C# .NET.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient) object.
*   Then, create an instance of [ExchangeTask](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/exchangetask) class.
*   Set properties of tasks such as subject, status, etc.
*   Finally, create task using [IEWSClient.CreateTask(IEWSClient.MailboxInfo.TasksUri, ExchangeTask)](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/createtask) method.

The following code sample shows how to create tasks on MS Exchange Server using C#.

\[gist id="af8bf4d377998e3ccc9d1bbcbad8fc85" file="create-task.cs"\]

## Update Task on MS Exchange Server in C# {#Update-Task-on-MS-Exchange-Server}

You can also access and update the existing tasks on MS Exchange Server programmatically using C#. The following are the steps to perform this operation.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient) object.
*   Then, get lists of tasks into an [ExchangeMessageInfoCollection](https://apireference.aspose.com/email/net/aspose.email.clients.exchange/exchangemessageinfocollection) object using [IEWSClient.ListMessages(IEWSClient.MailboxInfo.TasksUri)](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice.iewsclient/listmessages/methods/2) method.
*   Loop through each [ExchangeMessageInfo](https://apireference.aspose.com/email/net/aspose.email.clients.exchange/exchangemessageinfo) in the collection.
*   Fetch each [ExchangeTask](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/exchangetask) using [IEWSClient.FetchTask(ExchangeMessageInfo.UniqueUri)](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/fetchtask) method and filter the required one(s).
*   Finally, edit properties and update the task using [IEWSClient.UpdateTask(ExchangeTask)](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/updatetask) method.

The following code sample shows how to update a task on MS Exchange Server in C#.

\[gist id="af8bf4d377998e3ccc9d1bbcbad8fc85" file="update-task.cs"\]

## Delete Tasks on MS Exchange Server in C# {#Delete-Task-on-MS-Exchange-Server}

The following are the steps to delete tasks on MS Exchange server in C#.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient) object.
*   Then, get lists of tasks into an [ExchangeMessageInfoCollection](https://apireference.aspose.com/email/net/aspose.email.clients.exchange/exchangemessageinfocollection) object using [IEWSClient.ListMessages(IEWSClient.MailboxInfo.TasksUri)](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice.iewsclient/listmessages/methods/2) method.
*   Loop through each [ExchangeMessageInfo](https://apireference.aspose.com/email/net/aspose.email.clients.exchange/exchangemessageinfo) in the collection.
*   Fetch each [ExchangeTask](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/exchangetask) using [IEWSClient.FetchTask(ExchangeMessageInfo.UniqueUri)](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/fetchtask) method and filter the required one(s).
*   Finally, delete the task using [IEWSClient.DeleteItem(ExchangeTask.UniqueUri, DeletionOptions.DeletePermanently)](https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/deleteitem) method.

The following code sample shows how to delete tasks from MS Exchange Server in C#.

\[gist id="af8bf4d377998e3ccc9d1bbcbad8fc85" file="delete-task.cs"\]

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license](https://purchase.aspose.com/temporary-license) to use Aspose.Email for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to manage tasks on Microsoft Exchange Server. Particularly, you have seen how to add, update, or delete tasks on MS Exchange Server programmatically in C#. Alongside, you can explore the [documentation](https://docs.aspose.com/email/net/) to read more about Aspose.Email for .NET. Also, you can ask your questions via our [forum](https://forum.aspose.com/).

## See Also

*   [Read Emails from MS Exchange Server using C#](https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/)



