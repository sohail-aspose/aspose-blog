---
title: 'Connect to SMTP Server in Python'
date: Mon, 25 Apr 2022 18:02:45 +0000
draft: false
url: /2022/04/25/connect-to-smtp-server-in-python/
author: 'Usman Aziz'
summary: '[Simple Mail Transfer Protocol][1] (SMTP) is a well-known and commonly used protocol for sending email messages from client applications to the email server. While implementing email automation features, you may need to connect to the SMTP servers from within your Python applications. For such scenarios, this article covers **how to connect to an SMTP server programmatically in Python**. Furthermore, you will learn how to send an email after making a connection to an SMTP server.'
tags: ['Connect to an SMTP Server in Python', 'Python Library to Connect SMTP Server', 'Send an Email via SMTP in Python']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Connect-SMTP-Server.png" alt="Connect to SMTP Server in Python">}}


[Simple Mail Transfer Protocol][2] (SMTP) is a well-known and commonly used protocol for sending email messages from client applications to the email server. While implementing email automation features, you may need to connect to the SMTP servers from within your Python applications. For such scenarios, this article covers **how to connect to an SMTP server programmatically in Python**. Furthermore, you will learn how to send an email after making a connection to an SMTP server.

*   [Python Library to Connect SMTP Server][3]
*   [Connect to an SMTP Server][4]
*   [Send an Email via SMTP][5]

## Python Library to Connect SMTP Server {#API-to-Connect-SMTP-Servers}

[Aspose.Email for Python][6] is an amazing library that lets you create Python-based email client applications. Using the library, you can easily connect to and access the SMTP servers without writing complex code. You can install the library from [PyPI][7] using the following command.

```
> pip install Aspose.Email-for-Python-via-NET
```

## Connect to SMTP Server in Python {#Connect-to-SMTP-Server-using-csharp}

Before connecting to an SMTP server, you need to have the following things known.

*   Host
*   Username
*   Password
*   Port

Once you have them, you can configure the SMTP client using the following steps.

*   Create an object of **SmtpClient** class.
*   Set host, username, password, and port number using the **SmtpClient** object.
*   Set security options using **SmtpClient.security\_options** property.
*   At this point, you can communicate with the server using the **SmtpClient** object.

The following code sample shows how to set up a connection with an SMTP server in Python.

{{< gist aspose-com-gists 6352ca6844ca0c4643e38451ecca76c2 "connect-smtp-server.py" >}}

## Send an Email via SMTP in Python {#Send-an-Email-via-SMTP}

Once you have established the connection, you can proceed to send emails via SMTP in Python. The following are the steps to do so.

*   Create an object of **SmtpClient** class and set credentials and security options.
*   Create an object of **MailMessage** class.
*   Set email message's subject, body, to, from, and other fields.
*   Send message using **SmtpClient.send(MailMessage)** method.

The following code sample shows how to send an email via SMTP in Python.

{{< gist aspose-com-gists 6352ca6844ca0c4643e38451ecca76c2 "send-email-via-smtp.py" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try and use Aspose.Email for Python for free by [getting a temporary license][8].

## Conclusion

In this article, you have learned how to connect to an SMTP server in Python. Furthermore, you have seen how to send an email after making a connection to SMTP server programmatically in Python. In addition, you can explore more about Aspose.Email using [documentation][9]. Also, you can share your questions or queries on our [forum][10].

## See Also

*   [Send Emails in Python - Python Email API][11]




[1]: https://en.wikipedia.org/wiki/Simple_Mail_Transfer_Protocol
[2]: https://en.wikipedia.org/wiki/Simple_Mail_Transfer_Protocol
[3]: #API-to-Connect-SMTP-Servers
[4]: #Connect-to-SMTP-Server-using-csharp
[5]: #Send-an-Email-via-SMTP
[6]: https://products.aspose.com/email/python-net/
[7]: https://pypi.org/project/Aspose.Email-for-Python-via-NET/
[8]: https://purchase.aspose.com/temporary-license
[9]: https://docs.aspose.com/email/python-net/
[10]: https://forum.aspose.com/
[11]: https://blog.aspose.com/2021/05/21/send-emails-in-python/




