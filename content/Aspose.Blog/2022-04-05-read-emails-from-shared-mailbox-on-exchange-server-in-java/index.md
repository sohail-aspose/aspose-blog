---
title: 'Read Emails from Shared Mailbox on Exchange Server in Java'
seoTitle: "Java Read Emails from Shared Mailbox in MS Exchange Server | EWS API"
description: "Use Java EWS API to read emails from shared mailbox on Microsoft Exchange Server programmatically using Java. Retrieve messages with EWS client."
date: Tue, 05 Apr 2022 04:47:00 +0000
draft: false
url: /2022/04/05/read-emails-from-shared-mailbox-on-exchange-server-in-java/
author: Usman Aziz
summary: '[Microsoft Exchange Server][1] provides the facility of a shared mailbox that can be accessed by multiple users. The users can send or receive emails, create calendars and tasks, and perform other activities. While working with MS Exchange Server programmatically, you may need to access emails from a shared mailbox. Therefore, in this article, you will learn **how to read email messages from a shared mailbox on MS Exchange Server using Java**.'
tags: ['Java API to Read Emails from Shared Mailbox', 'Java EWS API', 'Read Emails from a Shared Mailbox in Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="">}}


[Microsoft Exchange Server][2] provides the facility of a shared mailbox that can be accessed by multiple users. The users can send or receive emails, create calendars and tasks, and perform other activities. While working with MS Exchange Server programmatically, you may need to access emails from a shared mailbox. Therefore, in this article, you will learn **how to read email messages from a shared mailbox on MS Exchange Server using Java**.

*   [Java API to Read Emails from Shared Mailbox][3]
*   [Read Emails from a Shared Mailbox][4]

## Java API to Read Emails from Shared Mailbox on Exchange Server {#API-to-Create-Folders-in-MS-Exchange-Server}

To read the messages from a shared mailbox on MS Exchange Server, we will use [Aspose.Email for Java][5]. The API provides a bunch of features to connect to and work with MS Exchange Server from within the Java applications. You can either [download][6] the API or install it using the following Maven configurations.

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
*   Connect to Exchange Server and get the instance of the EWS client into an [IEWSClient][7] object.
*   Get emails into an array from the desired folder using [IEWSClient.listItems(String, String)][8] method.
*   Loop through each email in the array and perform the following steps:
    *   Fetch each message into a [MapiMessage][9] object using [IEWSClient.fetchItem(String)][10] method.
    *   Read message's details using _MapiMessage_ object such as [MapiMessage.getSubject()][11] method.

The following code sample shows how to read email messages from a shared mailbox on MS Exchange Server in Java.

{{< gist aspose-com-gists 8d8bb9d85c39778451f702fc5f12f454 "read-emails-from-shared-mailbox.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][12] to use Aspose.Email for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to read email messages from a shared mailbox on Microsoft Exchange Server in Java. You can simply install the API and integrate the provided code sample to access the shared mailboxes from within your Java applications. Besides, you can learn more about Aspose.Email for Java from the [documentation][13]. Also, in case you would have any question, you can ask us via our [forum][14].

## See Also

*   [Read Emails from MS Exchange Server in Java][15]




[1]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[2]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[3]: #API-to-Create-Folders-in-MS-Exchange-Server
[4]: #Read-Emails-from-a-Shared-Mailbox
[5]: https://products.aspose.com/email/java/
[6]: https://downloads.aspose.com/email/java/
[7]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[8]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#listItems(java.lang.String,%20java.lang.String)
[9]: https://apireference.aspose.com/email/java/com.aspose.email/MapiMessage
[10]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#fetchItem(java.lang.String)
[11]: https://apireference.aspose.com/email/java/com.aspose.email/MapiMessageItemBase#getSubject()
[12]: https://purchase.aspose.com/temporary-license
[13]: https://docs.aspose.com/email/java/
[14]: https://forum.aspose.com/
[15]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/




