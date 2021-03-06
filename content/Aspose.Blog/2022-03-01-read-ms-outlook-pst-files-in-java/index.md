---
title: 'Read MS Outlook PST Files in Java'
seoTitle: "Read MS Outlook PST Files in Java | Read Emails and Contacts in Java"
description: "Use Java email processing library to parse PST files in Java. Extract emails and contacts from PST files programmatically in Java."
date: Tue, 01 Mar 2022 17:54:00 +0000
draft: false
url: /2022/03/01/read-ms-outlook-pst-files-in-java/
author: Usman Aziz
summary: "[PST (Personal Storage Table)][1] is a well-known file format that is used for storage purposes by different Microsoft programs such as MS Outlook, Exchange, and Windows Messaging. PST files can store messages, contacts, and information about other items such as calendars, events, etc. In certain cases, you may need to parse a PST file and extract data from it programmatically. To achieve that, this article shows **how to read MS Outlook PST files using Java**. You will learn how to extract folders' information, read emails and fetch contacts from a PST file."
tags: ['Extract Contacts from a PST File in Java', 'Java API to Read PST Files', 'Read Emails from a PST File in Java', 'Read an Outlook PST File in Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Parse-Outlook-PST-Files.png" alt="Read MS Outlook PST Files in Java">}}


[PST (Personal Storage Table)][2] is a well-known file format that is used for storage purposes by different Microsoft programs such as MS Outlook, Exchange, and Windows Messaging. PST files can store messages, contacts, and information about other items such as calendars, events, etc. In certain cases, you may need to parse a PST file and extract data from it programmatically. To achieve that, this article shows **how to read MS Outlook PST files using Java**. With the help of code samples, you will learn how to extract folders' information, read emails and fetch contacts from a PST file.

*   [Java API to Read PST Files][3]
*   [Read an Outlook PST File][4]
*   [Read Emails from a PST File][5]
*   [Extract Contacts from a PST File][6]

## Java API to Read Outlook PST Files {#API-to-Parse-PST-Files}

[Aspose.Email for Java][7] is a popular and feature-rich email processing API for creating and sending emails. In addition, it allows you to work with popular email clients and storage file formats. In this article, we will use Aspose.Email for Java to read messages and other information from PST files. You can either??[download][8]??the API or install it using the following Maven configurations.

```
**Repository:**
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>

**Dependency:**
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-email</artifactId>
    <version>22.3</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Read an Outlook PST File in Java {#Parse-a-PST-File}

The following are the steps to read a PST file and extract its information.

*   Load the PST file using [PersonalStorage.fromFile()][9] method.
*   Get the folders collection in PST using [PersonalStorage.getRootFolders().getSubFolders()][10] method.
*   Retrieve the information of the folders such as name, number of items, etc.

The following code sample shows how to read a PST file and fetch folders' information.

{{< gist aspose-com-gists f41f10fa8737347ab9300d8b675d3da6 "read-pst.java" >}}

## Read Emails from a PST File in Java {#Extract-Messages-from-a-PST-File}

The following are the steps to read email messages from a PST file in Java.

*   Load the PST file using [PersonalStorage.fromFile()][11] method.
*   Access the root folder using [PersonalStorage.getRootFolder()][12] method.
*   Get message collection from each subfolder using [FolderInfo.getContents()][13] method.
*   Loop through the messages in the collection and read each message's fields.

The following code sample shows how to extract messages from a PST file in Java.

{{< gist aspose-com-gists f41f10fa8737347ab9300d8b675d3da6 "read-emails.java" >}}

## Extract Contacts from a PST File in Java {#Extract-Contacts-in-a-PST-File}

In certain cases, you may need to extract the contacts' information stored in a PST file. The following steps show how to access the contacts in a PST file in Java.

*   Load the PST file using [PersonalStorage.fromFile()][14] method.
*   Get reference of the contacts folder using [PersonalStorage.getRootFolder().getSubFolder("Contacts")][15] method.
*   Get collection of contacts using [FolderInfo.getContents()][16] method.
*   Loop through the contacts collection and read each contact or save it.

The following code sample shows how to extract contacts from a PST file in Java.

{{< gist aspose-com-gists f41f10fa8737347ab9300d8b675d3da6 "extract-contacts.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try Aspose.Email for Java for free by??[getting a temporary license][17].

## Conclusion

In this article, you have learned how to read PST files programmatically in Java. Furthermore, you have seen how to extract folder information, fetch emails, and retrieve contacts from a PST file in Java. In addition, you can explore more about Aspose.Email for Java using [documentation][18]. Also, in case you would have any questions or queries, feel free to let us know via our [forum][19].

## See Also

*   [Read Emails from Exchange Server in Java][20]




[1]: https://docs.fileformat.com/email/pst/
[2]: https://docs.fileformat.com/email/pst/
[3]: #API-to-Parse-PST-Files
[4]: #Parse-a-PST-File
[5]: #Extract-Messages-from-a-PST-File
[6]: #Extract-Contacts-in-a-PST-File
[7]: https://products.aspose.com/email/java/
[8]: https://downloads.aspose.com/email/java/
[9]: https://apireference.aspose.com/email/java/com.aspose.email/PersonalStorage#fromFile(java.lang.String)
[10]: https://apireference.aspose.com/email/java/com.aspose.email/FolderInfo#getSubFolders()
[11]: https://apireference.aspose.com/email/java/com.aspose.email/PersonalStorage#fromFile(java.lang.String)
[12]: https://apireference.aspose.com/email/java/com.aspose.email/PersonalStorage#getRootFolder()
[13]: https://apireference.aspose.com/email/java/com.aspose.email/FolderInfo#getContents()
[14]: https://apireference.aspose.com/email/java/com.aspose.email/PersonalStorage#fromFile(java.lang.String)
[15]: https://apireference.aspose.com/email/java/com.aspose.email/FolderInfo#getSubFolder(java.lang.String)
[16]: https://apireference.aspose.com/email/java/com.aspose.email/FolderInfo#getContents()
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/email/java/
[19]: https://forum.aspose.com/
[20]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/




