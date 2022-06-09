---
title: 'Connect to SMTP Server using Python'
seoTitle: "Connect to SMTP Server in Python | Access Emails via SMTP in Python"
description: "Use Python email library to connect to SMTP server in Python. Access mailbox and read emails via SMTP from within Python applications."
date: Thu, 16 Dec 2021 15:38:41 +0000
draft: false
url: /2021/12/16/connect-to-smtp-server-using-python/
author: Usman Aziz
summary: '[Simple Mail Transfer Protocol][1] (SMTP) is the most commonly used email protocol that deals with sending email messages from client applications to the email server. In various cases, the email clients are implemented within Python applications to send emails via SMTP. For such scenarios, this article covers **how to connect to an SMTP server using Python**. Furthermore, it demonstrates how to send an email via SMTP.'
tags: ['connect to smtp server in python', 'python email library', 'send emails synchronously in python', 'send emails via smtp in python']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Connect to SMTP Servers using Python">}}


[Simple Mail Transfer Protocol][2] (SMTP) is the most commonly used email protocol that deals with sending email messages from client applications to the email server. In various cases, the email clients are implemented within Python applications to send emails via SMTP. For such scenarios, this article covers **how to connect to an SMTP server using Python**. Furthermore, it demonstrates how to send an email via SMTP.

*   [Python Library to Connect SMTP Server][3]
*   [Connect to an SMTP Server][4]
*   [Send Emails via SMTP in Python][5]

## Python Library to Connect SMTP Server {#API-to-Connect-SMTP-Servers}

[Aspose.Email for Python via .NET][6] is a Python library to create, send and manipulate emails. It allows you to implement your own email clients in Python seamlessly. We will use this library to connect to SMTP servers. You can install the library from [PyPI][7] using the following command.

```
pip install Aspose.Email-for-Python-via-NET
```

Or, you can follow the below steps for manual installation.

*   Download the installable _.whl_ file from the [downloads][8] section.
*   From the command line, use command: _**pip install <<FileName>>.whl**_ to install the API.
*   Download a complete package of source code samples from [GitHub][9].

## Connect to an SMTP Server in Python {#Connect-to-SMTP-Server-using-csharp}

Before connecting to an SMTP server, you need to have the following things known.

*   Username
*   Password
*   Port

Once you have them, you can configure the SMTP client using the following steps.

*   First, create an object of **SmtpClient** class.
*   Then, set host, username, password, and port number using **SmtpClient.host**, **SmtpClient.username**, **SmtpClient.password**, and **SmtpClient.port** properties, respectively.
*   Set security options using **SmtpClient.security\_options** property.
*   Finally, proceed to access mailbox using **SmtpClient** object.

The following code sample shows how to establish a connection with the SMTP server in Python.

{{< gist aspose-com-gists 0987ed331c4b11d0d17dbddcb323c6c8 "connect-smtp-server.py" >}}

## Send Emails via SMTP in Python {#Send-Emails-via-SMTP-in-Python}

After establishing the connection to SMTP server, you can send emails. The following code sample shows how to send an email via SMTP in Python.

{{< gist aspose-com-gists 0987ed331c4b11d0d17dbddcb323c6c8 "send-email-smtp.py" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Email for Python via .NET for free by [getting a temporary license][10].

## Conclusion

In this article, you have learned how to connect to an SMTP server using Python. Also, you have seen how to send an email via SMTP in Python. You can visit [documentation][11] to explore more about Aspose.Email for Python via .NET. In case you would have any questions or queries, feel free to let us know via our [forum][12].

## See Also

*   [Send Emails using Python Email Library][13]
*   [Read Email Messages using Python][14]
*   [Convert Emails to HTML in Python][15]




[1]: https://en.wikipedia.org/wiki/Simple_Mail_Transfer_Protocol
[2]: https://en.wikipedia.org/wiki/Simple_Mail_Transfer_Protocol
[3]: #API-to-Connect-SMTP-Servers
[4]: #Connect-to-SMTP-Server-using-csharp
[5]: #Send-Emails-via-SMTP-in-Python
[6]: https://products.aspose.com/email/python-net/
[7]: https://pypi.org/project/Aspose.Email-for-Python-via-NET/
[8]: https://downloads.aspose.com/email/pythonnet
[9]: https://github.com/aspose-email/Aspose.Email-Python-Dotnet
[10]: https://purchase.aspose.com/temporary-license
[11]: https://docs.aspose.com/email/pythonnet/
[12]: https://forum.aspose.com/
[13]: https://blog.aspose.com/2021/05/21/send-emails-in-python/
[14]: https://blog.aspose.com/2021/06/04/read-emails-in-python-using-pop3-or-imap/
[15]: https://blog.aspose.com/2021/05/24/convert-emails-to-html-in-python/




