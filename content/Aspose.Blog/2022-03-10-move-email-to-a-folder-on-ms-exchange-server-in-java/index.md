---
title: 'Move Email to a Folder on Microsoft Exchange Server in Java'
date: Thu, 10 Mar 2022 07:51:00 +0000
draft: false
url: /2022/03/10/move-email-to-a-folder-on-ms-exchange-server-in-java/
author: 'Usman Aziz'
summary: '[Aspose.Email for Java](https://products.aspose.com/email/java/) allows you to work with [Microsoft Exchange Server](https://en.wikipedia.org/wiki/Microsoft_Exchange_Server) services such as email, contact management, calendaring, etc. In a [previous post](https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/), you have seen how to read emails from MS Exchange Server programmatically from within your Java applications. However, in certain cases, you may have to move emails from one folder to another on Exchange Server. In this article, you will learn **how to move emails to a particular folder on MS Exchange Server in java**.'
tags: ['Java API to Move Emails on Microsoft Exchange Server', 'Move Existing Email to a Folder on MS Exchange Server', 'Move New Email to a Folder on MS Exchange Server in Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Move Email to a Folder on Microsoft Exchange Server in Java">}}


[Aspose.Email for Java](https://products.aspose.com/email/java/) allows you to work with [Microsoft Exchange Server](https://en.wikipedia.org/wiki/Microsoft_Exchange_Server)'s services such as email, contact management, calendaring, etc. In a [previous post](https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/), you have seen how to read emails from MS Exchange Server programmatically from within your Java applications. However, in certain cases, you may have to move emails from one folder to another on Exchange Server. In this article, you will learn **how to move emails to a particular folder on MS Exchange Server in java**.

*   [Java API to Move Emails on Microsoft Exchange Server](#API-to-Move-Emails-in-Microsoft-Exchange-Server)
*   [Move Existing Email to a Folder on MS Exchange Server](#Move-Existing-Email-to-a-Folder-in-MS-Exchange-Server)
*   [Move New Email to a Folder on MS Exchange Server](#Move-New-Email-to-a-Folder-in-MS-Exchange-Server)

## Java API to Move Emails on Microsoft Exchange Server {#API-to-Move-Emails-in-Microsoft-Exchange-Server}

[Aspose.Email for Java](https://products.aspose.com/email/java/) is a powerful email API to work with MS Exchange Server without writing complex code. In this article, we will use this API to move emails to a specific folder of the mailbox in MS Exchange Server. You can either [download](https://downloads.aspose.com/email/java/) the API or install it using the following Maven configurations.

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

## Move Email to a Folder on MS Exchange Server in Java {#Move-Existing-Email-to-a-Folder-in-MS-Exchange-Server}

The following are the steps to move emails to a particular folder on MS Exchange Server in Java.

*   First, initialize the [IEWSClient](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient) object using username, password, domain, and URI.
*   Then, get list of email messages in an [ExchangeMessageInfoCollection](https://apireference.aspose.com/email/java/com.aspose.email/ExchangeMessageInfoCollection) object using [IEWSClient.listMessages(IEWSClient.getMailboxInfo().getInboxUri())](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#listMessages(java.lang.String)) method.
*   After that, loop through each [ExchangeMessageInfo](https://apireference.aspose.com/email/java/com.aspose.email/ExchangeMessageInfo) message and filter the required one(s).
*   Then, get the URI of the email message to be moved using [ExchangeMessageInfo.getUniqueUri()](https://apireference.aspose.com/email/java/com.aspose.email/ExchangeMessageInfo#getUniqueUri()) method.
*   Finally, move email message using [IEWSClient.copyItem(String URI, IEWSClient.getMailboxInfo().getOutboxUri())](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#copyItem(java.lang.String,%20java.lang.String)) method.

The following code sample shows how to move an email to a folder on MS Exchange Server in Java.

\[gist id="ee4dc729258c1f97c40226b8481f7644" file="move-email.java"\]

## Move New Email to a Folder on MS Exchange Server {#Move-New-Email-to-a-Folder-in-MS-Exchange-Server}

You can also move a newly created email to a particular folder in MS Exchange Server. The following are the steps to perform this operation.

*   First, initialize the [IEWSClient](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient) object using username, password, domain, and URI.
*   Then, create a new message using [MailMessage](https://apireference.aspose.com/email/java/com.aspose.email/MailMessage) class.
*   After that, get the email message's URI returned by [IEWSClient.appendMessage(MailMessage)](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#appendMessage(com.aspose.email.MailMessage)) method.
*   Finally, move email message using [](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#copyItem(java.lang.String,%20java.lang.String))[IEWSClient.copyItem(String URI, IEWSClient.getMailboxInfo().getOutboxUri())](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#copyItem(java.lang.String,%20java.lang.String)) method.

The following code sample shows how to move a new email message to a folder in MS Exchange Server.

\[gist id="ee4dc729258c1f97c40226b8481f7644" file="move-new-email.java"\]

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license](https://purchase.aspose.com/temporary-license) to use Aspose.Email for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to move emails to a particular folder in Microsoft Exchange Server using Java. Furthermore, you have seen how to move a newly created email message to a specific folder in Exchange Server. Besides, you can explore the [documentation](https://docs.aspose.com/email/java/) to read more about Aspose.Email for Java. Also, you can ask your questions via our [forum](https://forum.aspose.com/).

## See Also

*   [Read Emails from MS Exchange Server in Java](https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/)



