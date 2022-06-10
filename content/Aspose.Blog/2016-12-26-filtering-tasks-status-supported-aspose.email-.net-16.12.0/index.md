---
title: 'Filtering Tasks by Status supported with Aspose.Email for .NET 16.12.0'
date: Mon, 26 Dec 2016 10:30:50 +0000
draft: false
url: /2016/12/26/filtering-tasks-status-supported-aspose.email-.net-16.12.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[![Aspose.Email for .NET][1]](http://www.aspose.com/products/email/net) We are pleased to announce the release of [Aspose.Email for .NET 16.12.0][2]. This month’s release includes a number of enhancements for working with tasks on Exchange server and searching messages by specifying date time. It also fixes a number of bugs related to the API that further improves the overall API functionality. For complete list of what is new and fixed in this month’s release, please visit the Release Notes section of Aspose.Email for .NET documentation.

# Enhancements

**Filtering Tasks from Exchange Server:** Aspose.Email for .NET API already supports fetching tasks from Exchange server. This month’s release further enhances the capabilities of fetching tasks using Exchange Web Service (EWS) by providing filtering capabilities. This allows to retrieve only those tasks from server that meet specific user criterion for task status. The possible statuses include:

*   Completed
*   Deferred
*   In Progress
*   Not Started
*   Waiting on others

The _TaskStatus_ property of _ExchangeQueryBuilder_ class can be used to specify a single status or a combination of statuses to be retrieved from the server as shown in the following code sample:```
 IEWSClient client = EWSClient.GetEWSClient("exchange.domain.com", "username", "password");

ExchangeQueryBuilder queryBuilder = null;
MailQuery query = null;
ExchangeTask fetchedTask = null;
ExchangeMessageInfoCollection messageInfoCol = null;
client.TimezoneId = "Central Europe Standard Time";
Array values = Enum.GetValues(typeof(ExchangeTaskStatus));

//Now retrieve the tasks with specific statuses
foreach (ExchangeTaskStatus status in values)
{
    queryBuilder = new ExchangeQueryBuilder();
    queryBuilder.TaskStatus.Equals(status);
    query = queryBuilder.GetQuery();
    messageInfoCol = client.ListMessages(client.MailboxInfo.TasksUri, query);
    fetchedTask = client.FetchTask(messageInfoCol[0].UniqueUri);
}

//retrieve all other than specified
foreach (ExchangeTaskStatus status in values)
{
    queryBuilder = new ExchangeQueryBuilder();
    queryBuilder.TaskStatus.NotEquals(status);
    query = queryBuilder.GetQuery();
    messageInfoCol = client.ListMessages(client.MailboxInfo.TasksUri, query);
} 
```**Support for Filtering Messages by Date Time:** This month’s release also enhances the API’s IMAP and EWS clients to filter messages from server by Time as well. Till yet, these provided the capability to filter messages from server based on date using the ExchangeQueryBuilder class. The implementation has been enhanced so that the comparison now considers the time part as well. The DateComparisonType.ByDateTime option serves this purpose for filtering messages using the MailQuery.

# Other Improvements

This month’s release also fixes several bugs that were reported with the last month’s release by our valued customers. This further improves the API functionality and stability.

# Worth Noticing

In addition to this month’s release, we have also published a [revamped version][3] of Aspose.Email for .NET that is based on a more improved namespace structure. The new version of the API will be published in parallel to this version, now known as legacy API, for three consecutive release so as to give customers ample time for migration to the new API.

# API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   Product Documentation – Provides detailed examples of working with the API
*   API Reference Guide – Details all the namespaces and classes of the API
*   [GitHub Examples][4] – Provides ready to run API example
*   [Support Forum][5] – Write to us if you have any query or inquiry about the API




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2016/12/Aspose.Email-for-.NET_-1.png
[2]: http://downloads.aspose.com/email/net/new-releases/aspose.email-for-.net-16.12.0---revamped/
[3]: https://blog.aspose.com/2016/12/26/aspose.email-.net-improved-namespace-structure-available-now/
[4]: https://github.com/asposeemail/Aspose_Email_NET
[5]: https://forum.aspose.com/c/email




