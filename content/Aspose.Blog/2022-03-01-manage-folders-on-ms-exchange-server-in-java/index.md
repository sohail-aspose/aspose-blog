---
title: 'Create and Delete Folders on MS Exchange Server in Java'
date: Tue, 01 Mar 2022 00:08:00 +0000
draft: false
url: /2022/03/01/manage-folders-on-ms-exchange-server-in-java/
author: 'Usman Aziz'
summary: '[Microsoft Exchange Server](https://en.wikipedia.org/wiki/Microsoft_Exchange_Server) keeps emails in different folders such as inbox, outbox, etc. In addition, it allows you to create your own folders or subfolders inside the predefined folders. In certain cases, you may need to create custom folders on Exchange Server programmatically. To accomplish that, this article covers **how to create or delete folders or subfolders with EWS on MS Exchange Server in Java**.'
tags: ['Create a Folder on MS Exchange Server Java', 'Create a Subfolder on MS Exchange Server Java', 'Delete a Folder on MS Exchange Server Java', 'Java API to Create Folders with EWS on MS Exchange Server']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Create and Delete Folders on MS Exchange Server in Java">}}


[Microsoft Exchange Server](https://en.wikipedia.org/wiki/Microsoft_Exchange_Server) keeps emails in different folders such as inbox, outbox, etc. In addition, it allows you to create your own folders or subfolders inside the predefined folders. In certain cases, you may need to create custom folders on Exchange Server programmatically. To accomplish that, this article covers **how to create or delete folders or subfolders with EWS on MS Exchange Server in Java**.

*   [Java API to Create Folders with EWS on MS Exchange Server](#API-to-Create-Folders-in-MS-Exchange-Server)
*   [Create a Folder on MS Exchange Server](#Create-a-Folder-on-MS-Exchange-Server)
*   [Create a Subfolder on MS Exchange Server](#Create-a-Subfolder-on-MS-Exchange-Server)
*   [Delete a Folder on MS Exchange Server](#Delete-a-Folder-on-MS-Exchange-Server)

## Java API to Create Folders on MS Exchange Server {#API-to-Create-Folders-in-MS-Exchange-Server}

To work with folders on MS Exchange Server using EWS, we will utilize [Aspose.Email for Java](https://products.aspose.com/email/net/). It is a powerful API to work with the Exchange Server's services from within Java applications. You can either [download](https://downloads.aspose.com/email/java/) the API or install it using the following Maven configurations.

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

*   Connect to MS Exchange Server and get the EWS client object in [IEWSClient](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient).
*   Specify the name of the root folder and the folder you want to create.
*   Create folder using [IEWSClient.createFolder(String, String)](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#createFolder(java.lang.String,%20java.lang.String)) method.

The following code sample shows how to create a folder on MS Exchange Server with EWS in Java.

\[gist id="21cb4c6bb9e8748dcd7e5a15cd1c9e4c" file="create-folder.java"\]

## Create a Subfolder on MS Exchange Server in Java {#Create-a-Subfolder-on-MS-Exchange-Server}

To create a subfolder, you would first need to check if the parent folder exists or not. If it does, simply create the subfolder, else create the parent folder first. The following steps demonstrate how to create a subfolder on MS Exchange Server in Java.

*   Connect to MS Exchange Server and get the EWS client object in [IEWSClient](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient).
*   Specify the name of the root folder and subfolder.
*   Check if the parent folder exists using [IEWSClient.folderExists(String, String)](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#folderExists(java.lang.String,%20java.lang.String)) method. If it doesn't, create one.
*   Create subfolder using [IEWSClient.createFolder(String, String)](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#createFolder(java.lang.String,%20java.lang.String)) method.

The following code sample shows how to create a subfolder on MS Exchange Server in Java.

\[gist id="21cb4c6bb9e8748dcd7e5a15cd1c9e4c" file="create-subfolder.java"\]

## Delete a Folder on MS Exchange Server in Java {#Delete-a-Folder-on-MS-Exchange-Server}

The following are the steps to delete a folder on MS Exchange Server in Java.

*   Connect to MS Exchange Server and get the EWS client object in [IEWSClient](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient).
*   Check if the folder exists using [IEWSClient.folderExists(String, String, ExchangeFolderInfo\[\])](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#folderExists(java.lang.String,%20java.lang.String,%20com.aspose.email.ExchangeFolderInfo[])) method.
*   Delete folder using [IEWSClient.deleteFolder(String, boolean)](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#deleteFolder(java.lang.String,%20boolean)) method.

The following code sample shows how to delete a folder on MS Exchange Server in Java.

\[gist id="21cb4c6bb9e8748dcd7e5a15cd1c9e4c" file="delete-folder.java"\]

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license](https://purchase.aspose.com/temporary-license) to use Aspose.Email for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to work with folders on Microsoft Exchange Server with EWS in Java. You have seen how to create and delete a particular folder on MS Exchange Server programmatically in Java. In addition, you can learn more about Aspose.Email for Java from the [documentation](https://docs.aspose.com/email/java/). In case you would have any queries, you can post them to our [forum](https://forum.aspose.com/).

## See Also

*   [Read Emails from MS Exchange Server in Java](https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/)



