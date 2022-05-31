---
title: 'Parse Outlook PST Files in Python'
date: Wed, 27 Apr 2022 16:34:38 +0000
draft: false
url: /2022/04/27/parse-outlook-pst-files-in-python/
author: 'Usman Aziz'
summary: '[PST (Personal Storage Table)](https://docs.fileformat.com/email/pst/) is a storage file format that is used by different Microsoft programs. PST files are capable of keeping data of messages, contacts, calendars, events, etc. It is used by popular Microsoft softwares such as MS Outlook, Exchange, and Windows Messaging. In certain cases, you may need to parse a PST file and extract data from it programmatically. To achieve that, this article shows **how to parse PST files from within the Python applications**.'
tags: ['Extract Contacts from a PST File in Python', 'Extract Messages from a PST File in Python', 'Parse a PST File in Python', 'Python Library to Parse PST Files']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Parse-Outlook-PST-Files.png" alt="Parse Outlook PST Files in Python">}}


[PST (Personal Storage Table)](https://docs.fileformat.com/email/pst/) is a storage file format that is used by different Microsoft programs. PST files are capable of keeping data of messages, contacts, calendars, events, etc. It is used by popular Microsoft softwares such as MS Outlook, Exchange, and Windows Messaging. In certain cases, you may need to parse a PST file and extract data from it programmatically. To achieve that, this article shows **how to parse PST files from within the Python applications**.

*   [Python Library to Parse PST Files](#Python-Library-to-Parse-PST-Files)
*   [Parse a PST File in Python](#Parse-a-PST-File-in-Python)
*   [Extract Messages from a PST File](#Extract-Messages-from-a-PST-File)
*   [Extract Contacts from a PST File](#Extract-Contacts-in-a-PST-File)

## Python Library to Parse PST Files {#Python-Library-to-Parse-PST-Files}

In order to parse PST files, we will use [Aspose.Email for Python](https://products.aspose.com/email/python-net). It is a powerful Python library that lets you implement feature-rich email clients seamlessly. Furthermore, it allows you to work with popular email and storage formats. You can install the library from [PyPI](https://pypi.org/project/Aspose.Email-for-Python-via-NET/) using the following command.

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

You can try Aspose.Email for Python for free by [getting a temporary license](https://purchase.aspose.com/temporary-license).

## Conclusion

In this article, you have learned how to parse PST files in Python. Furthermore, you have seen how to extract contacts and messages from a PST file programmatically in Python. In addition, you can explore more about Aspose.Email using [documentation](https://docs.aspose.com/email/python-net/). Also, you can share your questions or queries on our [forum](https://forum.aspose.com/).

## See Also

*   [Send Emails in Python - Python Email API](https://blog.aspose.com/2021/05/21/send-emails-in-python/)




