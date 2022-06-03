---
title: 'Create MS Outlook Distribution Lists in Python'
date: Mon, 18 Apr 2022 17:26:35 +0000
draft: false
url: /2022/04/18/create-ms-outlook-distribution-lists-in-python/
author: 'Usman Aziz'
summary: 'MS Outlook allows creating the distribution lists to send emails to multiple people without writing individual email addresses. Furthermore, you can create different lists based on types of people such as official, social, etc. While working with MS Outlook programmatically, you can create and save a distribution list on disk in [PST][1] format. This PST file can be loaded and utilized in MS Outlook or from within your application. In this article, you will learn **how to create MS Outlook distribution lists in Python**.'
tags: ['Create a Distribution List in MS Outlook in Python', 'Python Library to Create MS Outlook Distribution Lists', 'Python Outlook Library']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Users.png" alt="Create Outlook Distribution Lists in Python">}}


[MS Outlook][2] allows creating the distribution lists to send emails to multiple people without writing individual email addresses. Furthermore, you can create different lists based on types of people such as official, social, etc. While working with MS Outlook programmatically, you can create and save a distribution list on disk in [PST][3] format. This PST file can be loaded and utilized in MS Outlook or from within your application. In this article, you will learn **how to create MS Outlook distribution lists in Python**.

*   [Python Library to Create MS Outlook Distribution Lists][4]
*   [Create a Distribution List in MS Outlook][5]

## Python Library to Create MS Outlook Distribution Lists {#Python-Library-to-Create-MS-Outlook-Distribution-Lists}

To create Outlook distribution lists from within Python applications, we will use [Aspose.Email for Python via .NET][6]. It is a feature-rich library that lets you create and send emails and work with popular email clients seamlessly. You can install it using the following command.

```
> pip install Aspose.Email-for-Python-via-NET
```

_(Download a complete package of source code samples from [GitHub][7].)_

## Create a Distribution List in MS Outlook in Python {#Create-a-Distribution-List-in-MS-Outlook}

Let's see how to create a distribution list in MS Outlook programmatically using Aspose.Email for Python.

*   First, create string objects to store details of the members.
*   Then, create a PST file using the **PersonalStorage.create()** method to store the distribution list.
*   After that, make a new folder in PST using **PersonalStorage.create\_predefined\_folder()** method and set its name.
*   Then, create a **MapiDistributionListMember** object for each member and initialize it.
*   Create a new **MapiDistributionListMemberCollection** object and add members to it.
*   Assign the collection to a **MapiDistributionList** object.
*   Finally, add a distribution list to the folder of PST using the **add\_mapi\_message\_item()** method.

The following code sample shows how to create an MS Outlook distribution list in Python.

{{< gist aspose-com-gists aaf32c39df10712c3958c113b95f11bb "create-outlook-distribution-list.py" >}}

## Get a Free API License

You can use Aspose.Email for Python via .NET by requesting a [free temporary license][8].

## Conclusion

The distribution lists in MS Outlook make it easier to send an email to a collection of people. You can create as many lists as required based on the type of recipients. In this article, you have learned how to create MS Outlook distribution lists programmatically in Python. You can simply install Aspose.Email and integrate the provided code sample into your Python applications. In addition, you can explore more about the Python email API using the [documentation][9]. Furthermore, you can post your questions on our [forum][10].

## See Also

*   [Send Emails in Python – Python Email API][11]




[1]: https://docs.fileformat.com/email/pst/
[2]: https://en.wikipedia.org/wiki/Microsoft_Outlook
[3]: https://docs.fileformat.com/email/pst/
[4]: #Python-Library-to-Create-MS-Outlook-Distribution-Lists
[5]: #Create-a-Distribution-List-in-MS-Outlook
[6]: https://products.aspose.com/email/python-net
[7]: https://github.com/aspose-email/Aspose.Email-Python-Dotnet
[8]: https://products.aspose.com/email
[9]: https://docs.aspose.com/email/python-net
[10]: https://forum.aspose.com/
[11]: https://blog.aspose.com/2021/05/21/send-emails-in-python/




