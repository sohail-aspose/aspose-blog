---
title: 'Create and Send Messages using Microsoft Graph API in Java'
date: Fri, 01 Apr 2022 17:42:00 +0000
draft: false
url: /2022/04/01/create-and-send-messages-using-microsoft-graph-api-in-java/
author: 'Usman Aziz'
summary: '[Microsoft Graph API][1] allows you to access and utilize various services of Office 365 and Microsoft Cloud programmatically. In the [previous article][2], we have shown you how to use Microsoft Graph API to create and update folders. In this article, we will demonstrate **how to create and send messages using Graph API in Java**.'
tags: ['Create Messages using Microsoft Graph API in Java', 'Java Microsoft Graph API', 'Java Microsoft Graph API to Create and Send Messages', 'Send Messages using Microsoft Graph API in Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Using-Microsoft-Graph-API-1024x542.jpg" alt="Create and Send Messages using Microsoft Graph API in Java">}}


[Microsoft Graph API][3] allows you to access and utilize various services of Office 365 and Microsoft Cloud programmatically. In the [previous article][4], we have shown you how to use Microsoft Graph API to create and update folders. In this article, we will demonstrate **how to create and send messages using Graph API in Java**.

*   [Java Microsoft Graph API to Create and Send Messages][5]
*   [Create Messages using Microsoft Graph API in Java][6]
*   [Send Messages using Microsoft Graph API in Java][7]

## Java Microsoft Graph API to Create and Send Messages {#Java-Microsoft-Graph-API-to-Create-and-Send-Messages}

[Aspose.Email for Java][8] provides a range of features to create and process emails. In addition, it allows you to work with Microsoft Outlook, Exchange and Graph API seamlessly. You can either [download][9] the API or install it using the following Maven configurations.

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

## Create Messages using Microsoft Graph API in Java {#Create-Messages-using-Microsoft-Graph-API-in-Java}

To communicate with the Graph API, you need to first implement the [ITokenProvider][10] interface for authenticating the requests. The following is the basic implementation of _ITokenProvider_.

{{< gist aspose-com-gists e9851d09ebd67ccd725fa01a8ed0daef "TokenProvider.java" >}}

The following are the steps to create a message using Microsoft Graph API in Java.

*   First, get an instance of Microsoft Graph client using [GraphClient.getClient(ITokenProvider)][11] method.
*   Then, create an instance of [MapiMessage][12] class.
*   After that, set subject, body, and other properties of the message.
*   Finally, create message in desired folder using [IGraphClient.createMessage(GraphKnownFolders, MapiMessage)][13] method.

The following code sample shows how to create a message using Microsoft Graph API in Java.

{{< gist aspose-com-gists 15c98b166292e7112871f6370c036733 "create-message.java" >}}

## Send Messages using Microsoft Graph API in Java {#Send-Messages-using-Microsoft-Graph-API-in-Java}

Let's now have a look at how to send a message using Microsoft Graph API in Java.

*   First, get an instance of Microsoft Graph client using [GraphClient.getClient(ITokenProvider)][14] method.
*   Then, create an instance of [MapiMessage][15] class.
*   After that, set subject, body, and other properties of the message.
*   Finally, send message using [IGraphClient.send(MapiMessage)][16] method.

The following code sample shows how to send a message using Microsoft Graph API in Java.

{{< gist aspose-com-gists 15c98b166292e7112871f6370c036733 "send-message.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][17] to use Aspose.Email for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to use Microsoft Graph API to create and send messages in Java. You can simply install Aspose.Email and integrate the provided code samples into your Java applications. In addition, you can have a look at other features offered by Aspose.Email for Java using the [documentation][18]. Also, in case you would have any questions, you can post to our [forum][19].

## See Also

*   [Work with Folders using Microsoft Graph API in Java][20]
*   [Read Emails from MS Exchange Server in Java][21]




[1]: https://en.wikipedia.org/wiki/Microsoft_Graph
[2]: https://blog.aspose.com/2022/04/14/manage-folders-with-microsoft-graph-api-java/
[3]: https://en.wikipedia.org/wiki/Microsoft_Graph
[4]: https://blog.aspose.com/2022/04/14/manage-folders-with-microsoft-graph-api-java/
[5]: #Java-Microsoft-Graph-API-to-Create-and-Send-Messages
[6]: #Create-Messages-using-Microsoft-Graph-API-in-Java
[7]: #Send-Messages-using-Microsoft-Graph-API-in-Java
[8]: https://products.aspose.com/email/java/
[9]: https://downloads.aspose.com/email/java/
[10]: https://apireference.aspose.com/email/java/com.aspose.email/ITokenProvider
[11]: https://apireference.aspose.com/email/java/com.aspose.email/GraphClient#getClient(com.aspose.email.ITokenProvider)
[12]: https://apireference.aspose.com/email/java/com.aspose.email/MapiMessage
[13]: https://apireference.aspose.com/email/java/com.aspose.email/IGraphClient#createMessage(java.lang.String,%20com.aspose.email.MapiMessage)
[14]: https://apireference.aspose.com/email/java/com.aspose.email/GraphClient#getClient(com.aspose.email.ITokenProvider)
[15]: https://apireference.aspose.com/email/java/com.aspose.email/MapiMessage
[16]: https://apireference.aspose.com/email/java/com.aspose.email/IGraphClient#send(com.aspose.email.MapiMessage)
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/email/java/
[19]: https://forum.aspose.com/
[20]: https://blog.aspose.com/2022/04/14/manage-folders-with-microsoft-graph-api-java/
[21]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/




