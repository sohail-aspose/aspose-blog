---
title: 'Move Email to a Folder on Microsoft Exchange Server in Java'
seoTitle: "Java Move Email to a Folder in MS Exchange Server | Java Email API"
description: "Use Java API to move emails to a particular folder in MS Exchange Server in Java. Move newly created email messages to a specific folder in Exchange Server."
date: Thu, 10 Mar 2022 07:51:00 +0000
draft: false
url: /2022/03/10/move-email-to-a-folder-on-ms-exchange-server-in-java/
author: Usman Aziz
summary: '[Aspose.Email for Java][1] allows you to work with [Microsoft Exchange Server][2] services such as email, contact management, calendaring, etc. In a [previous post][3], you have seen how to read emails from MS Exchange Server programmatically from within your Java applications. However, in certain cases, you may have to move emails from one folder to another on Exchange Server. In this article, you will learn **how to move emails to a particular folder on MS Exchange Server in java**.'
tags: ['Java API to Move Emails on Microsoft Exchange Server', 'Move Existing Email to a Folder on MS Exchange Server', 'Move New Email to a Folder on MS Exchange Server in Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Move Email to a Folder on Microsoft Exchange Server in Java">}}


[Aspose.Email for Java][4] allows you to work with [Microsoft Exchange Server][5]'s services such as email, contact management, calendaring, etc. In a [previous post][6], you have seen how to read emails from MS Exchange Server programmatically from within your Java applications. However, in certain cases, you may have to move emails from one folder to another on Exchange Server. In this article, you will learn **how to move emails to a particular folder on MS Exchange Server in java**.

*   [Java API to Move Emails on Microsoft Exchange Server][7]
*   [Move Existing Email to a Folder on MS Exchange Server][8]
*   [Move New Email to a Folder on MS Exchange Server][9]

## Java API to Move Emails on Microsoft Exchange Server {#API-to-Move-Emails-in-Microsoft-Exchange-Server}

[Aspose.Email for Java][10] is a powerful email API to work with MS Exchange Server without writing complex code. In this article, we will use this API to move emails to a specific folder of the mailbox in MS Exchange Server. You can either [download][11] the API or install it using the following Maven configurations.

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

*   First, initialize the [IEWSClient][12] object using username, password, domain, and URI.
*   Then, get list of email messages in an [ExchangeMessageInfoCollection][13] object using [IEWSClient.listMessages(IEWSClient.getMailboxInfo().getInboxUri())][14] method.
*   After that, loop through each [ExchangeMessageInfo][15] message and filter the required one(s).
*   Then, get the URI of the email message to be moved using [ExchangeMessageInfo.getUniqueUri()][16] method.
*   Finally, move email message using [IEWSClient.copyItem(String URI, IEWSClient.getMailboxInfo().getOutboxUri())][17] method.

The following code sample shows how to move an email to a folder on MS Exchange Server in Java.

{{< gist aspose-com-gists ee4dc729258c1f97c40226b8481f7644 "move-email.java" >}}

## Move New Email to a Folder on MS Exchange Server {#Move-New-Email-to-a-Folder-in-MS-Exchange-Server}

You can also move a newly created email to a particular folder in MS Exchange Server. The following are the steps to perform this operation.

*   First, initialize the [IEWSClient][18] object using username, password, domain, and URI.
*   Then, create a new message using [MailMessage][19] class.
*   After that, get the email message's URI returned by [IEWSClient.appendMessage(MailMessage)][20] method.
*   Finally, move email message using [](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#copyItem(java.lang.String,%20java.lang.String))[IEWSClient.copyItem(String URI, IEWSClient.getMailboxInfo().getOutboxUri())][21] method.

The following code sample shows how to move a new email message to a folder in MS Exchange Server.

{{< gist aspose-com-gists ee4dc729258c1f97c40226b8481f7644 "move-new-email.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][22] to use Aspose.Email for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to move emails to a particular folder in Microsoft Exchange Server using Java. Furthermore, you have seen how to move a newly created email message to a specific folder in Exchange Server. Besides, you can explore the [documentation][23] to read more about Aspose.Email for Java. Also, you can ask your questions via our [forum][24].

## See Also

*   [Read Emails from MS Exchange Server in Java][25]




[1]: https://products.aspose.com/email/java/
[2]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[3]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/
[4]: https://products.aspose.com/email/java/
[5]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[6]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/
[7]: #API-to-Move-Emails-in-Microsoft-Exchange-Server
[8]: #Move-Existing-Email-to-a-Folder-in-MS-Exchange-Server
[9]: #Move-New-Email-to-a-Folder-in-MS-Exchange-Server
[10]: https://products.aspose.com/email/java/
[11]: https://downloads.aspose.com/email/java/
[12]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[13]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeMessageInfoCollection
[14]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#listMessages(java.lang.String)
[15]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeMessageInfo
[16]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeMessageInfo#getUniqueUri()
[17]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#copyItem(java.lang.String,%20java.lang.String)
[18]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[19]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage
[20]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#appendMessage(com.aspose.email.MailMessage)
[21]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#copyItem(java.lang.String,%20java.lang.String)
[22]: https://purchase.aspose.com/temporary-license
[23]: https://docs.aspose.com/email/java/
[24]: https://forum.aspose.com/
[25]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/




