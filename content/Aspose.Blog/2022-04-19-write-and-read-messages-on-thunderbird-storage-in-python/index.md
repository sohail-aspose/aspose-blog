---
title: 'Write and Read Messages on Thunderbird Storage in Python'
date: Tue, 19 Apr 2022 11:22:53 +0000
draft: false
url: /2022/04/19/write-and-read-messages-on-thunderbird-storage-in-python/
author: 'Usman Aziz'
summary: '[Thunderbird][1] is an open-source email client that allows you to get messages from more than one email servers. Thus, you can manage emails from multiple accounts in a single place. In certain cases, you may need to access email messages from Thunderbird programmatically. Furthermore, you may have to write new messages on Thunderbird. In this article, you will learn **how to write and read messages on Thunderbird storage in Python**.'
tags: ['Python Library to Write and Read Messages on Thunderbird', 'Python Thunderbird Library', 'Read Messages from Thunderbird in Python', 'Write Messages on Thunderbird in Python']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Write-and-Read-Messages-in-Thunderbird.png" alt="Write and Read Messages on Thunderbird in Python">}}


[Thunderbird][2] is an open-source email client that allows you to get messages from more than one email servers. Thus, you can manage emails from multiple accounts in a single place. In certain cases, you may need to access email messages from Thunderbird programmatically. Furthermore, you may have to write new messages on Thunderbird. In this article, you will learn **how to write and read messages on Thunderbird storage in Python**.

*   [Python Library to Write and Read Messages on Thunderbird][3]
*   [Write Messages on Thunderbird Storage][4]
*   [Read Messages from Thunderbird Storage][5]

## Python Library to Write and Read Messages on Thunderbird Storage {#Python-Library-to-Write-and-Read-Messages-on-Thunderbird}

To write and read email messages on Thunderbird storage, we will use [Aspose.Email for Python via .NET][6]. It is a powerful library that lets you create and send emails and work with popular email clients such as Thunderbird, Outlook, etc. You can install the library from [PyPI][7] using the following command.

```
> pip install Aspose.Email-for-Python-via-NET
```

## Write a Message on Thunderbird Storage in Python {#Write-Messages-on-Thunderbird}

You can create new messages and store them on Thunderbird's storage within a few steps using Aspose.Email for Python. The following are the steps to perform this operation.

*   Create an instance of **MboxrdStorageWriter** and initialize it with the file name.
*   Create a new **MailMessage** and set its properties.
*   Write message to storage using **MboxrdStorageWriter.write\_message(MailMessage)** method.
*   Dispose of the writer.

The following code sample shows how to write a message to Thunderbird storage in Python.

{{< gist aspose-com-gists 02d9c6c226b8836d8b8a2a8bb6b80ef7 "write-message-thunderbird.py" >}}

## Read Messages from Thunderbird Storage in Python {#Read-Messages-from-Thunderbird}

To read the messages from Thunderbird storage, we need to load the storage file using **MboxrdStorageReader** class. The following are the steps to read messages from Thunderbird in Python.

*   Create an instance of **MboxrdStorageReader** to read the storage file.
*   Read first message using **MboxrdStorageReader.read\_next\_message()** method.
*   Start a loop to iterate through all the messages.
*   Read each message and save it on disk if required.
*   Dispose of the reader at the end.

The following code sample shows how to read messages from Thunderbird storage in Python.

{{< gist aspose-com-gists 02d9c6c226b8836d8b8a2a8bb6b80ef7 "read-message-thunderbird.py" >}}

## Get a Free API License

You can use Aspose.Email for Python via .NET by getting a [free temporary license][8].

## Conclusion

Thunderbird is an amazing email client application to configure multiple email accounts at a single location. In this article, you have learned how to write messages to Thunderbird storage in Python. Moreover, you have seen how to read messages from Thunderbird storage programmatically. Besides, you can visit the [documentation][9] to explore other features of Aspose.Email for Python. In case you would have any questions, you can post to our [forum][10].

## See Also

*   [Send Emails in Python – Python Email API][11]




[1]: https://en.wikipedia.org/wiki/Mozilla_Thunderbird
[2]: https://en.wikipedia.org/wiki/Mozilla_Thunderbird
[3]: #Python-Library-to-Write-and-Read-Messages-on-Thunderbird
[4]: #Write-Messages-on-Thunderbird
[5]: #Read-Messages-from-Thunderbird
[6]: https://products.aspose.com/email/python-net
[7]: https://pypi.org/project/Aspose.Email-for-Python-via-NET/
[8]: https://products.aspose.com/email
[9]: https://docs.aspose.com/email/python-net
[10]: https://forum.aspose.com/
[11]: https://blog.aspose.com/2021/05/21/send-emails-in-python/




