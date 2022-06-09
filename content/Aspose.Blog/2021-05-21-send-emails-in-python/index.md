---
title: 'Create and Send Emails via SMTP in Python'
seoTitle: "Python: Create and Send Emails via SMTP | Python Email Library"
description: "Use Python email API to create and send emails from within Python applications via SMTP. Send emails with plain text or HTML body."
date: Fri, 21 May 2021 04:00:00 +0000
draft: false
url: /2021/05/21/send-emails-in-python/
author: Usman Aziz
summary: 'Automated emails are commonly used to send notifications or other messages to subscribers. Also, various emails are triggered based on the actions or behavior of the users. In order to implement email automation, this article covers **how to create and send emails programmatically in Python**.'
tags: ['Create and send emails in python', 'Python API to Send Emails', 'Send Bulk Emails in Python', 'Send Emails with HTML Body Python']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Send-Emails-in-Python.jpg" alt="Send Emails in Python">}}


Automated emails are widely used to send notifications or other messages to subscribers. Also, various emails are triggered based on the actions or behavior of the users. In order to implement email automation, this article covers **how to create and send emails using SMTP in Python**.

*   [Python Library to Send Emails][1]
*   [Create and Send Emails in Python][2]
*   [Send Emails with HTML Body][3]
*   [Send Bulk Emails][4]
*   [Forward an Email Message][5]

## Python Library to Create and Send Emails via SMTP {#Python-API-to-Send-Emails}

In order to create and send emails using SMTP, we will use [Aspose.Email for Python via .NET][6]. It is a powerful Python library that lets you implement feature-rich email clients. You can install the API from [PyPI][7] using the following command.

```
pip install Aspose.Email-for-Python-via-NET
```

Or, you can follow the below steps for manual installation.

*   Download the installable _.whl_ file from the [downloads][8] section.
*   From the command line, use command: _**pip install <<FileName>>.whl**_ to install the API.
*   Download a complete package of source code samples from [GitHub][9].

## Create and Send Emails via SMTP in Python {#Create-and-Send-Emails-in-Python}

The following are the steps to create and send an email via SMTP in Python.

*   Create an object of _MailMessage_ class.
*   Set subject, body, sender's, and recipient's addresses.
*   Set Cc or Bcc (optional).
*   Create a new SMTP client using _SmtpClient_ class and set host, port, username, and password.
*   Set security options.
*   Send email using _SmtpClient.send(MailMessage)_ method.

The following code sample shows how to create and send emails in Python.

{{< gist aspose-com-gists 103afb8b13c3a66b26bd10eda694a733 "send-email.py" >}}

## Send Emails with HTML Body in Python {#Send-Emails-with-HTML-Body}

The following are the steps to send emails with HTML body.

*   Create an object of _MailMessage_ class.
*   Set body of the email using _MailMessage.body\_html_ property.
*   Set _MailMessage.is\_body\_html_ property to true.
*   Assign subject, sender's, and recipient's addresses.
*   Set Cc or Bcc (optional).
*   Create a new SMTP client using _SmtpClient_ class and set host, port, username, and password.
*   Send email using _SmtpClient.send(MailMessage)_ method.

The following code sample shows how to send emails with HTML body in Python.

{{< gist aspose-com-gists 103afb8b13c3a66b26bd10eda694a733 "send-email-html-body.py" >}}

## Send Bulk Emails using SMTP in Python {#Send-Bulk-Emails}

The following are the steps to send bulk emails in Python.

*   Create multiple email messages using _MailMessage_ class and set their properties, such as subject, recipients, etc.
*   Create an object of _MailMessageCollection_ class.
*   Add email messages to the collection using _MailMessageCollection.append(MailMessage)_ method.
*   Create a new SMTP client using _SmtpClient_ class and set host, port, username, and password.
*   Send email using _SmtpClient.send(MailMessageCollection)_ method.

The following code sample shows how to send bulk emails in Python.

{{< gist aspose-com-gists 103afb8b13c3a66b26bd10eda694a733 "send-bulk-emails.py" >}}

## Forward an Email Message in Python {#Forward-an-Email-Message-in-Python}

The following are the steps to forward an email message in Python.

*   Load the email message into an object using _MailMessage.load(String fileName)_ method.
*   Set recipient's address.
*   Create an SMTP client using _SmtpClient_ class.
*   Forward message using _SmtpClient.forward()_ method.

The following code sample shows how to forward an email message in Python.

{{< gist aspose-com-gists 103afb8b13c3a66b26bd10eda694a733 "forward-email.py" >}}

## Get a Free API License

You may request a [Free Temporary License][10] in order to use the API without evaluation limitations.

## Live Demo

*   [Email Editor][11]

## Conclusion

In this article, you have learned how to create and send emails via SMTP in Python. Furthermore, you have seen how to send bulk emails with plain text or HTML body programmatically. You can explore more about the Python email API using the [documentation][12]. In case you would have any questions or queries, feel free to let us know via our [forum][13].

## See Also

*   [Read Email Messages Programmatically using Java][14]
*   [Convert Email Messages to PDF using C#][15]




[1]: #Python-API-to-Send-Emails
[2]: #Create-and-Send-Emails-in-Python
[3]: #Send-Emails-with-HTML-Body
[4]: #Send-Bulk-Emails
[5]: #Forward-an-Email-Message-in-Python
[6]: https://products.aspose.com/email/python-net
[7]: https://pypi.org/project/Aspose.Email-for-Python-via-NET/
[8]: https://downloads.aspose.com/email/pythonnet
[9]: https://github.com/aspose-email/Aspose.Email-Python-Dotnet
[10]: https://purchase.aspose.com/temporary-license
[11]: https://products.aspose.app/email/editor
[12]: https://docs.aspose.com/email/pythonnet/getting-started/
[13]: https://forum.aspose.com/
[14]: https://blog.aspose.com/2021/04/12/read-email-messages-programmatically-using-java/
[15]: https://blog.aspose.com/2021/01/07/convert-emails-to-pdf-using-csharp/





