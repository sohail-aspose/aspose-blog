---
title: 'Read Emails using IMAP in Python'
seoTitle: "Read Emails in Python | Access Mailbox Server via IMAP | Source Code"
description: "Use Python email library to read emails from an email server via IMAP in Python. Get the list of folders, select a folder and read emails dynamically."
date: Fri, 17 Dec 2021 13:31:08 +0000
draft: false
url: /2021/12/17/read-emails-using-imap-in-python/
author: Usman Aziz
summary: 'In various cases, the email servers are accessed from within the Python applications to read emails or implement email clients. For retrieving emails from an email server, [Internet Message Access Protocol][1] (IMAP) protocol is commonly used. In this article, we will show you **how to read emails from a server using IMAP in Python**. The article will explicitly cover how to connect to an email server, access the desired folder, and read emails.'
tags: ['Access Email Folders from Mailbox in Python', 'Connect to IMAP Server in Python', 'Python Library to Read Emails using IMAP', 'Read Emails from a Folder in Python']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Connect to IMAP Server C#">}}


In various cases, the email servers are accessed from within the Python applications to read emails or to implement email clients. For retrieving emails from an email server, [Internet Message Access Protocol][2] (IMAP) protocol is commonly used. In this article, we will show you **how to read emails from a server using IMAP in Python**. The article will explicitly cover how to connect to an email server, access the desired folder, and read emails.

*   [Python Library to Read Emails using IMAP][3]
*   [Connect to an IMAP Server in Python][4]
*   [Access Email Folders from Mailbox][5]
*   [Read Emails from a Folder][6]

## Python Library to Read Emails using IMAP {#API-to-Connect-IMAP-Server}

To read emails from the email server via IMAP, we will use [Aspose.Email for Python via .NET][7]. It is a powerful email library that lets you send emails and access mailboxes from email servers. You can install the library from [PyPI][8] using the following command.

```
pip install Aspose.Email-for-Python-via-NET
```

For manual installation using a **.whl** file, you can follow the steps below.

*   Download the installable _.whl_ file from the [downloads][9] section.
*   From the command line, use command: _**pip install <<FileName>>.whl**_ to install the library.

## Connect to Email Server via IMAP in Python {#Connect-to-IMAP-Server-in-csharp}

The following are the steps to connect to an email server using IMAP.

1.  Create an instance of the **ImapClient **class and initialize it with hostname, port, username, and password.
2.  Use the **ImapClient** object to access the mailbox.

The following code sample shows how to connect to an email server using IMAP in Python.

{{< gist aspose-com-gists 9132c041d110e75d026870a96a08b189 "connect-email-server-imap.py" >}}

## Access Email Folders from Mailbox in Python {#Access-Email-Folders-from-Mailbox}

Once you have established the connection to the email server, you can choose the folder from which you want to read the email messages. Let's first check out how to get the list of all the folders in the mailbox. The following are the steps to get information about each folder.

1.  Create an instance of the **ImapClient **class and initialize it with hostname, port, username, and password.
2.  Use **ImapClient.list\_folders()** method to get folders collection in an object.
3.  Loop through the collection and retrive folders' details.

The following code sample shows how to print details of the folders in a mailbox.

{{< gist aspose-com-gists 9132c041d110e75d026870a96a08b189 "get-folder-list-imap.py" >}}

Let's now proceed to access a particular folder in the mailbox using IMAP.

1.  Create an instance of the **ImapClient **class and initialize it with hostname, port, username, and password.
2.  Use **ImapClient.select\_folder(string)** method to select the folder.

The following code sample shows how to select an email folder from the mailbox.

{{< gist aspose-com-gists 9132c041d110e75d026870a96a08b189 "select-folder-imap.py" >}}

## Read Emails from a Folder in Python {#Read-Emails-from-a-Folder}

The following are the steps to read email messages from a particular folder in the mailbox using Python.

1.  Create an instance of the **ImapClient **class and initialize it with hostname, port, username, and password.
2.  Use **ImapClient.select\_folder(string)** method to select the folder.
3.  Get list of messages in the folder using **client.list\_messages()** method.
4.  Loop through the collection of messages.
5.  Get details of each email message and save it to the disk if required.

The following code sample shows how to read emails from an email server in Python.

{{< gist aspose-com-gists 9132c041d110e75d026870a96a08b189 "read-emails-imap.py" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Email for Python via .NET for free by [getting a temporary license][10].

## Conclusion

In this article, you have learned how to read emails from an email server using IMAP in Python. The code samples have demonstrated how to connect to an email server, get the list of folders in the mailbox, select a folder and read emails. In addition, you can visit [documentation][11] to explore more about Aspose.Email for Python via .NET. Also, you can download the complete package of source code samples from [GitHub][12]. In case you would have any questions or queries, feel free to let us know via our [forum][13].

## See Also

*   [Send Emails using Python Email Library][14]
*   [Read Email Messages using Python][15]
*   [Convert Emails to HTML in Python][16]




[1]: https://en.wikipedia.org/wiki/Internet_Message_Access_Protocol
[2]: https://en.wikipedia.org/wiki/Internet_Message_Access_Protocol
[3]: #API-to-Connect-IMAP-Server
[4]: #Connect-to-IMAP-Server-in-csharp
[5]: #Access-Email-Folders-from-Mailbox
[6]: #Read-Emails-from-a-Folder
[7]: https://products.aspose.com/email/python-net/
[8]: https://pypi.org/project/Aspose.Email-for-Python-via-NET/
[9]: https://downloads.aspose.com/email/pythonnet
[10]: https://purchase.aspose.com/temporary-license
[11]: https://docs.aspose.com/email/pythonnet/
[12]: https://github.com/aspose-email/Aspose.Email-Python-Dotnet
[13]: https://forum.aspose.com/
[14]: https://blog.aspose.com/2021/05/21/send-emails-in-python/
[15]: https://blog.aspose.com/2021/06/04/read-emails-in-python-using-pop3-or-imap/
[16]: https://blog.aspose.com/2021/05/24/convert-emails-to-html-in-python/




