---
title: 'Connect to an IMAP Server using Java'
seoTitle: "Connect to IMAP Server using Java | Aspose.Email for Java"
description: "Use Java Email API to connect to the IMAP server from within your Java applications. Connect IMAP server via SOCKS or HTTP proxies."
date: Thu, 08 Jul 2021 11:26:00 +0000
draft: false
url: /2021/07/08/connect-to-an-imap-server-using-java/
author: Usman Aziz
summary: '[Internet Message Access Protocol][1] (IMAP) is a commonly used protocol for retrieving messages from the email servers. In order to access the mailbox from your client applications, you would first need to establish a connection with the IMAP server. To achieve this, this article covers**how to connect to an IMAP server using Java.** Furthermore, you will learn how to use SOCKS or HTTP proxy and connect to an SSL-enabled IMAP server programmatically.'
tags: ['Connect to IMAP Server in Java', 'Java API to Connect IMAP Servers', 'Java Access IMAP Server via HTTP Proxy', 'Java Connect to IMAP Server via SOCKS Proxy', 'Java Connect to SSL Enabled IMAP Server']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Connect-Email-Server.jpg" alt="Connect to IMAP Server using Java">}}


[Internet Message Access Protocol][2] (IMAP) is a commonly used protocol for retrieving messages from the email servers. In order to access the mailbox from your client applications, you would first need to establish a connection with the IMAP server. To achieve this, this article covers**how to connect to an IMAP server using Java.** Furthermore, you will learn how to use SOCKS or HTTP proxy and connect to an SSL-enabled IMAP server programmatically.

*   [Java API to Connect IMAP Servers][3]
*   [Connect to IMAP Server in Java][4]
*   [Connect to IMAP Server via SOCKS Proxy][5]
*   [Access IMAP Server via HTTP Proxy][6]
*   [Connect to SSL Enabled IMAP Server][7]

## Java API to Connect an IMAP Server {#Java-API-to-Connect-IMAP-Servers}

In order to connect to the IMAP servers, we will use [Aspose.Email for Java][8]. It is a powerful API that lets you implement feature-rich email clients from within your Java applications. You can either [download][9] the API or install it using the following Maven configurations.

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
    <version>21.6</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Connect to an IMAP Server in Java {#Connect-to-IMAP-Server-in-Java}

The following are the steps to connect to an IMAP server using Java.

1.  Create an instance of [ImapClient][10] class and set the host, username and password.
2.  Use the ImapClient object to access the mailbox, i.e. using [ImapClient.selectFolder("Inbox")][11] method.

The following code sample shows how to connect to an IMAP server.

{{< gist aspose-com-gists 01831893169b346cc3bd4c142c1508b3 "connect-imap.java" >}}

## Connect to IMAP Servers via Proxy

In certain cases, the email servers are not accessible directly and you have to use a proxy. Aspose.Email for Java supports SOCKS and HTTP proxies to connect to an IMAP server. The following sections demonstrate how to establish a connection via a proxy.

### Connect to an IMAP Server via SOCKS Proxy {#Connect-to-IMAP-Server-via-SOCKS-Proxy}

The following are the steps to connect to an IMAP server via SOCKS proxy.

1.  Create an instance of [ImapClient][12] class and specify the host, username and password.
2.  Create an instance of [SocksProxy][13] class and specify proxy address, port, and version.
3.  Set proxy using [ImapClient.setProxy(SocksProxy)][14] method.
4.  Use the ImapClient object to access the mail box, i.e. using [ImapClient.selectFolder("Inbox")][15] method.

The following code sample shows how to connect to the IMAP servers via SOCKS proxy in Java.

{{< gist aspose-com-gists 01831893169b346cc3bd4c142c1508b3 "connect-imap-socks.java" >}}

### Connect to an IMAP Server via HTTP Proxy {#Access-IMAP-Server-via-HTTP-Proxy}

The following are the steps to connect to an IMAP server via HTTP proxy in Java.

1.  Create an instance of [ImapClient][16] class and specify the host, username and password.
2.  Create an instance of [HttpProxy][17] class and specify address and port.
3.  Set proxy using [ImapClient.setProxy(HttpProxy)][18] method.
4.  Use the ImapClient object to access the mailbox, i.e. using [ImapClient.selectFolder("Inbox")][19] method.

The following code sample shows how to access IMAP servers via HTTP proxy in Java.

{{< gist aspose-com-gists 01831893169b346cc3bd4c142c1508b3 "connect-imap-http.java" >}}

## Connect to SSL-enabled IMAP Servers in Java {#Connect-to-SSL-Enabled-IMAP-Server}

Aspose.Email for Java also allows connecting SSL-enabled IMAP servers. In that case, you need to set the [SecurityOptions.SSLImplicit][20] security option of the ImapClient using [ImapClient.setSecurityOptions()][21] method.

The following code sample shows how to connect to an SSL-enabled IMAP server.

{{< gist aspose-com-gists 01831893169b346cc3bd4c142c1508b3 "connect-imap-ssl.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Email for Java for free by [getting a temporary license][22].

## Conclusion

In this article, you have learned how to connect to an IMAP server using Java. Furthermore, the step-by-step guide and code samples have demonstrated how to connect to an IMAP server via SOCKS or HTTP proxy. You can explore more about the API using [documentation][23]. For any questions or queries, feel free to let us know via our [forum][24].

## See Also

*   [Read Emails from MS Exchange Server using Java][25]
*   [Create and Send Outlook Email Messages using Java][26]




[1]: https://en.wikipedia.org/wiki/Internet_Message_Access_Protocol
[2]: https://en.wikipedia.org/wiki/Internet_Message_Access_Protocol
[3]: #Java-API-to-Connect-IMAP-Servers
[4]: #Connect-to-IMAP-Server-in-Java
[5]: #Connect-to-IMAP-Server-via-SOCKS-Proxy
[6]: #Access-IMAP-Server-via-HTTP-Proxy
[7]: #Connect-to-SSL-Enabled-IMAP-Server
[8]: https://products.aspose.com/email/java
[9]: https://downloads.aspose.com/email/java
[10]: https://apireference.aspose.com/email/java/com.aspose.email/ImapClient
[11]: https://apireference.aspose.com/email/java/com.aspose.email/ImapClient#selectFolder(java.lang.String)
[12]: https://apireference.aspose.com/email/java/com.aspose.email/ImapClient
[13]: https://apireference.aspose.com/email/java/com.aspose.email/SocksProxy
[14]: https://apireference.aspose.com/email/java/com.aspose.email/EmailClient#setProxy(com.aspose.email.Proxy)
[15]: https://apireference.aspose.com/email/java/com.aspose.email/ImapClient#selectFolder(java.lang.String)
[16]: https://apireference.aspose.com/email/java/com.aspose.email/ImapClient
[17]: https://apireference.aspose.com/email/java/com.aspose.email/HttpProxy
[18]: https://apireference.aspose.com/email/java/com.aspose.email/EmailClient#setProxy(com.aspose.email.Proxy)
[19]: https://apireference.aspose.com/email/java/com.aspose.email/ImapClient#selectFolder(java.lang.String)
[20]: https://apireference.aspose.com/email/java/com.aspose.email/SecurityOptions#SSLImplicit
[21]: https://apireference.aspose.com/email/java/com.aspose.email/EmailClient#setSecurityOptions(int)
[22]: https://purchase.aspose.com/temporary-license
[23]: https://docs.aspose.com/email/java
[24]: https://forum.aspose.com/
[25]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/
[26]: https://blog.aspose.com/2020/05/20/create-and-send-outlook-email-messages-asynchronously-using-java/





