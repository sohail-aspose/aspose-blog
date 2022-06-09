---
title: 'Create and Update Folders using Microsoft Graph API in Java'
seoTitle: "Create and Update Folders | Java Microsoft Graph API"
description: "Use Microsoft Graph API for Java to create folders programmatically. Fetch and update the folders with Graph API from within Java applications."
date: Thu, 14 Apr 2022 14:44:47 +0000
draft: false
url: /2022/04/14/manage-folders-with-microsoft-graph-api-java/
author: Usman Aziz
summary: 'Microsoft provides [Graph API][1] to interact and work with Office 365 and Microsoft Cloud services. It allows you to create and manage folders, access messages, manage categories and use other services programmatically. In this article, you will learn **how to use Microsoft Graph API to create and update folders in Java**.'
tags: ['Create Folders using Microsoft Graph API Java', 'Create a Subfolder using Microsoft Graph API Java', 'Java Microsoft Graph API to Manage Folders', 'Update Folders using Microsoft Graph API Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Using-Microsoft-Graph-API-1024x542.jpg" alt="Create and Update Folders using Microsoft Graph API in Java">}}


Microsoft provides [Graph API][2] to interact and work with Office 365 and Microsoft Cloud services. It allows you to create and manage folders, access messages, manage categories and use other services programmatically. In this article, you will learn **how to use Microsoft Graph API to create and update folders in Java**.

*   [Java Microsoft Graph API to Manage Folders][3]
*   [Create Folders using Microsoft Graph API][4]
*   [Create a Subfolder using Microsoft Graph API][5]
*   [Update Folders using Microsoft Graph API][6]

## Java Microsoft Graph API to Manage Folders {#Java-Microsoft-Graph-API-to-Manage-Folders}

To create and update folders using Microsoft Graph API, we will use [Aspose.Email for Java][7]. The API makes it quite easier to seamlessly work with Office 365 services using Microsoft Graph API. You can either [download][8] the API or install it using the following Maven configurations.

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

To communicate with the Graph API, you need to first implement the [ITokenProvider][9] interface for authenticating the requests. The following is the basic implementation of _ITokenProvider_.

{{< gist aspose-com-gists e9851d09ebd67ccd725fa01a8ed0daef "TokenProvider.java" >}}

The following are the steps to create a folder using Microsoft Graph API in Java.

*   First, get an instance of Microsoft Graph client using [GraphClient.getClient(ITokenProvider)][10] method.
*   Then, call [IGraphClient.createFolder(String)][11] method to create the folder.

The following code sample shows how to create a folder using Microsoft Graph API in Java.

{{< gist aspose-com-gists e9851d09ebd67ccd725fa01a8ed0daef "create-folder.java" >}}

## Create a Subfolder using Microsoft Graph API in Java {#Create-a-Subfolder-using-Microsoft-Graph-API}

You can also create a subfolder in a similar way. The only difference is that you have to provide the root folder's path as the first argument of the _createFolder_ method. The following code sample shows how to create a subfolder using Microsoft Graph API in Java.

{{< gist aspose-com-gists e9851d09ebd67ccd725fa01a8ed0daef "create-subfolder.java" >}}

## Update Folders using Microsoft Graph API in Java {#Update-Folders-using-Microsoft-Graph-API}

You can also fetch and update an existing folder using Microsoft Graph API. For this, you have to get the list of folders and filter the required one. The following are the steps to update a folder using Aspose.Email for Java.

*   First, get instance of Microsoft Graph client using [GraphClient.getClient(ITokenProvider)][12] method.
*   Then, get list of all folders using [IGraphClient.listFolders()][13] method.
*   After that, loop through all the [GraphFolderInfo][14] objects in the list and fetch the required one.
*   Then, use _GraphFolderInfo_ object to update the folder's properties.
*   Finally, update the folder using [IGraphClient.updateFolder(GraphFolderInfo)][15] method.

The following code sample shows how to update a folder using Microsoft Graph API in Java.

{{< gist aspose-com-gists e9851d09ebd67ccd725fa01a8ed0daef "update-folder.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][16] to use Aspose.Email for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to work with folders using Microsoft Graph API from within Java applications. Particularly, you have seen how to create or update a folder/subfolder with Microsoft Graph API in Java. Besides, you can explore other features of Aspose.Email for Java using the [documentation][17]. Also, in case you would have any questions, you can post to our [forum][18].

## See Also

*   [Read Emails from MS Exchange Server in Java][19]




[1]: https://en.wikipedia.org/wiki/Microsoft_Graph
[2]: https://en.wikipedia.org/wiki/Microsoft_Graph
[3]: #Java-Microsoft-Graph-API-to-Manage-Folders
[4]: #Create-Folders-using-Microsoft-Graph-API
[5]: #Create-a-Subfolder-using-Microsoft-Graph-API
[6]: #Update-Folders-using-Microsoft-Graph-API
[7]: https://products.aspose.com/email/java/
[8]: https://downloads.aspose.com/email/java/
[9]: https://apireference.aspose.com/email/java/com.aspose.email/ITokenProvider
[10]: https://apireference.aspose.com/email/java/com.aspose.email/GraphClient#getClient(com.aspose.email.ITokenProvider)
[11]: https://apireference.aspose.com/email/java/com.aspose.email/IGraphClient#createFolder(java.lang.String)
[12]: https://apireference.aspose.com/email/java/com.aspose.email/GraphClient#getClient(com.aspose.email.ITokenProvider)
[13]: https://apireference.aspose.com/email/java/com.aspose.email/IGraphClient#listFolders()
[14]: https://apireference.aspose.com/email/java/com.aspose.email/GraphFolderInfo
[15]: https://apireference.aspose.com/email/java/com.aspose.email/IGraphClient#updateFolder(com.aspose.email.GraphFolderInfo)
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/email/java/
[18]: https://forum.aspose.com/
[19]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/




