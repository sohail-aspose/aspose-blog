---
title: 'Connect to SMTP Servers using C#'
seoTitle: "Connect to SMTP Server in C# | SOCKS and HTTP Proxy Server"
description: "Use .NET email API to connect to SMTP server and send emails using C#. Connect to SMTP server via SOCKS or HTTP proxy servers."
date: Tue, 23 Feb 2021 11:52:00 +0000
draft: false
url: /2021/02/23/connect-to-smtp-servers-using-csharp/
author: Usman Aziz
summary: '[Simple Mail Transfer Protocol][1] (SMTP) is the most commonly used email protocol that deals with sending email messages from client applications to the email server. In various cases, the email clients are implemented within .NET applications in order to send emails via SMTP. For such scenarios, this article covers **how to connect to an SMTP server programmatically using C#**. Furthermore, the code samples demonstrate how to send an email via SMTP client after connection establishment.'
tags: ['Connect to SMTP in Csharp', 'Connect to SMTP via HTTP Proxy in Csharp', 'Connect to SMTP via SOCKS Proxy in Csharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Connect to SMTP Servers using C#">}}


[Simple Mail Transfer Protocol][2] (SMTP) is the most commonly used email protocol that deals with sending email messages from client applications to the email server. In various cases, the email clients are implemented within .NET applications in order to send emails via SMTP. For such scenarios, this article covers **how to connect to an SMTP server programmatically using [C#][3]**. Furthermore, the code samples demonstrate how to send an email via SMTP client after connection establishment.

*   [C# API to Connect SMTP Server][4]
*   [Connect to an SMTP Server][5]
    *   [SOCKS Proxy Server][6]
    *   [HTTP Proxy Server][7]
*   [Get a Free API License][8]

## C# API to Connect SMTP Server {#API-to-Connect-SMTP-Servers}

[Aspose.Email for .NET][9] is a C# API that is designed to create powerful email client applications. The API makes it possible to perform complex email operations quite easily within a few lines of code. Furthermore, it allows you to connect SMTP servers via SOCKS and HTTP proxy servers. You can either [download][10] the API's DLL or install it using [NuGet][11].

```
PM> Install-Package Aspose.Email
```

## Connect to SMTP Server using C# {#Connect-to-SMTP-Server-using-csharp}

Before connecting to an SMTP server, you need to have the following things known.

*   Username
*   Password
*   Port

Once you have them, you can configure the SMTP client using the following steps.

*   Create an object of [SmtpClient][12] class.
*   Set username, password, and port number using [SmtpClient.Username][13], [SmtpClient.Password][14], and [SmtpClient.Port][15] properties respectively.
*   Set Security options using [SmtpClient.SecurityOptions][16] property.

The following code sample shows how to set up the API for an SMTP connection in C#.

{{< gist aspose-com-gists 6e5185a63aec6fd70d83098e82b06a32 "Examples-CSharp-SMTP-SSLEnabledSMTPServer-SSLEnabledSMTPServer.cs" >}}

Once you have configured the API, you can connect to an SMTP server using one of the following options.

## Connect to SMTP via SOCKS Proxy Server in C# {#SOCKS-Proxy-Server}

Aspose.Email provides support for versions 4, 4a, and 5 of the SOCKS proxy protocol. The following are the steps to connect to an SMTP server via a SOCKS proxy server using Aspose.Email for .NET.

*   Initialize [SmtpClient][17] with the host address, username, password, and other settings.
*   Create an object of the [SocksProxy][18] class and set the address and port.
*   Set the client’s proxy using [SmtpClient.Proxy][19] property.
*   Send email using [SmtpClient.Send()][20] method.

The following code sample shows how to connect to an SMTP server via SOCKS proxy using C#.

{{< gist aspose-com-gists 6e5185a63aec6fd70d83098e82b06a32 "Examples-CSharp-SMTP-SendEmailViaProxyServer-SendEmailViaProxyServer.cs" >}}

## Connect to SMTP Server via HTTP Proxy Server {#HTTP-Proxy-Server}

The following are the steps to connect to an SMTP server via an HTTP proxy server.

*   Create an instance of the [HttpProxy][21] class and initialize it with IP and port number.
*   Create and configure the [SmtpClient][22] object.
*   Set HTTP proxy using [SmtpClient.Proxy][23] property.
*   Send email using [SmtpClient.Send()][24] method.

The following code sample shows how to connect to an SMTP server via HTTP proxy server.

{{< gist aspose-com-gists 6e5185a63aec6fd70d83098e82b06a32 "Examples-CSharp-SMTP-SendEmailViaHttpProxy-SendEmailViaHttpProxy.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try and use Aspose.Email for .NET for free by [getting a temporary license][25].

## Conclusion

In this article, you have learned how to connect to an SMTP server using C#. Furthermore, the step-by-step guide and code samples have shown how to connect to the SMTP server via SOCKS and HTTP proxy servers. You can explore more about the C# email API using [documentation][26].

## See Also

*   [Create Outlook Messages and Send Emails using C#][27]




[1]: https://en.wikipedia.org/wiki/Simple_Mail_Transfer_Protocol
[2]: https://en.wikipedia.org/wiki/Simple_Mail_Transfer_Protocol
[3]: https://docs.fileformat.com/programming/cs/
[4]: #API-to-Connect-SMTP-Servers
[5]: #Connect-to-SMTP-Server-using-csharp
[6]: #SOCKS-Proxy-Server
[7]: #HTTP-Proxy-Server
[8]: #Get-a-Free-API-License
[9]: https://products.aspose.com/email/net
[10]: https://downloads.aspose.com/email/net
[11]: https://nuget.org/packages/Aspose.Email
[12]: https://apireference.aspose.com/email/net/aspose.email.clients.smtp/smtpclient
[13]: https://apireference.aspose.com/email/net/aspose.email.clients/emailclient/properties/username
[14]: https://apireference.aspose.com/email/net/aspose.email.clients/emailclient/properties/password
[15]: https://apireference.aspose.com/email/net/aspose.email.clients/emailclient/properties/port
[16]: https://apireference.aspose.com/email/net/aspose.email.clients/emailclient/properties/securityoptions
[17]: https://apireference.aspose.com/net/email/aspose.email.clients.smtp/smtpclient
[18]: https://apireference.aspose.com/email/net/aspose.email.clients/socksproxy
[19]: https://apireference.aspose.com/net/email/aspose.email.clients/proxy
[20]: https://apireference.aspose.com/email/net/aspose.email.clients.smtp.smtpclient/send/methods/5
[21]: https://apireference.aspose.com/email/net/aspose.email.clients/httpproxy
[22]: https://apireference.aspose.com/net/email/aspose.email.clients.smtp/smtpclient
[23]: https://apireference.aspose.com/email/net/aspose.email.clients/emailclient/properties/proxy
[24]: https://apireference.aspose.com/email/net/aspose.email.clients.smtp.smtpclient/send/methods/5
[25]: https://purchase.aspose.com/temporary-license
[26]: https://docs.aspose.com/email/net/
[27]: https://blog.aspose.com/2020/01/23/create-send-outlook-email-eml-msg-csharp-net-core/





