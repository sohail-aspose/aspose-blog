---
title: 'Filtering Exchange Tasks by Status supported with Aspose.Email for Java 16.12.0'
date: Wed, 28 Dec 2016 18:32:43 +0000
draft: false
url: /2016/12/28/filtering-exchange-tasks-status-supported-aspose.email-java-16.12.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[![][1]](http://www.aspose.com/products/email/java)[Aspose.Email for Java 16.12.0][2] has been released. Ported form its’ equivalent .NET version, this month’s release provides the capability to filter tasks from exchange server based on the task status. It also improves the IMAP and Exchange server APIs to search for messages by specifying time in addition to date. For a complete list of what is new and fixed, please visit the release notes section of Aspose.Email for Java.

# Enhancements

**Filtering Tasks from Exchange Server:** This month’s release enhances the capability of Aspose.Email API in terms of working with tasks on Exchange server. This new capability enables users to retrieve filtered tasks from Exchange server based on the specified criterion. The filtering options include the task’s statuses such as:

*   Completed
*   Deferred
*   In Progress
*   Not Started
*   Waiting on others

This is achieved by using the _TaskStatus_ property of _ExchangeQueryBuilder_ class that allows to define the criterion as a single or combination of various task statuses, as shown in the code sample below.

```
ExchangeQueryBuilder queryBuilder = null;
MailQuery query = null;
ExchangeTask fetchedTask = null;
ExchangeMessageInfoCollection messageInfoCol = null;

//Set timezone for tasks
client.setTimezoneId("Central Europe Standard Time");

//We use these status values for specifying in queries
Integer[] values = new Integer[] {ExchangeTaskStatus.Completed, ExchangeTaskStatus.Deferred,
        ExchangeTaskStatus.InProgress, ExchangeTaskStatus.NotStarted, ExchangeTaskStatus.WaitingOnOthers};

messageInfoCol = client.listMessages(client.getMailboxInfo().getTasksUri());

//Now retrieve the tasks with specific statuses
for (int status : values)
{
    queryBuilder = new ExchangeQueryBuilder();
    queryBuilder.getTaskStatus().equals(status);
    query = queryBuilder.getQuery();
    messageInfoCol = client.listMessages(client.getMailboxInfo().getTasksUri(), query);
    fetchedTask = client.fetchTask(messageInfoCol.get_Item(0).getUniqueUri());
}

//retrieve all other than specified
for (int status : values)
{
    queryBuilder = new ExchangeQueryBuilder();
    queryBuilder.getTaskStatus().notEquals((int)status);
    query = queryBuilder.getQuery();
    messageInfoCol = client.listMessages(client.getMailboxInfo().getTasksUri(), query);
}

//specifying multiple criterion
Integer[] selectedStatuses = new Integer[]
        {
                ExchangeTaskStatus.Completed,
                ExchangeTaskStatus.InProgress
        };
queryBuilder = new ExchangeQueryBuilder();
queryBuilder.getTaskStatus().in(Arrays.asList(selectedStatuses));
query = queryBuilder.getQuery();
messageInfoCol = client.listMessages(client.getMailboxInfo().getTasksUri(), query);

queryBuilder = new ExchangeQueryBuilder();
queryBuilder.getTaskStatus().notIn(Arrays.asList(selectedStatuses));
query = queryBuilder.getQuery();
messageInfoCol = client.listMessages(client.getMailboxInfo().getTasksUri(), query); 
```

**Filtering Messages from Server by Date Time:** This month’s release also improves the functionality of IMAP and EWS clients to filter messages by date and time. Now, the API takes into account the time part as well for comparison which can be utilized using the DateComparisonType.ByDateTime property in MailQuery.

# Other Improvements

This month’s release also fixes several bugs that were either resolved in .NET equivalent API or were directly reported in the Java API. This further adds stability to the overall functionality of the API.

# API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   Product Documentation – Provides detailed examples of working with the API
*   [API Reference Guide][3] – Details all the packages and classes of the API
*   [GitHub Examples][4] – Provides ready to run API examples
*   [Aspose.Email Forum][5] – Feel free to contact us on Aspose.Email forum for your queries




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2016/11/aspose-Email-for-Java_100.png
[2]: http://downloads.aspose.com/email/java
[3]: http://www.aspose.com/api/java/email
[4]: https://github.com/aspose-email/Aspose.Email-for-Java
[5]: https://forum.aspose.com/c/email




