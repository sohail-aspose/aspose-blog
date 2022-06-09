---
title: 'Read Emails in Python using POP3 or IMAP'
seoTitle: "Read Emails in Python using POP3 or IMAP | Python Email API | Aspose"
description: "Use Python email API to read emails from mail servers in Python. Fetch email messages using POP3 or IMAP protocols seamlessly."
date: Fri, 04 Jun 2021 01:10:58 +0000
draft: false
url: /2021/06/04/read-emails-in-python-using-pop3-or-imap/
author: Usman Aziz
summary: 'In this article, you will learn how to retrieve email messages from the mail servers programmatically. Particularly, you will come to know **how to connect to the mail server using [IMAP][1] or [POP3][2] protocols and read the emails in Python**.'
tags: ['Fetch Email Messages using IMAP', 'Fetch Email Messages using POP3', 'Python API to Read Emails', 'Read Emails from Mail Server in Python']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Read-Emails.jpg" alt="">}}


In this article, you will learn how to retrieve email messages from the mail servers programmatically. Particularly, you will come to know **how to connect to the mail server using [IMAP][3] or [POP3][4] protocols and read the emails in Python**.

*   [Python API to Read Emails][5]
*   [Read Emails from Mail Servers in Python][6]
    *   [Fetch Email Messages using POP3][7]
    *   [Fetch Email Messages using IMAP][8]

## Python API to Read Emails {#Python-API-to-Read-Emails}

In order to read emails from the mail servers, we will use [Aspose.Email for Python via .NET][9]. It is a feature-rich email API that lets you implement email clients from within your Python applications. You can either [download][10] _.whl_ file or install the API using the following pip command.

```
> pip install Aspose.Email-for-Python-via-NET
```

## Read Emails from Mail Servers in Python {#Read-Emails-from-Mail-Server-in-Python}

POP3 and IMAP are commonly used for retrieving emails from the mail servers. The following sections demonstrate how to read emails using both of the email protocols separately.

### Read Email Messages using POP3 {#Read-Email-Messages-using-POP3}

The following are the steps to read email messages using POP3.

*   Create an object of **Pop3Client** class and initialize it with host, port, username and password.
*   Set security options using **Pop3Client.security\_options** property.
*   Get message count using **Pop3Client.get\_message\_count()** method.
*   Access each message in a loop using **Pop3Client.fetch\_message()** method.

The following code sample shows how to read an email in Python using POP3.

{{< gist aspose-com-gists 971f68115475795758003fdd3ebc579d "read-email-POP3.py" >}}

### Read Email Messages using IMAP {#Fetch-Email-Messages-using-IMAP}

The following are the steps to read email messages using IMAP.

*   Create an object of **ImapClient** class and initialize it with host, port, username, and password.
*   Select folder using **ImapClient.select\_folder(folderName)** method.
*   Loop through the list of the messages using **ImapClient.list\_messages()** method.

The following code sample shows how to read email messages using IMAP in Python.

{{< gist aspose-com-gists 971f68115475795758003fdd3ebc579d "read-email-IMAP.py" >}}

## Get a Free API License

You can use Aspose.Email for Python via .NET by requesting a [free temporary license][11].

## Conclusion

In this article, you have learned how to read emails from mail servers using Python. Particularly, you have seen how to use POP3 and IMAP clients to fetch and read email messages. You can explore more about the Python email API using the [documentation][12]. Furthermore, you can post your queries on our [forum][13].

## See Also

*   [Send Emails in Python – Python Email API][14]




[1]: https://en.wikipedia.org/wiki/Internet_Message_Access_Protocol#:~:text=In%20computing%2C%20the%20Internet%20Message,is%20defined%20by%20RFC%203501.
[2]: https://en.wikipedia.org/wiki/Post_Office_Protocol
[3]: https://en.wikipedia.org/wiki/Internet_Message_Access_Protocol#:~:text=In%20computing%2C%20the%20Internet%20Message,is%20defined%20by%20RFC%203501.
[4]: https://en.wikipedia.org/wiki/Post_Office_Protocol
[5]: #Python-API-to-Read-Emails
[6]: #Read-Emails-from-Mail-Server-in-Python
[7]: #Read-Email-Messages-using-POP3
[8]: #Fetch-Email-Messages-using-IMAP
[9]: https://products.aspose.com/email/python-net/
[10]: https://downloads.aspose.com/email/pythonnet
[11]: https://products.aspose.com/email
[12]: https://docs.aspose.com/email/pythonnet/getting-started/
[13]: https://forum.aspose.com/
[14]: https://blog.aspose.com/2021/05/21/send-emails-in-python/





