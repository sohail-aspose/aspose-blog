---
title: 'Connect to POP3 Servers using C#'
seoTitle: "Connect POP3 Server in C# | Connect via SOCKS or HTTP Proxy | SSL"
description: "Use .NET Email API to connect to POP3 server using C#. Connect to the SSL-enabled POP3 server or connect via SOCKS or HTTP proxy servers."
date: Fri, 19 Mar 2021 13:35:00 +0000
draft: false
url: /2021/03/19/connect-to-pop3-servers-in-csharp/
author: Usman Aziz
summary: '[Post Office Protocol][1] (POP3) is an email protocol that is used to fetch emails from the mailing servers. While implementing email clients and working with POP3 servers, you will first need to establish a connection to access the mailbox. To achieve this, in this article, you will learn **how to connect to POP3 servers using C#** from within your .NET applications.'
tags: ['Connect to SSL enabled POP3 Server via Proxy', 'Connect to a POP3 Server using Csharp', 'Connect to a POP3 Server via Proxy', 'Csharp API to Connect POP3 Servers']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="connect POP3 server in C#">}}


[Post Office Protocol][2] (POP3) is an email protocol that is used to fetch emails from the mailing servers. While implementing email clients and working with POP3 servers, you will first need to establish a connection to access the mailbox. To achieve this, in this article, you will learn **how to connect to POP3 servers using C#** from within your .NET applications.

*   [C# API to Connect POP3 Servers][3]
*   [Connect to a POP3 Server using C#][4]
*   [Connect to a POP3 Server via Proxy][5]
*   [Establish Connection to SSL Enabled POP3 Server][6]
*   [Get a Free API License][7]

## C# API to Connect POP3 Servers {#API-to-Connect-POP3-Server}

[Aspose.Email for .NET][8] is a powerful API that allows you to create feature-rich email client applications. The API lets you create and send emails as well as retrieve messages from POP3 servers. You can either [download][9] the API or install it using [NuGet][10].

```
PM> Install-Package Aspose.Email
```

## Connect to a POP3 Server using C# {#Connect-to-a-POP3-Server-using-csharp}

In order to connect to a POP3 server, Aspose.Email for .NET provides [Pop3Client][11] class. The following are the steps to connect to a POP3 server.

*   Create an instance of the [Pop3Client][12] class.
*   Specify the host, username, and password using the [Pop3Client][13] instance.
*   Access the mailbox.

The following code sample shows how to connect to a POP3 server using C#.

{{< gist aspose-com-gists 141797c6552408d82eec15a0c9faa33a "connect-pop3.cs" >}}

## Connect to POP3 Server via Proxy {#Connect-to-POP3-Server-via-Proxy}

In various cases, you have to access the email servers via a proxy. Currently, Aspose.Email for .NET supports connecting to a POP3 server via SOCKS or HTTP proxy.

### Connecting POP3 Server via SOCKS Proxy

The following are the steps to connect to a POP3 server via SOCKS proxy.

*   Create a [SocksProxy][14] object and set address, port, and SOCKS version.
*   Create an instance of the [Pop3Client][15] class and set address, username, password, and other settings.
*   Set the [Pop3Client.Proxy][16] property to the [SocksProxy][17] object.
*   Access mailbox.

The following code sample shows how to connect to POP3 server via SOCKS proxy in C#.

{{< gist aspose-com-gists 141797c6552408d82eec15a0c9faa33a "connect-pop3-socks.cs" >}}

### Connecting POP3 Server via HTTP Proxy

The following are the steps to connect to a POP3 server via HTTP proxy.

*   Create an [HttpProxy][18] object and set address, username, and password.
*   Create an instance of the [Pop3Client][19] class and set address, username, password, and other settings.
*   Set the [Pop3Client.Proxy][20] property to the [HttpProxy][21] object.
*   Access mailbox.

The following code sample shows how to connect to a POP3 server via HTTP proxy in C#.

{{< gist aspose-com-gists 141797c6552408d82eec15a0c9faa33a "connect-pop3-http.cs" >}}

## Connect to SSL-Enabled POP3 Server {#Establish-Connection-to-SSL-Enabled-POP3-Server}

In case of connecting to an SSL-enabled POP3 server, you would need to set additional security options using [Pop3Client.SecurityOptions][22] property. The following code sample shows how to connect to an SSL-enabled POP3 server.

{{< gist aspose-com-gists 141797c6552408d82eec15a0c9faa33a "connect-pop3-ssl.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try Aspose.Email for .NET for free by [getting a temporary license][23].

## Conclusion

In this article, you have learned how to connect to the POP3 servers using C# from within your .NET applications. Furthermore, you have seen how to connect to an SSL-enabled POP3 server or establish a connection via SOCKS or HTTP proxy. You can explore other features of Aspose.Email for .NET using [documentation][24]. In case you would have any questions or queries, you can contact us via our [forum][25].

## See Also

*   [Send Word Document in Email Body using C#][26]




[1]: https://en.wikipedia.org/wiki/Post_Office_Protocol
[2]: https://en.wikipedia.org/wiki/Post_Office_Protocol
[3]: #API-to-Connect-POP3-Server
[4]: #Connect-to-a-POP3-Server-using-csharp
[5]: #Connect-to-POP3-Server-via-Proxy
[6]: #Establish-Connection-to-SSL-Enabled-POP3-Server
[7]: #Get-a-Free-API-License
[8]: https://products.aspose.com/email/net
[9]: https://downloads.aspose.com/email/net
[10]: https://nuget.org/packages/Aspose.Email
[11]: https://apireference.aspose.com/net/email/aspose.email.clients.pop3/pop3client
[12]: https://apireference.aspose.com/net/email/aspose.email.clients.pop3/pop3client
[13]: https://apireference.aspose.com/net/email/aspose.email.clients.pop3/pop3client
[14]: https://apireference.aspose.com/email/net/aspose.email.clients/socksproxy
[15]: https://apireference.aspose.com/net/email/aspose.email.clients.pop3/pop3client
[16]: https://apireference.aspose.com/email/net/aspose.email.clients/emailclient/properties/proxy
[17]: https://apireference.aspose.com/email/net/aspose.email.clients/socksproxy
[18]: https://apireference.aspose.com/email/net/aspose.email.clients/httpproxy
[19]: https://apireference.aspose.com/net/email/aspose.email.clients.pop3/pop3client
[20]: https://apireference.aspose.com/email/net/aspose.email.clients/emailclient/properties/proxy
[21]: https://apireference.aspose.com/email/net/aspose.email.clients/httpproxy
[22]: https://apireference.aspose.com/email/net/aspose.email.clients/emailclient/properties/securityoptions
[23]: https://purchase.aspose.com/temporary-license
[24]: https://docs.aspose.com/email/net/getting-started/
[25]: https://forum.aspose.com/
[26]: https://blog.aspose.com/2021/02/16/send-word-document-in-email-body-using-csharp/





