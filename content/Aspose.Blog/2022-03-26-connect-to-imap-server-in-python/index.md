---
title: 'Connect to IMAP Servers in Python'
seoTitle: "Connect to IMAP Servers in Python | Fetch Messages from IMAP Server"
description: "Use Python email library to connect to IMAP server programmatically in Python. Read email messages from IMAP servers in Python."
date: Sat, 26 Mar 2022 10:08:00 +0000
draft: false
url: /2022/03/26/connect-to-imap-server-in-python/
author: Usman Aziz
summary: '[Internet Message Access Protocol][1] (IMAP) is one of the most commonly used protocols for reading messages from an email server. In order to access the mailbox from your client applications, you would first need to establish a connection with the IMAP server. To achieve this, this article covers **how to connect to an IMAP server using Python**. Furthermore, you will learn how to fetch messages from an IMAP server programmatically.'
tags: ['Connect to an IMAP Server in Python', 'Fetch Messages from IMAP Server in Python', 'Python Library to Connect IMAP Server', 'python email library']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Connect-IMAP-Server.png" alt="Connect to IMAP Server in Python">}}


[Internet Message Access Protocol][2] (IMAP) is one of the most commonly used protocols for reading messages from an email server. In order to access the mailbox from your client applications, you would first need to establish a connection with the IMAP server. To achieve this, this article covers **how to connect to an IMAP server using Python**. Furthermore, you will learn how to fetch messages from an IMAP server programmatically.

*   [Python Library to Connect IMAP Server][3]
*   [Connect to an IMAP Server][4]
*   [Fetch Messages from IMAP Server][5]

## Python Library to Connect IMAP Server {#API-to-Connect-IMAP-Servers}

[Aspose.Email for Python][6] is a feature-rich library to create email client applications using Python. Using the library, you can easily access IMAP servers and work with messages. You can install the library from [PyPI][7] using the following command.

```
> pip install Aspose.Email-for-Python-via-NET
```

## Connect to an IMAP Server in Python {#Connect-to-IMAP-Server}

Before connecting to an IMAP server, you need to have the following things known.

*   Host
*   Username
*   Password
*   Port

Once you have them, you can configure the IMAP client using the following steps.

*   Create an object of **ImapClient** class and initialize it with host, username, password, and port number.
*   Set security options using ****ImapClient**.security\_options** property.
*   Once done, you can work with the IMAP server using the ******ImapClient****** object.

The following code sample shows how to establish a connection with an IMAP server in Python.

{{< gist aspose-com-gists c7412861cf4d24878c1b922133e5862d "connect-imap-server.py" >}}

## Fetch Email Messages from IMAP Server in Python {#Fetch-Messages-from-IMAP-Server}

After establishing the connection, you can proceed to fetch the emails from IMAP server in Python. The following are the steps to perform this operation.

*   Create an object of ****ImapClient**** class and configure it.
*   Select the desired message folder using the **select\_folder()** method.
*   Loop through the list of messages you get using the **list\_messages()** method.
*   Save message to disk using **save\_message()** method, if required.

The following code sample shows how to read messages from an IMAP server in Python.

{{< gist aspose-com-gists c7412861cf4d24878c1b922133e5862d "fetch-emails-from-imap.py" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try and use Aspose.Email for Python for free by [getting a temporary license][8].

## Conclusion

In this article, you have learned how to connect to an IMAP server in Python. Furthermore, you have seen how to fetch messages from an IMAP server and save them on disk programmatically in Python. Besides, you can explore other features of Aspose.Email using [documentation][9]. Also, you can post your questions or queries to our [forum][10].

## See Also

*   [Send Emails in Python - Python Email API][11]




[1]: https://en.wikipedia.org/wiki/Internet_Message_Access_Protocol
[2]: https://en.wikipedia.org/wiki/Internet_Message_Access_Protocol
[3]: #API-to-Connect-IMAP-Servers
[4]: #Connect-to-IMAP-Server
[5]: #Fetch-Messages-from-IMAP-Server
[6]: https://products.aspose.com/email/python-net/
[7]: https://pypi.org/project/Aspose.Email-for-Python-via-NET/
[8]: https://purchase.aspose.com/temporary-license
[9]: https://docs.aspose.com/email/python-net/
[10]: https://forum.aspose.com/
[11]: https://blog.aspose.com/2021/05/21/send-emails-in-python/




