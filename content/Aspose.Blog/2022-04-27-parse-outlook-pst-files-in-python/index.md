---
title: 'Parse Outlook PST Files in Python'
seoTitle: "Parse Outlook PST Files in Python | Extract Messages and Contacts"
description: "Use Python email processing library to parse PST files in Python. Extract messages and contacts from PST files programmatically in Python."
date: Wed, 27 Apr 2022 16:34:38 +0000
draft: false
url: /2022/04/27/parse-outlook-pst-files-in-python/
author: Usman Aziz
summary: '[PST (Personal Storage Table)][1] is a storage file format that is used by different Microsoft programs. PST files are capable of keeping data of messages, contacts, calendars, events, etc. It is used by popular Microsoft softwares such as MS Outlook, Exchange, and Windows Messaging. In certain cases, you may need to parse a PST file and extract data from it programmatically. To achieve that, this article shows **how to parse PST files from within the Python applications**.'
tags: ['Extract Contacts from a PST File in Python', 'Extract Messages from a PST File in Python', 'Parse a PST File in Python', 'Python Library to Parse PST Files']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Parse-Outlook-PST-Files.png" alt="Parse Outlook PST Files in Python">}}


[PST (Personal Storage Table)][2] is a storage file format that is used by different Microsoft programs. PST files are capable of keeping data of messages, contacts, calendars, events, etc. It is used by popular Microsoft softwares such as MS Outlook, Exchange, and Windows Messaging. In certain cases, you may need to parse a PST file and extract data from it programmatically. To achieve that, this article shows **how to parse PST files from within the Python applications**.

*   [Python Library to Parse PST Files][3]
*   [Parse a PST File in Python][4]
*   [Extract Messages from a PST File][5]
*   [Extract Contacts from a PST File][6]

## Python Library to Parse PST Files {#Python-Library-to-Parse-PST-Files}

In order to parse PST files, we will use [Aspose.Email for Python][7]. It is a powerful Python library that lets you implement feature-rich email clients seamlessly. Furthermore, it allows you to work with popular email and storage formats. You can install the library from [PyPI][8] using the following command.

```
> pip install Aspose.Email-for-Python-via-NET
```

## Parse a PST File in Python {#Parse-a-PST-File-in-Python}

The following are the steps to parse a PST file and extract its information in Python.

*   Load the PST file using **PersonalStorage.from\_file()** method.
*   Get the folders collection in PST using **PersonalStorage.root\_folder.get\_sub\_folders()** method.
*   Retrieve the information of the folders such as name, number of items, etc.

The following code sample shows how to parse a PST file and fetch folders' information.

{{< gist aspose-com-gists 1d9204a42d1674c51aab2a3db41be12f "parse-pst.py" >}}

## Extract Messages from a PST File in Python {#Extract-Messages-from-a-PST-File}

Messages are the major entities that are stored in PST files by Microsoft programs such as MS Outlook. So let's see how to extract messages from a PST file in Python.

*   Load the PST file using **PersonalStorage.from\_file()** method.
*   Get the reference of the desired folder in an object using **PersonalStorage.root\_folder.get\_sub\_folder()** method.
*   Get message collection using **get\_contents()** method.
*   Loop through the messages in the collection and read each message's fields.

The following code sample shows how to extract messages from a PST file in Python.

{{< gist aspose-com-gists 1d9204a42d1674c51aab2a3db41be12f "extract-messages.py" >}}

## Extract Contacts from a PST File in Python {#Extract-Contacts-in-a-PST-File}

In certain cases, you may need to extract the contacts' information stored in a PST file. The following steps show how to access the contacts in a PST file in Python.

*   Load the PST file using **PersonalStorage.from\_file()** method.
*   Get reference of the contacts folder using **get\_predefined\_folder(StandardIpmFolder.CONTACTS)** method.
*   Get collection of contacts using **get\_contents()** method.
*   Loop through the collection and read each contact or save it.

The following code sample shows how to extract contacts from a PST file in Python.

{{< gist aspose-com-gists 1d9204a42d1674c51aab2a3db41be12f "extract-contacts.py" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try Aspose.Email for Python for free by [getting a temporary license][9].

## Conclusion

In this article, you have learned how to parse PST files in Python. Furthermore, you have seen how to extract contacts and messages from a PST file programmatically in Python. In addition, you can explore more about Aspose.Email using [documentation][10]. Also, you can share your questions or queries on our [forum][11].

## See Also

*   [Send Emails in Python - Python Email API][12]




[1]: https://docs.fileformat.com/email/pst/
[2]: https://docs.fileformat.com/email/pst/
[3]: #Python-Library-to-Parse-PST-Files
[4]: #Parse-a-PST-File-in-Python
[5]: #Extract-Messages-from-a-PST-File
[6]: #Extract-Contacts-in-a-PST-File
[7]: https://products.aspose.com/email/python-net
[8]: https://pypi.org/project/Aspose.Email-for-Python-via-NET/
[9]: https://purchase.aspose.com/temporary-license
[10]: https://docs.aspose.com/email/python-net/
[11]: https://forum.aspose.com/
[12]: https://blog.aspose.com/2021/05/21/send-emails-in-python/




