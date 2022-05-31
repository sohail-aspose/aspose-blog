---
title: 'Connect to POP3 Servers in Java'
date: Fri, 13 May 2022 05:40:08 +0000
draft: false
url: /2022/05/13/connect-to-pop3-servers-in-java/
author: ''Usman Aziz''
summary: '[Post Office Protocol][1] (POP3) is an email protocol that is used to fetch emails from the mailing servers. While implementing email clients and working with POP3 servers, you will first need to establish a connection to access the mailbox. To achieve this, in this article, you will learn **how to connect to POP3 servers in Java**.'
tags: ['Connect to a POP3 Server using Java', 'Connect to a POP3 Server via HTTP Proxy in Java', 'Connect to a POP3 Server via SOCKS Proxy in Java', 'Java API to Connect POP3 Servers']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Fetch-Emails-from-POP3-Servers.png" alt="Connect to POP3 Servers in Java">}}


[Post Office Protocol][2] (POP3) is an email protocol that is used to fetch emails from the mailing servers. While implementing email clients and working with POP3 servers, you will first need to establish a connection to access the mailbox. To achieve this, in this article, you will learn **how to connect to POP3 servers in Java**.

*   [Java API to Connect POP3 Servers][3]
*   [Connect to a POP3 Server using Java][4]
*   [Connect to a POP3 Server via Proxy][5]
    *   [Access POP3 Server via SOCKS][6]
    *   [Access POP3 Server via HTTP][7]

## Java API to Connect POP3 Servers {#API-to-Connect-POP3-Server}

[Aspose.Email for Java][8] is an amazing API that allows you to create feature-rich email client applications. The API lets you create and send emails as well as retrieve messages from POP3 servers. We will use this API to connect to the POP3 servers and access the mailbox. You can either [download][9] the API or install it using the following Maven configurations.

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
    <version>22.4</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Connect to a POP3 Server in Java {#Connect-to-a-POP3-Server}

In order to connect to a POP3 server, Aspose.Email for Java provides [Pop3Client][10] class. The following are the steps to connect to a POP3 server.

*   Create an instance of the [Pop3Client][11] class.
*   Specify the host, username, and password using the _Pop3Client_ instance.
*   Access the mailbox.

The following code sample shows how to connect to a POP3 server in Java.

{{< gist aspose-com-gists 7c5b8a4ddb79171f1b12ab6a777674d7 "connect-pop3-server.java" >}}

## Connect to POP3 Server via Proxy {#Connect-to-POP3-Server-via-Proxy}

In various cases, you have to access the email servers via a proxy. Currently, Aspose.Email for Java supports connecting to a POP3 server via SOCKS or HTTP proxy.

### Connecting POP3 Server via SOCKS Proxy {#Access-POP3-Server-via-SOCKS}

The following are the steps to connect to a POP3 server via SOCKS proxy.

*   Create a [SocksProxy][12] object and set the address, port, and SOCKS version.
*   Create an instance of the [Pop3Client][13] class and set address, username, password, and other settings.
*   Set proxy to _SocksProxy_ object using [Pop3Client.setProxy()][14] method.
*   Access mailbox.

The following code sample shows how to connect to the POP3 server via SOCKS proxy in Java.

{{< gist aspose-com-gists 7c5b8a4ddb79171f1b12ab6a777674d7 "connect-pop3-server-socks.java" >}}

### Connecting POP3 Server via HTTP Proxy {#Access-POP3-Server-via-HTTP}

The following are the steps to connect to a POP3 server via HTTP proxy.

*   Create an [HttpProxy][15] object and set address, username, and password.
*   Create an instance of the [Pop3Client][16] class and set address, username, password, and other settings.
*   Set proxy to _HttpProxy_ object using [Pop3Client.setProxy()][17] method.
*   Access mailbox.

The following code sample shows how to connect to a POP3 server via HTTP proxy in Java.

{{< gist aspose-com-gists 7c5b8a4ddb79171f1b12ab6a777674d7 "connect-pop3-server-http.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try Aspose.Email for Java for free by [getting a temporary license][18].

## Conclusion

In this article, you have learned how to connect to the POP3 servers in Java. Furthermore, you have seen how to connect to a server via SOCKS or HTTP proxy. In addition, you can explore other features of Aspose.Email for Java using [documentation][19]. In case you would have any questions or queries, you can contact us via our [forum][20].

## See Also

*   [Read Emails from MS Exchange Server using Java][21]
*   [Create and Send Outlook Email Messages using Java][22]




[1]: https://en.wikipedia.org/wiki/Post_Office_Protocol
[2]: https://en.wikipedia.org/wiki/Post_Office_Protocol
[3]: #API-to-Connect-POP3-Server
[4]: #Connect-to-a-POP3-Server
[5]: #Connect-to-POP3-Server-via-Proxy
[6]: #Access-POP3-Server-via-SOCKS
[7]: #Access-POP3-Server-via-HTTP
[8]: https://products.aspose.com/email/java/
[9]: https://downloads.aspose.com/email/java/
[10]: https://apireference.aspose.com/email/java/com.aspose.email/Pop3Client
[11]: https://apireference.aspose.com/email/java/com.aspose.email/Pop3Client
[12]: https://apireference.aspose.com/email/java/com.aspose.email/SocksProxy
[13]: https://apireference.aspose.com/email/java/com.aspose.email/Pop3Client
[14]: https://apireference.aspose.com/email/java/com.aspose.email/EmailClient#setProxy(com.aspose.email.Proxy)
[15]: https://apireference.aspose.com/email/java/com.aspose.email/HttpProxy
[16]: https://apireference.aspose.com/email/java/com.aspose.email/Pop3Client
[17]: https://apireference.aspose.com/email/java/com.aspose.email/EmailClient#setProxy(com.aspose.email.Proxy)
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/email/java/
[20]: https://forum.aspose.com/
[21]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/
[22]: https://blog.aspose.com/2020/05/20/create-and-send-outlook-email-messages-asynchronously-using-java/




