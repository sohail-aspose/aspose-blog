---
title: 'Create MS Outlook Distribution Lists in Java'
date: Fri, 06 May 2022 17:06:00 +0000
draft: false
url: /2022/05/06/create-ms-outlook-distribution-lists-in-java/
author: ''Usman Aziz''
summary: "Email distribution lists make it possible to send emails to a group of people without writing individual email addresses. You can create a number of lists based on types of people such as official, social, etc. [MS Outlook][1] also allows you to make the distribution lists and often you may need to create such lists programmatically. So let's see **how to create and read MS Outlook distribution lists programmatically in Java**."
tags: ['Create a Distribution List in MS Outlook in Java', 'Java API to Create MS Outlook Distribution Lists', 'Java MS Outlook Library', 'Read an MS Outlook Distribution List in Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Users.png" alt="Create Outlook Distribution Lists in Java">}}


Email distribution lists make it possible to send emails to a group of people without writing individual email addresses. You can create a number of lists based on types of people such as official, social, etc. [MS Outlook][2] also allows you to make the distribution lists and often you may need to create such lists programmatically. So let's see **how to create and read MS Outlook distribution lists programmatically in Java**.

*   [Java API to Create MS Outlook Distribution Lists][3]
*   [Create a Distribution List in MS Outlook][4]
*   [Read an MS Outlook Distribution List][5]

## Java API to Create MS Outlook Distribution Lists {#API-to-Create-MS-Outlook-Distribution-Lists}

[Aspose.Email for Java][6] is an amazing API to work with emails. It lets you create, send, and process emails and work with various email clients including MS Outlook. We will use this API to create and read the Outlook distribution lists in this article. You can either [download][7] the API or install it using the following Maven configurations.

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

## Create a Distribution List in MS Outlook in Java {#Create-a-Distribution-List-in-MS-Outlook}

MS Outlook uses [PST][8] format to store the information about the distribution lists. Let's see how to create a distribution list in MS Outlook programmatically using Aspose.Email for Java.

*   First, create string objects to store details of the members.
*   Then, create a PST file using the [PersonalStorage.create()][9] method to store the distribution list.
*   After that, make a new folder in PST using [PersonalStorage.createPredefinedFolder()][10] method and set its name.
*   Then, create a [MapiDistributionListMember][11] object for each member and initialize it.
*   Create a new [MapiDistributionListMemberCollection][12] object and add members to it.
*   Assign the collection to a [MapiDistributionList][13] object.
*   Finally, add a distribution list to the folder of PST using the [FolderInfo.addMapiMessageItem()][14] method.

The following code sample shows how to create an MS Outlook distribution list in Java.

{{< gist aspose-com-gists 118c50bf438492723e2474e9eb1bce62 "create-outlook-distribution-list.java" >}}

## Read an MS Outlook Distribution List in Java {#Read-an-MS-Outlook-Distribution-List}

You can also read an Outlook distribution list and fetch the contacts' information. The following steps show how to perform this operation.

*   Load the distribution list from the PST file using [MapiMessage.load()][15] method.
*   Fetch the list using [MapiMessage.toMapiMessageItem()][16] method and cast it to [MapiDistributionList][17].
*   Read the contacts from the _MapiDistributionList_ object.

The following code sample shows how to read an MS Outlook distribution list in Java.

{{< gist aspose-com-gists 118c50bf438492723e2474e9eb1bce62 "read-outlook-distribution-list.java" >}}

## Get a Free API License

You can use Aspose.Email for Java without evaluation limitations by getting a [free temporary license][18].

## Conclusion

A distribution list in MS Outlook lets you send an email to a group of people. In this article, you have learned how to create MS Outlook distribution lists in Java. Furthermore, you have seen how to read the Outlook distribution lists programmatically. Besides, you can explore more about the Java email API using the [documentation][19]. Also, you can post your questions or queries on our [forum][20].

## See Also

*   [Create Exchange Distribution List in Java][21]




[1]: https://en.wikipedia.org/wiki/Microsoft_Outlook
[2]: https://en.wikipedia.org/wiki/Microsoft_Outlook
[3]: #API-to-Create-MS-Outlook-Distribution-Lists
[4]: #Create-a-Distribution-List-in-MS-Outlook
[5]: #Read-an-MS-Outlook-Distribution-List
[6]: https://products.aspose.com/email/java/
[7]: https://downloads.aspose.com/email/java/
[8]: https://docs.fileformat.com/email/pst/
[9]: https://apireference.aspose.com/email/java/com.aspose.email/PersonalStorage#create(java.io.OutputStream,%20int)
[10]: https://apireference.aspose.com/email/java/com.aspose.email/PersonalStorage#createPredefinedFolder(java.lang.String,%20int)
[11]: https://apireference.aspose.com/email/java/com.aspose.email/MapiDistributionListMember
[12]: https://apireference.aspose.com/email/java/com.aspose.email/MapiDistributionListMemberCollection
[13]: https://apireference.aspose.com/email/java/com.aspose.email/MapiDistributionList
[14]: https://apireference.aspose.com/email/java/com.aspose.email/FolderInfo#addMapiMessageItem(com.aspose.email.IMapiMessageItem)
[15]: https://apireference.aspose.com/email/java/com.aspose.email/MapiMessage#load(java.lang.String)
[16]: https://apireference.aspose.com/email/java/com.aspose.email/MapiMessage#toMapiMessageItem()
[17]: https://apireference.aspose.com/email/java/com.aspose.email/MapiDistributionList
[18]: https://products.aspose.com/email
[19]: https://docs.aspose.com/email/java/
[20]: https://forum.aspose.com/
[21]: https://blog.aspose.com/2022/04/07/create-exchange-distribution-list-in-java/




