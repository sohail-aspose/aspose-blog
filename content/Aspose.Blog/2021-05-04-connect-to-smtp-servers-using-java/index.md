---
title: 'Connect to SMTP Server using Java'
seoTitle: "Connect to SMTP Server in Java | Use SOCKS and HTTP Proxies"
description: "Use email API to connect to the SMTP email servers using Java. Connect to SMTP server using SOCKS or HTTP proxies from within Java applications."
date: Tue, 04 May 2021 11:29:00 +0000
draft: false
url: /2021/05/04/connect-to-smtp-servers-using-java/
author: Usman Aziz
summary: 'The [SMTP][1] is a commonly used email protocol to send emails from the client applications to the email servers. Before communicating with an SMTP server, you need to establish a connection. In this article, you will learn **how to connect to an SMTP server programmatically using Java**. Furthermore, the article will cover how to connect to the SMTP servers via SOCKS or HTTP proxies.'
tags: ['Connect to SMTP Server java', 'Connect to SMTP Server using HTTP Proxy', 'Connect to SMTP Server using SOCKS Proxy']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Connect to SMTP Server using Java">}}


The [SMTP][2] is a commonly used email protocol to send emails from the client applications to the email servers. Before communicating with an SMTP server, you need to establish a connection. In this article, you will learn **how to connect to an SMTP server programmatically using Java**. Furthermore, the article will cover how to connect to the SMTP servers via SOCKS or HTTP proxies.

*   [Java API to Connect to SMTP Server][3]
*   [Connect to an SMTP Server][4]
*   [Use SOCKS Proxy to Connect to SMTP Server][5]
*   [Use HTTP Proxy to Connect to SMTP Server][6]
*   [Get a Free API License][7]

## Java API to Connect to SMTP Server {#Java-API-to-Connect-SMTP-Server}

In order to connect to an SMTP server, we will use [Aspose.Email for Java][8]. It is a powerful API that lets you create feature-rich email client applications using Java. Furthermore, it provides simplified ways to connect to the SMTP servers. You can either [download][9] the API's JAR or install it using the following Maven configurations.

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
    <version>21.3</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Connect to an SMTP Server using Java {#Connect-to-SMTP-Server-using-Java}

The following are the steps to connect to an SMTP server.

*   Create an object of [SmtpClient][10] class and initialize it with the host's address.
*   Set username, password, port, and security options using the _SmtpClient_ object.
*   Send the email.

The following code sample shows how to connect to an SMTP server using Java.

{{< gist aspose-com-gists f43b7488e0a05aad6f2a67c221fdc876 "connect-smtp-server.java" >}}

## Use Proxy to Connect to an SMTP Server {#Use-SOCKS-Proxy-to-Connect-to-SMTP-Server}

In various cases, the SMTP servers are secured using the proxy. Therefore, you have to connect to the SMTP server via the proxy server. For such cases, Aspose.Email for Java provides the following methods.

### Connect to SMTP Servers via SOCKS Proxy in Java {#Use-SOCKS-Proxy-to-Connect-to-SMTP-Server}

Aspose.Email for Java provides the support for versions 4, 4a and 5 of SOCKS proxy protocol. The following are the steps to connect to an SMTP server via SOCKS proxy.

*   Create an object of [SmtpClient][11] class and initialize it with the host, username, and password.
*   Create an object of the [SocksProxy][12] class and set the server's address, port, and SOCKS version.
*   Set proxy using [SmtpClient.setProxy(SocksProxy)][13] method.
*   Send emails.

The following code sample shows how to connect to an SMTP server via SOCKS proxy.

{{< gist aspose-com-gists f43b7488e0a05aad6f2a67c221fdc876 "connect-smtp-server-socks.java" >}}

### Connect to an SMTP Servers via HTTP Proxy in Java {#Connect-to-SMTP-Server-via-HTTP}

The following are the steps to connect to an SMTP server via HTTP proxy.

*   Create an object of the [HttpProxy][14] class and initialize it with the host and port number.
*   Create an object of [SmtpClient][15] class and set host, username, password, and port.
*   Set proxy using [SmtpClient.setProxy(HttpProxy)][16] method.
*   Send emails.

The following code sample shows how to connect to an SMTP server via HTTP proxy.

{{< gist aspose-com-gists f43b7488e0a05aad6f2a67c221fdc876 "connect-smtp-server-http.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [get a free temporary license][17] in order to use Aspose.Email for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to connect to an SMTP server programmatically using Java. In addition, you have seen how to use SOCKS and HTTP proxies to connect to an SMTP server. You can explore more about Aspose.Email for Java using [documentation][18]. Furthermore, you can submit your queries via our [forum][19].

## See Also

*   [Create and Send Outlook Email Messages using Java][20]




[1]: https://en.wikipedia.org/wiki/Simple_Mail_Transfer_Protocol
[2]: https://en.wikipedia.org/wiki/Simple_Mail_Transfer_Protocol
[3]: #Java-API-to-Connect-SMTP-Server
[4]: #Connect-to-SMTP-Server-using-Java
[5]: #Use-SOCKS-Proxy-to-Connect-to-SMTP-Server
[6]: #Connect-to-SMTP-Server-via-HTTP
[7]: #Get-a-Free-API-License
[8]: https://products.aspose.com/email/java
[9]: https://downloads.aspose.com/email/java
[10]: https://apireference.aspose.com/email/java/com.aspose.email/SmtpClient
[11]: https://apireference.aspose.com/email/java/com.aspose.email/SmtpClient
[12]: https://apireference.aspose.com/email/java/com.aspose.email/SocksProxy
[13]: https://apireference.aspose.com/email/java/com.aspose.email/EmailClient#setProxy(com.aspose.email.Proxy)
[14]: https://apireference.aspose.com/email/java/com.aspose.email/HttpProxy
[15]: https://apireference.aspose.com/email/java/com.aspose.email/SmtpClient
[16]: https://apireference.aspose.com/email/java/com.aspose.email/EmailClient#setProxy(com.aspose.email.Proxy)
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/email/java/getting-started/
[19]: https://forum.aspose.com/
[20]: https://blog.aspose.com/2020/05/20/create-and-send-outlook-email-messages-asynchronously-using-java/





