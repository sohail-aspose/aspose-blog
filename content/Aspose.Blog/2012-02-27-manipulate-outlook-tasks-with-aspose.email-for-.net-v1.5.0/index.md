---
title: 'Manipulate Outlook Tasks with Aspose.Email for .NET v1.5.0'
date: Mon, 27 Feb 2012 18:19:08 +0000
draft: false
url: /2012/02/27/manipulate-outlook-tasks-with-aspose.email-for-.net-v1.5.0/
author: Babar Raza
summary: ''
tags: ['Home', 'Outlook', 'exchange', 'tasks']
categories: ['Aspose.Total Product Family', 'Aspose.Email Product Family']
---

[![Aspose.Email for .NET][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2012/02/aspose.email-logo120.jpg)We are pleased to announce the release of Aspose.Email for .NET 1.5.0. This release includes some great new features such as email conversion to EMLX format, extraction of tasks from PST file, listing any number of messages using the ImapClient class and much more.

Check the [release notes][2] to get a full list of new features and enhancements included in Aspose.Email for .NET 1.5.0.

## Create, Update and Delete Outlook Tasks

The most exciting feature from this release is to manipulate tasks on an Exchange Server. For this purpose we have added a new class called ExchangeTask and some new methods to the ExchangeWebServiceClient class that enables you to create, delete and update tasks on the Exchange Server.

The code segment below shows how to create a task.

```
ExchangeWebServiceClient client = new ExchangeWebServiceClient(host, credentials);
ExchangeTask task = new ExchangeTask();
task.Subject = "New-Test";
task.Status = ExchangeTaskStatus.InProgress;
client.CreateTask(client.MailboxInfo.TasksUri, task);
```

You can also update an existing tasks by using the UpdateTask method exposed by the ExchangeWebServiceClient class. The sample code below shows how to use the UpdateTask method.

```
ExchangeMessageInfoCollection tasks = client.ListMessages(client.MailboxInfo.TasksUri);
foreach (ExchangeMessageInfo info in tasks)
{
     ExchangeTask task = client.FetchTask(info.UniqueUri);
     task.Status = ExchangeTaskStatus.NotStarted;
     task.DueDate = new DateTime(2012, 9, 26);
     task.Priority = MailPriority.Low;
     client.UpdateTask(task);
}
```

To delete a task, use the DeleteTask method exposed by the ExchangeWebServiceClient class and pass the task's unique URI, along with an appropriate value from the DeleteTasksOptions enumerator.

```
ExchangeMessageInfoCollection tasks = client.ListMessages(client.MailboxInfo.TasksUri);
foreach (ExchangeMessageInfo info in tasks)
{
    ExchangeTask task = client.FetchTask(info.UniqueUri);
    if (task.Subject.Equals("test"))
    {
        client.DeleteTask(task.UniqueUri, DeleteTaskOptions.DeletePermanently);
    }
}
```




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2012/02/aspose.email-logo120.jpg
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.email-for-.net/entry363550.aspx "Release Notes of Aspose.Email for .NET v1.5.0"




