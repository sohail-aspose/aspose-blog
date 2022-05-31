---
title: 'Create, Update or Delete Tasks on MS Exchange Server in Java'
date: Fri, 11 Mar 2022 13:14:00 +0000
draft: false
url: /2022/03/11/create-update-or-delete-tasks-on-ms-exchange-server-in-java/
author: 'Usman Aziz'
summary: 'To-do lists are used to keep track of the activities to be performed. People create such lists on paper, text editors, spreadsheets, etc. [Microsoft Exchange Server][1] also provides the feature of creating and managing to-do lists that are composed of tasks. To work with these tasks programmatically, this article shows **how to add, update, or delete tasks on MS Exchange Server in Java**.'
tags: ['Create a Task on MS Exchange Server in Java', 'Delete a Task on MS Exchange Server in Java', 'Java API to Manage Tasks on MS Exchange Server', 'Java EWS API', 'Update a Task on MS Exchange Server in Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Create, Update or Delete Tasks on MS Exchange Server in Java">}}


To-do lists are used to keep track of the activities to be performed. People create such lists on paper, text editors, spreadsheets, etc. [Microsoft Exchange Server][2] also provides the feature of creating and managing to-do lists that are composed of tasks. To work with these tasks programmatically, this article shows **how to add, update, or delete tasks on MS Exchange Server in Java**.

*   [API to Manage Tasks on MS Exchange Server][3]
*   [Create a Task on MS Exchange Server in Java][4]
*   [Update a Task on MS Exchange Server in Java][5]
*   [Delete a Task on MS Exchange Server in Java][6]

## Java API to Manage Tasks on MS Exchange Server {#API-to-Manage-Tasks-on-MS-Exchange}

[Aspose.Email for Java][7] is an email processing API that is used to create and send emails and implement email client applications. In addition, it allows you to work with MS Exchange Server seamlessly. We will use this API to create and manipulate tasks on MS Exchange Server. You can either [download][8] the API or install it using the following Maven configurations.

```
**Repository:**
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>

**Dependency:** 
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-email</artifactId>
    <version>22.3</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Create a Task on MS Exchange Server in Java {#Create-Task-on-MS-Exchange-Server}

The following are the steps to create tasks on MS Exchange Server in Java.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient][9] object.
*   Then, create an instance of [ExchangeTask][10] class.
*   Set properties of tasks such as subject, status, etc.
*   Finally, create the task using [IEWSClient.createTask(String, ExchangeTask)][11] method.

The following code sample shows how to create tasks on MS Exchange Server using Java.

{{< gist aspose-com-gists f17a81214b8e111869e19ac9bc3188d6 "create-task.java" >}}

## Update Task on MS Exchange Server in Java {#Update-Task-on-MS-Exchange-Server}

You can also access and update the existing tasks on MS Exchange Server programmatically using Java. The following are the steps to perform this operation.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient][12] object.
*   Then, get lists of tasks into an [ExchangeMessageInfoCollection][13] object using [IEWSClient.listMessages(String)][14] method.
*   Loop through each [ExchangeMessageInfo][15] in the collection.
*   Fetch each [ExchangeTask][16] using [IEWSClient.fetchTask(String)][17] method and filter the required one(s).
*   Finally, edit properties and update the task using [IEWSClient.updateTask(ExchangeTask)][18] method.

The following code sample shows how to update a task on MS Exchange Server in Java.

{{< gist aspose-com-gists f17a81214b8e111869e19ac9bc3188d6 "update-task.java" >}}

## Delete Tasks on MS Exchange Server in Java {#Delete-Task-on-MS-Exchange-Server}

The following are the steps to delete tasks on MS Exchange Server in Java.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient][19] object.
*   Then, get lists of tasks into an [ExchangeMessageInfoCollection][20] object using [IEWSClient.listMessages(String)][21] method.
*   Loop through each [ExchangeMessageInfo][22] in the collection.
*   Fetch each [ExchangeTask][23] using [IEWSClient.fetchTask(String)][24] method and filter the required one(s).
*   Finally, delete the task using [IEWSClient.deleteItem(String, DeletionOptions)][25] method.

The following code sample shows how to delete tasks from MS Exchange Server in Java.

{{< gist aspose-com-gists f17a81214b8e111869e19ac9bc3188d6 "delete-task.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][26] to use Aspose.Email for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to manage tasks on Microsoft Exchange Server. Particularly, you have seen how to add, update, or delete tasks on MS Exchange Server programmatically in Java. Alongside, you can explore the [documentation][27] to read more about Aspose.Email for Java. Also, you can ask your questions via our [forum][28].

## See Also

*   [Read Emails from MS Exchange Server in Java][29]




[1]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[2]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[3]: #API-to-Manage-Tasks-on-MS-Exchange
[4]: #Create-Task-on-MS-Exchange-Server
[5]: #Update-Task-on-MS-Exchange-Server
[6]: #Delete-Task-on-MS-Exchange-Server
[7]: https://products.aspose.com/email/java/
[8]: https://downloads.aspose.com/email/java/
[9]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[10]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeTask
[11]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#createTask(java.lang.String,%20com.aspose.email.ExchangeTask)
[12]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[13]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeMessageInfoCollection
[14]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#listMessages(java.lang.String)
[15]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeMessageInfo
[16]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeTask
[17]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#fetchTask(java.lang.String)
[18]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#updateTask(com.aspose.email.ExchangeTask)
[19]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[20]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeMessageInfoCollection
[21]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#listMessages(java.lang.String)
[22]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeMessageInfo
[23]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeTask
[24]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#fetchTask(java.lang.String)
[25]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#deleteItem(java.lang.String,%20com.aspose.email.DeletionOptions)
[26]: https://purchase.aspose.com/temporary-license
[27]: https://docs.aspose.com/email/java/
[28]: https://forum.aspose.com/
[29]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/




