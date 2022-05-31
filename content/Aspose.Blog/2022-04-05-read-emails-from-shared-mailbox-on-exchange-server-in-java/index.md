---
title: 'Read Emails from Shared Mailbox on Exchange Server in Java'
date: Tue, 05 Apr 2022 04:47:00 +0000
draft: false
url: /2022/04/05/read-emails-from-shared-mailbox-on-exchange-server-in-java/
author: 'Usman Aziz'
summary: '[Microsoft Exchange Server](https://en.wikipedia.org/wiki/Microsoft_Exchange_Server) provides the facility of a shared mailbox that can be accessed by multiple users. The users can send or receive emails, create calendars and tasks, and perform other activities. While working with MS Exchange Server programmatically, you may need to access emails from a shared mailbox. Therefore, in this article, you will learn **how to read email messages from a shared mailbox on MS Exchange Server using Java**.'
tags: ['Java API to Read Emails from Shared Mailbox', 'Java EWS API', 'Read Emails from a Shared Mailbox in Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="">}}


[Microsoft Exchange Server](https://en.wikipedia.org/wiki/Microsoft_Exchange_Server) provides the facility of a shared mailbox that can be accessed by multiple users. The users can send or receive emails, create calendars and tasks, and perform other activities. While working with MS Exchange Server programmatically, you may need to access emails from a shared mailbox. Therefore, in this article, you will learn **how to read email messages from a shared mailbox on MS Exchange Server using Java**.

*   [Java API to Read Emails from Shared Mailbox](#API-to-Create-Folders-in-MS-Exchange-Server)
*   [Read Emails from a Shared Mailbox](#Read-Emails-from-a-Shared-Mailbox)

## Java API to Read Emails from Shared Mailbox on Exchange Server {#API-to-Create-Folders-in-MS-Exchange-Server}

To read the messages from a shared mailbox on MS Exchange Server, we will use [Aspose.Email for Java](https://products.aspose.com/email/java/). The API provides a bunch of features to connect to and work with MS Exchange Server from within the Java applications. You can either [download](https://downloads.aspose.com/email/java/) the API or install it using the following Maven configurations.

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
    <version>22.2</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Read Emails from a Shared Mailbox on Exchange Server in Java {#Read-Emails-from-a-Shared-Mailbox}

The following are the steps to read emails from a shared mailbox on MS Exchange Server with an EWS client in Java.

*   Setup the network credentials.
*   Connect to Exchange Server and get the instance of the EWS client into an [IEWSClient](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient) object.
*   Get emails into an array from the desired folder using [IEWSClient.listItems(String, String)](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#listItems(java.lang.String,%20java.lang.String)) method.
*   Loop through each email in the array and perform the following steps:
    *   Fetch each message into a [MapiMessage](https://apireference.aspose.com/email/java/com.aspose.email/MapiMessage) object using [IEWSClient.fetchItem(String)](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#fetchItem(java.lang.String)) method.
    *   Read message's details using _MapiMessage_ object such as [MapiMessage.getSubject()](https://apireference.aspose.com/email/java/com.aspose.email/MapiMessageItemBase#getSubject()) method.

The following code sample shows how to read email messages from a shared mailbox on MS Exchange Server in Java.

\[gist id="8d8bb9d85c39778451f702fc5f12f454" file="read-emails-from-shared-mailbox.java"\]

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license](https://purchase.aspose.com/temporary-license) to use Aspose.Email for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to read email messages from a shared mailbox on Microsoft Exchange Server in Java. You can simply install the API and integrate the provided code sample to access the shared mailboxes from within your Java applications. Besides, you can learn more about Aspose.Email for Java from the [documentation](https://docs.aspose.com/email/java/). Also, in case you would have any question, you can ask us via our [forum](https://forum.aspose.com/).

## See Also

*   [Read Emails from MS Exchange Server in Java](https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/)



