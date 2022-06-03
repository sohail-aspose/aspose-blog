---
title: 'Create and Update Folders using Microsoft Graph API in Java'
date: Thu, 14 Apr 2022 14:44:47 +0000
draft: false
url: /2022/04/14/manage-folders-with-microsoft-graph-api-java/
author: 'Usman Aziz'
summary: 'Microsoft provides [Graph API](https://en.wikipedia.org/wiki/Microsoft_Graph) to interact and work with Office 365 and Microsoft Cloud services. It allows you to create and manage folders, access messages, manage categories and use other services programmatically. In this article, you will learn **how to use Microsoft Graph API to create and update folders in Java**.'
tags: ['Create Folders using Microsoft Graph API Java', 'Create a Subfolder using Microsoft Graph API Java', 'Java Microsoft Graph API to Manage Folders', 'Update Folders using Microsoft Graph API Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Using-Microsoft-Graph-API-1024x542.jpg" alt="Create and Update Folders using Microsoft Graph API in Java">}}


Microsoft provides [Graph API](https://en.wikipedia.org/wiki/Microsoft_Graph) to interact and work with Office 365 and Microsoft Cloud services. It allows you to create and manage folders, access messages, manage categories and use other services programmatically. In this article, you will learn **how to use Microsoft Graph API to create and update folders in Java**.

*   [Java Microsoft Graph API to Manage Folders](#Java-Microsoft-Graph-API-to-Manage-Folders)
*   [Create Folders using Microsoft Graph API](#Create-Folders-using-Microsoft-Graph-API)
*   [Create a Subfolder using Microsoft Graph API](#Create-a-Subfolder-using-Microsoft-Graph-API)
*   [Update Folders using Microsoft Graph API](#Update-Folders-using-Microsoft-Graph-API)

## Java Microsoft Graph API to Manage Folders {#Java-Microsoft-Graph-API-to-Manage-Folders}

To create and update folders using Microsoft Graph API, we will use [Aspose.Email for Java](https://products.aspose.com/email/java/). The API makes it quite easier to seamlessly work with Office 365 services using Microsoft Graph API. You can either [download](https://downloads.aspose.com/email/java/) the API or install it using the following Maven configurations.

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

## Create a Folder using Microsoft Graph API in Java {#Create-Folders-using-Microsoft-Graph-API}

To communicate with the Graph API, you need to first implement the [ITokenProvider](https://apireference.aspose.com/email/java/com.aspose.email/ITokenProvider) interface for authenticating the requests. The following is the basic implementation of _ITokenProvider_.

{{< gist aspose-com-gists e9851d09ebd67ccd725fa01a8ed0daef "TokenProvider.java" >}}

The following are the steps to create a folder using Microsoft Graph API in Java.

*   First, get an instance of Microsoft Graph client using [GraphClient.getClient(ITokenProvider)](https://apireference.aspose.com/email/java/com.aspose.email/GraphClient#getClient(com.aspose.email.ITokenProvider)) method.
*   Then, call [IGraphClient.createFolder(String)](https://apireference.aspose.com/email/java/com.aspose.email/IGraphClient#createFolder(java.lang.String)) method to create the folder.

The following code sample shows how to create a folder using Microsoft Graph API in Java.

{{< gist aspose-com-gists e9851d09ebd67ccd725fa01a8ed0daef "create-folder.java" >}}

## Create a Subfolder using Microsoft Graph API in Java {#Create-a-Subfolder-using-Microsoft-Graph-API}

You can also create a subfolder in a similar way. The only difference is that you have to provide the root folder's path as the first argument of the _createFolder_ method. The following code sample shows how to create a subfolder using Microsoft Graph API in Java.

{{< gist aspose-com-gists e9851d09ebd67ccd725fa01a8ed0daef "create-subfolder.java" >}}

## Update Folders using Microsoft Graph API in Java {#Update-Folders-using-Microsoft-Graph-API}

You can also fetch and update an existing folder using Microsoft Graph API. For this, you have to get the list of folders and filter the required one. The following are the steps to update a folder using Aspose.Email for Java.

*   First, get instance of Microsoft Graph client using [GraphClient.getClient(ITokenProvider)](https://apireference.aspose.com/email/java/com.aspose.email/GraphClient#getClient(com.aspose.email.ITokenProvider)) method.
*   Then, get list of all folders using [IGraphClient.listFolders()](https://apireference.aspose.com/email/java/com.aspose.email/IGraphClient#listFolders()) method.
*   After that, loop through all the [GraphFolderInfo](https://apireference.aspose.com/email/java/com.aspose.email/GraphFolderInfo) objects in the list and fetch the required one.
*   Then, use _GraphFolderInfo_ object to update the folder's properties.
*   Finally, update the folder using [IGraphClient.updateFolder(GraphFolderInfo)](https://apireference.aspose.com/email/java/com.aspose.email/IGraphClient#updateFolder(com.aspose.email.GraphFolderInfo)) method.

The following code sample shows how to update a folder using Microsoft Graph API in Java.

{{< gist aspose-com-gists e9851d09ebd67ccd725fa01a8ed0daef "update-folder.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license](https://purchase.aspose.com/temporary-license) to use Aspose.Email for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to work with folders using Microsoft Graph API from within Java applications. Particularly, you have seen how to create or update a folder/subfolder with Microsoft Graph API in Java. Besides, you can explore other features of Aspose.Email for Java using the [documentation](https://docs.aspose.com/email/java/). Also, in case you would have any questions, you can post to our [forum](https://forum.aspose.com/).

## See Also

*   [Read Emails from MS Exchange Server in Java](https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/)




