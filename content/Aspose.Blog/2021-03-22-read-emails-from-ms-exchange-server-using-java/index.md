---
title: 'Read Emails from MS Exchange Server using Java'
seoTitle: "Java: Read Emails from MS Exchange Server | Using EWS or IMAP"
description: "Read emails from MS Exchange Server from within Java applications. Connect to MS Exchanges Server and read emails using EWS or IMAP."
date: Mon, 22 Mar 2021 05:06:00 +0000
draft: false
url: /2021/03/22/read-emails-from-ms-exchange-server-using-java/
author: Usman Aziz
summary: '[Microsoft Exchange Server][1] is a mail server that provides email, calendaring, contact management, and other collaboration services. It can easily be connected and accessed from within your web or desktop applications. Thus, you can communicate with the Exchange Server and access emails, contacts, calendars, etc. In this article, you will learn **how to connect to MS Exchange Server and read emails using Java**.'
tags: ['Connect Exchange Server via EWS', 'Connect Exchange Server via IMAP', 'Connect to MS Exchange Server in Java', 'Java API to Work with MS Exchange Server', 'Read Emails from MS Exchange Server in Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="">}}


[Microsoft Exchange Server][2] is a mail server that provides email, calendaring, contact management, and other collaboration services. It can easily be connected and accessed from within your web or desktop applications. Thus, you can communicate with the Exchange Server and access emails, contacts, calendars, etc. In this article, you will learn **how to connect to MS Exchange Server and read emails using Java**.

*   [Java API to Work with MS Exchange Server][3]
*   [Connect to MS Exchange Server in Java][4]
    *   [Using EWS][5]
    *   [Using IMAP][6]
*   [Read Emails from MS Exchange Server in Java][7]
    *   [Using EWS][8]
    *   [Using IMAP][9]
*   [Get a Free API License][10]

## Java API to Work with MS Exchange Server {#Java-API-to-Work-with-MS-Exchange-Server}

[Aspose.Email for Java][11] is a powerful API that provides you with a wide range of email management features. It lets you implement feature-rich email clients from within your Java applications. Furthermore, the API allows you to access folders, subfolders, emails, calendars, contacts, etc. from MS Exchange Server. You can either [download][12] the API's JAR or install it using the following Maven configurations.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-email</artifactId>
    <version>21.2</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Connect to MS Exchange Server in Java {#Connect-to-MS-Exchange-Server-in-Java}

In order to work with MS Exchange Server, you need to establish a connection first. Aspose.Email for Java provides the following ways to connect to an Exchange Server.

*   Using Exchange Web Service (EWS)
*   Using Internet Message Access Protocol (IMAP)

### Connect to Exchange Server using EWS {#Connect-Using-EWS}

The following are the steps to connect to Exchange Server via EWS.

*   Create an instance of [IEWSClient][13] class.
*   Use [EWSClient.getEWSClient(String, String, String, String)][14] method to initialize _EWSClient_ object.

The following code sample shows how to connect to MS Exchange Server using EWS in Java.

{{< gist aspose-com-gists b89a7274c26beb2dfba09662ea3244d0 "connect-exchange-server-ews.java" >}}

### Connect to Exchange Server using IMAP {#Connect-Using-IMAP}

Before attempting to connect to Exchange Server using IMAP, please make sure that you have enabled IMAP services. Once done, the following are the steps to connect to an Exchange Server using IMAP.

*   Create an instance of [ImapClient][15] class and initialize it with address, port, username, and password.
*   Access messages, contacts, etc. using the [ImapClient][16] object.

The following code sample shows how to connect to Exchange Sever using IMAP.

{{< gist aspose-com-gists b89a7274c26beb2dfba09662ea3244d0 "connect-exchange-server-imap.java" >}}

## Read Emails from MS Exchange Server in Java {#Read-Emails-from-MS-Exchange-Server-in-Java}

Once you have connected to the Exchange Server, you can read messages from the server. You can do it using EWS or IMAP.

### Read Emails from MS Exchange Server using EWS {#Read-Emails-from-MS-Exchange-Server-EWS}

The following are the steps to read emails from Exchange Server using EWS.

*   Create an instance of [IEWSClient][17] class.
*   Use [EWSClient.getEWSClient(String, String, String, String)][18] method to initialize _EWSClient_ object.
*   Get list of message info from inbox into [ExchangeMessageInfoCollection][19] object using [EWSClient.listMessages(EWSClient.getMailboxInfo().getInboxUri())][20] method.
*   Loop through each [ExchangeMessageInfo][21] object in the collection to read the message.

The following code sample shows how to read messages from Exchange Server via EWS in Java.

{{< gist aspose-com-gists b89a7274c26beb2dfba09662ea3244d0 "read-email-ews.java" >}}

### Read Emails from MS Exchange Server using IMAP {#Read-Emails-from-MS-Exchange-Server-IMAP}

The following are the steps to read emails from Exchange Server using IMAP.

*   Create an instance of [ImapClient][22] class and initialize it with address, port, username, and password.
*   Get the list of message info into [ImapMessageInfoCollection][23] object using [ImapClient.listMessages()][24] method.
*   Loop through each [ImapMessageInfo][25] object in the collection to read the emails.

The following code sample shows how to read emails from Exchange Server via IMAP using Java.

{{< gist aspose-com-gists b89a7274c26beb2dfba09662ea3244d0 "read-email-imap.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try Aspose.Email for Java without evaluation limitations by getting a [temporary license][26].

## Live Demo

*   [Email Viewer][27]

## Conclusion

In this article, you have learned how to connect to MS Exchange Server and read emails using Java. Furthermore, you have seen how to access MS Exchange Server using EWS or IMAP. You can explore more about Aspose.Email for Java using [documentation][28]. In case you would have any questions or queries, feel free to let us know via our [forum][29].

## See Also

*   [Create and Send Outlook Email Messages using Java][30]




[1]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[2]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[3]: #Java-API-to-Work-with-MS-Exchange-Server
[4]: #Connect-to-MS-Exchange-Server-in-Java
[5]: #Connect-Using-EWS
[6]: #Connect-Using-IMAP
[7]: #Read-Emails-from-MS-Exchange-Server-in-Java
[8]: #Read-Emails-from-MS-Exchange-Server-EWS
[9]: #Read-Emails-from-MS-Exchange-Server-IMAP
[10]: #Get-a-Free-API-License
[11]: https://products.aspose.com/email/java
[12]: https://downloads.aspose.com/email/java
[13]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[14]: https://apireference.aspose.com/email/java/com.aspose.email/EWSClient#getEWSClient(java.lang.String,%20java.lang.String,%20java.lang.String,%20java.lang.String)
[15]: https://apireference.aspose.com/email/java/com.aspose.email/ImapClient
[16]: https://apireference.aspose.com/email/java/com.aspose.email/ImapClient
[17]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[18]: https://apireference.aspose.com/email/java/com.aspose.email/EWSClient#getEWSClient(java.lang.String,%20java.lang.String,%20java.lang.String,%20java.lang.String)
[19]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeMessageInfoCollection
[20]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#listMessages(java.lang.String)
[21]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeMessageInfo
[22]: https://apireference.aspose.com/email/java/com.aspose.email/ImapClient
[23]: https://apireference.aspose.com/email/java/com.aspose.email/ImapMessageInfoCollection
[24]: https://apireference.aspose.com/email/java/com.aspose.email/ImapClient#listMessages()
[25]: https://apireference.aspose.com/email/java/com.aspose.email/ImapMessageInfo
[26]: https://purchase.aspose.com/temporary-license
[27]: http://products.aspose.app/email/viewer
[28]: https://docs.aspose.com/email/java/getting-started/
[29]: https://forum.aspose.com/
[30]: https://blog.aspose.com/2020/05/20/create-and-send-outlook-email-messages-asynchronously-using-java/





