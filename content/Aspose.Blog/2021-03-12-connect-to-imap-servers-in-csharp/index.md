---
title: 'Connect to IMAP Servers using C#'
seoTitle: "Connect to IMAP Server in C# | Connect IMAP via HTTP or SOCKS Proxy"
description: "Use .NET Email API to connect to IMAP server using C#. Connect to IMAP server using HTTP or SOCKS proxy. Connect to SSL-enabled IMAP server."
date: Fri, 12 Mar 2021 11:53:00 +0000
draft: false
url: /2021/03/12/connect-to-imap-servers-in-csharp/
author: Usman Aziz
summary: '[Internet Message Access Protocol][1] (IMAP) is the most commonly used protocol for retrieving messages from an email server. In order to access the mailbox from your client applications, you would first need to establish a connection with the IMAP server. To achieve this, this article covers **how to connect to an IMAP server via SOCKS or HTTP proxy using C#**. Furthermore, you will learn how to connect to an SSL-enabled IMAP server programmatically.'
tags: ['connect to imap server in csharp', 'connect to imap server via HTTP in csharp', 'connect to imap server via socks in csharp', 'connect to ssl enabled imap server in csharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Connect to IMAP Server C#">}}


[Internet Message Access Protocol][2] (IMAP) is the most commonly used protocol for retrieving messages from an email server. In order to access the mailbox from your client applications, you would first need to establish a connection with the IMAP server. To achieve this, this article covers **how to connect to an IMAP server via SOCKS or HTTP proxy using [C#][3]**. Furthermore, you will learn how to connect to an SSL-enabled IMAP server programmatically.

*   [C# API to Connect IMAP Server][4]
*   [Connect to IMAP Server in C#][5]
*   [Connect to IMAP Server via SOCKS Proxy][6]
*   [Access IMAP Server via HTTP Proxy][7]
*   [Connect to SSL Enabled IMAP Server][8]
*   [Get a Free API License][9]

## C# API to Connect IMAP Server {#API-to-Connect-IMAP-Server}

[Aspose.Email for .NET][10] is a feature-rich API that lets you implement email clients from within your .NET applications. In addition, it lets you connect to IMAP servers and access the mailboxes via SOCKS or HTTP proxies. You can either [download][11] the API or install it via [NuGet][12].

```
PM> Install-Package Aspose.Email
```

## Connect to IMAP Server in C# {#Connect-to-IMAP-Server-in-csharp}

The following are the steps to connect to an IMAP server using Aspose.Email for .NET.

1.  Create an instance of the [ImapClient][13] class.
2.  Specify the hostname, username, and password in the [ImapClient][14] constructor.
3.  Use the [ImapClient][15] object to access the mailbox.

The following code sample shows how to connect to an IMAP server using C#.

{{< gist aspose-com-gists 511425122d8f8dce06ef076bb0308463 "connect-imap.cs" >}}

## Connect to IMAP Server via SOCKS Proxy {#Connect-to-IMAP-Server-via-SOCKS-Proxy}

In various cases, email servers are not directly accessible and you have to use a proxy server. In order to connect the IMAP server via SOCKS proxy, Aspose.Email for .NET supports SOCKS version 4, 4a, and 5. The following are the steps to connect to an IMAP server via SOCKS proxy.

1.  Create an instance of the [ImapClient][16] class.
2.  Specify the hostname, username, and password in the [ImapClient][17] constructor.
3.  Create an instance of [SocksProxy][18] and initialize it with proxy address, port, and SOCKS version.
4.  Set proxy for IMAP using [ImapClient.Proxy][19] property.

The following code sample shows how to connect to an IMAP server via SOCKS proxy.

{{< gist aspose-com-gists 511425122d8f8dce06ef076bb0308463 "connect-imap-socks.cs" >}}

## Connect to IMAP Server via HTTP Proxy {#Access-IMAP-Server-via-HTTP-Proxy}

The following are the steps to connect to an IMAP server via HTTP proxy.

1.  Create an instance of the [ImapClient][20] class.
2.  Specify the hostname, username, and password in the [ImapClient][21] constructor.
3.  Create an instance of [HttpProxy][22] and initialize it with the proxy address and port number.
4.  Set HTTP proxy for IMAP using [ImapClient.Proxy][23] property.

The following code sample shows how to connect to an IMAP server via HTTP proxy.

{{< gist aspose-com-gists 511425122d8f8dce06ef076bb0308463 "connect-imap-http.cs" >}}

## Connect to SSL Enabled IMAP Server in C# {#Create-Connection-with-SSL-Enabled-IMAP-Server}

The following are the steps to connect to an SSL-enabled IMAP server using C#.

1.  Create an instance of the [ImapClient][24] class.
2.  Specify the hostname, username, and password in the [ImapClient][25] constructor.
3.  Set [ImapClient.SecurityOptions][26] property to [SecurityOptions.SSLImplicit][27].

The following code sample shows how to connect to an SSL-enabled IMAP server.

{{< gist aspose-com-gists 511425122d8f8dce06ef076bb0308463 "connect-imap-ssl.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try and use Aspose.Email for .NET for free by [getting a temporary license][28].

## Conclusion

In this article, you have learned how to connect to an IMAP server using C#. Furthermore, the step-by-step guide and code samples have demonstrated how to connect to an IMAP server via SOCKS or HTTP proxy. You can explore more about the API using [documentation][29]. For any questions or queries, feel free to let us know via our [forum][30].

## See Also

*   [Connect to SMTP Servers using C#][31]




[1]: https://en.wikipedia.org/wiki/Internet_Message_Access_Protocol
[2]: https://en.wikipedia.org/wiki/Internet_Message_Access_Protocol
[3]: https://docs.fileformat.com/programming/cs/
[4]: #API-to-Connect-IMAP-Server
[5]: #Connect-to-IMAP-Server-in-csharp
[6]: #Connect-to-IMAP-Server-via-SOCKS-Proxy
[7]: #Access-IMAP-Server-via-HTTP-Proxy
[8]: #Create-Connection-with-SSL-Enabled-IMAP-Server
[9]: #Get-a-Free-API-License
[10]: https://products.aspose.com/email/net
[11]: https://downloads.aspose.com/email/net
[12]: https://www.nuget.org/packages/Aspose.Email
[13]: https://apireference.aspose.com/net/email/aspose.email.clients.imap/imapclient
[14]: https://apireference.aspose.com/net/email/aspose.email.clients.imap/imapclient/constructors/8
[15]: https://apireference.aspose.com/net/email/aspose.email.clients.imap/imapclient
[16]: https://apireference.aspose.com/net/email/aspose.email.clients.imap/imapclient
[17]: https://apireference.aspose.com/net/email/aspose.email.clients.imap/imapclient/constructors/8
[18]: https://apireference.aspose.com/net/email/aspose.email.clients/socksproxy
[19]: https://apireference.aspose.com/email/net/aspose.email.clients/emailclient/properties/proxy
[20]: https://apireference.aspose.com/net/email/aspose.email.clients.imap/imapclient
[21]: https://apireference.aspose.com/net/email/aspose.email.clients.imap/imapclient/constructors/8
[22]: https://apireference.aspose.com/email/net/aspose.email.clients/httpproxy
[23]: https://apireference.aspose.com/email/net/aspose.email.clients/emailclient/properties/proxy
[24]: https://apireference.aspose.com/net/email/aspose.email.clients.imap/imapclient
[25]: https://apireference.aspose.com/net/email/aspose.email.clients.imap/imapclient/constructors/8
[26]: https://apireference.aspose.com/email/net/aspose.email.clients/emailclient/properties/securityoptions
[27]: https://apireference.aspose.com/email/net/aspose.email.clients/securityoptions
[28]: https://purchase.aspose.com/temporary-license
[29]: https://docs.aspose.com/email/net/developer-guide/
[30]: https://forum.aspose.com/
[31]: https://blog.aspose.com/2021/02/23/connect-to-smtp-servers-using-csharp/





