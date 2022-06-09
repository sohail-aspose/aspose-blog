---
title: 'Create and Delete Folders on MS Exchange Server in Java'
seoTitle: "Java Create and Delete Folders with EWS on Exchange Server | Java API"
description: "Use Java EWS API to work with folders on MS Exchange Server in Java. Create and delete the folders using the EWS client on MS Exchange Server."
date: Tue, 01 Mar 2022 00:08:00 +0000
draft: false
url: /2022/03/01/manage-folders-on-ms-exchange-server-in-java/
author: Usman Aziz
summary: '[Microsoft Exchange Server][1] keeps emails in different folders such as inbox, outbox, etc. In addition, it allows you to create your own folders or subfolders inside the predefined folders. In certain cases, you may need to create custom folders on Exchange Server programmatically. To accomplish that, this article covers **how to create or delete folders or subfolders with EWS on MS Exchange Server in Java**.'
tags: ['Create a Folder on MS Exchange Server Java', 'Create a Subfolder on MS Exchange Server Java', 'Delete a Folder on MS Exchange Server Java', 'Java API to Create Folders with EWS on MS Exchange Server']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Create and Delete Folders on MS Exchange Server in Java">}}


[Microsoft Exchange Server][2] keeps emails in different folders such as inbox, outbox, etc. In addition, it allows you to create your own folders or subfolders inside the predefined folders. In certain cases, you may need to create custom folders on Exchange Server programmatically. To accomplish that, this article covers **how to create or delete folders or subfolders with EWS on MS Exchange Server in Java**.

*   [Java API to Create Folders with EWS on MS Exchange Server][3]
*   [Create a Folder on MS Exchange Server][4]
*   [Create a Subfolder on MS Exchange Server][5]
*   [Delete a Folder on MS Exchange Server][6]

## Java API to Create Folders on MS Exchange Server {#API-to-Create-Folders-in-MS-Exchange-Server}

To work with folders on MS Exchange Server using EWS, we will utilize [Aspose.Email for Java][7]. It is a powerful API to work with the Exchange Server's services from within Java applications. You can either [download][8] the API or install it using the following Maven configurations.

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
    <version>22.2</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Create a Folder on MS Exchange Server in Java {#Create-a-Folder-on-MS-Exchange-Server}

The following are the steps to create a folder on MS Exchange Server in Java.

*   Connect to MS Exchange Server and get the EWS client object in [IEWSClient][9].
*   Specify the name of the root folder and the folder you want to create.
*   Create folder using [IEWSClient.createFolder(String, String)][10] method.

The following code sample shows how to create a folder on MS Exchange Server with EWS in Java.

{{< gist aspose-com-gists 21cb4c6bb9e8748dcd7e5a15cd1c9e4c "create-folder.java" >}}

## Create a Subfolder on MS Exchange Server in Java {#Create-a-Subfolder-on-MS-Exchange-Server}

To create a subfolder, you would first need to check if the parent folder exists or not. If it does, simply create the subfolder, else create the parent folder first. The following steps demonstrate how to create a subfolder on MS Exchange Server in Java.

*   Connect to MS Exchange Server and get the EWS client object in [IEWSClient][11].
*   Specify the name of the root folder and subfolder.
*   Check if the parent folder exists using [IEWSClient.folderExists(String, String)][12] method. If it doesn't, create one.
*   Create subfolder using [IEWSClient.createFolder(String, String)][13] method.

The following code sample shows how to create a subfolder on MS Exchange Server in Java.

{{< gist aspose-com-gists 21cb4c6bb9e8748dcd7e5a15cd1c9e4c "create-subfolder.java" >}}

## Delete a Folder on MS Exchange Server in Java {#Delete-a-Folder-on-MS-Exchange-Server}

The following are the steps to delete a folder on MS Exchange Server in Java.

*   Connect to MS Exchange Server and get the EWS client object in [IEWSClient][14].
*   Check if the folder exists using [IEWSClient.folderExists(String, String, ExchangeFolderInfo\[\])][15] method.
*   Delete folder using [IEWSClient.deleteFolder(String, boolean)][16] method.

The following code sample shows how to delete a folder on MS Exchange Server in Java.

{{< gist aspose-com-gists 21cb4c6bb9e8748dcd7e5a15cd1c9e4c "delete-folder.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][17] to use Aspose.Email for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to work with folders on Microsoft Exchange Server with EWS in Java. You have seen how to create and delete a particular folder on MS Exchange Server programmatically in Java. In addition, you can learn more about Aspose.Email for Java from the [documentation][18]. In case you would have any queries, you can post them to our [forum][19].

## See Also

*   [Read Emails from MS Exchange Server in Java][20]




[1]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[2]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[3]: #API-to-Create-Folders-in-MS-Exchange-Server
[4]: #Create-a-Folder-on-MS-Exchange-Server
[5]: #Create-a-Subfolder-on-MS-Exchange-Server
[6]: #Delete-a-Folder-on-MS-Exchange-Server
[7]: https://products.aspose.com/email/net/
[8]: https://downloads.aspose.com/email/java/
[9]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[10]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#createFolder(java.lang.String,%20java.lang.String)
[11]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[12]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#folderExists(java.lang.String,%20java.lang.String)
[13]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#createFolder(java.lang.String,%20java.lang.String)
[14]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[15]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#folderExists(java.lang.String,%20java.lang.String,%20com.aspose.email.ExchangeFolderInfo[])
[16]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#deleteFolder(java.lang.String,%20boolean)
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/email/java/
[19]: https://forum.aspose.com/
[20]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/




