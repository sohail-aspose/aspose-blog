---
title: 'Fetch Emails from POP3 Server in Python'
seoTitle: "Fetch Emails from POP3 Server in Python | Python POP3 Library"
description: "Use the Python email library to connect to POP3 servers in Python. Fetch email messages from POP3 servers programmatically in Python."
date: Tue, 01 Mar 2022 18:09:00 +0000
draft: false
url: /2022/03/01/fetch-emails-from-pop3-server-in-python/
author: Usman Aziz
summary: ''
tags: ['Connect to a POP3 Server in Python', 'Fetch Emails from Mailbox on POP3 Server in Python', 'Python Library to Fetch Emails from POP3 Server', 'python email library']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Fetch-Emails-from-POP3-Servers.png" alt="Fetch Emails from POP3 Server in Python">}}


[Post Office Protocol][1] (POP3) is a popular email protocol that is used to fetch emails from the mail servers. To work with the email messages in the mailbox, you first need to establish a connection to the POP3 server. To achieve that, this article covers how to connect to a POP3 server from within a Python application. Furthermore, you will learn **how to fetch email messages from a POP3 server programmatically in Python**.

*   [Python Library to Fetch Emails from POP3 Server][2]
*   [Connect to a POP3 Server in Python][3]
*   [Fetch Emails from Mailbox on POP3 Server][4]

## Python Library to Fetch Emails from POP3 Server {#Python-Library-to-Fetch-Emails-from-POP3-Server}

To retrieve the emails from POP3 servers, we will use [Aspose.Email for Python][5]. It is a feature-rich email processing library that lets you create and send emails and work with popular email protocols. You can install the library from [PyPI][6] using the following command.

```
> pip install Aspose.Email-for-Python-via-NET
```

## Connect to a POP3 Server in Python {#Connect-to-a-POP3-Server-in-Python}

Before you access the mailbox on a POP3 server, you first need to establish a connection. The following are the steps to establish a connection with the POP3 server in Python.

*   Create an instance of the **Pop3Client** class.
*   Specify the host, username, and password using the **Pop3Client** object.
*   Access the mailbox.

The following code sample shows how to connect to a POP3 server in Python.

{{< gist aspose-com-gists e0c82cfa3355c28a5208ca2fab91f7a5 "connect-pop3-server.py" >}}

## Fetch Emails from POP3 Server in Python {#Fetch-Emails-from-Mailbox-on-POP3-Server}

Once you have established the connection with the POP3 server, you can read emails from the mailbox. The following are the steps to fetch emails from a POP3 server in Python.

*   Establish the connection with the POP3 server using the **Pop3Client** class.
*   Get count of messages using **Pop3Client.get\_message\_count()** method.
*   Start a loop and fetch each message by index using **Pop3Client.fetch\_message()** method.
*   Read details of the message such as subject, from, body, etc.

The following code sample shows how to fetch emails from a POP3 server in Python.

{{< gist aspose-com-gists e0c82cfa3355c28a5208ca2fab91f7a5 "fetch-emails-from-pop3.py" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try and use Aspose.Email for Python for free by [getting a temporary license][7].

## Conclusion

In this article, you have learned how to connect to a POP3 server in Python. Furthermore, you have seen how to fetch email messages from a POP3 server programmatically in Python. In addition, you can explore more about Aspose.Email using [documentation][8]. Also, you can share your questions or queries on our [forum][9].

## See Also

*   [Send Emails in Python - Python Email API][10]




[1]: https://en.wikipedia.org/wiki/Post_Office_Protocol
[2]: #Python-Library-to-Fetch-Emails-from-POP3-Server
[3]: #Connect-to-a-POP3-Server-in-Python
[4]: #Fetch-Emails-from-Mailbox-on-POP3-Server
[5]: https://products.aspose.com/email/python-net/
[6]: https://pypi.org/project/Aspose.Email-for-Python-via-NET/
[7]: https://purchase.aspose.com/temporary-license
[8]: https://docs.aspose.com/email/python-net/
[9]: https://forum.aspose.com/
[10]: https://blog.aspose.com/2021/05/21/send-emails-in-python/




