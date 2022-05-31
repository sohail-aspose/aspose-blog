---
title: 'Work with Conversations on MS Exchange Server in Java'
date: Mon, 28 Feb 2022 07:41:00 +0000
draft: false
url: /2022/02/28/work-with-conversations-on-ms-exchange-server-in-java/
author: ''Usman Aziz''
summary: 'Often, an email is composed of multiple messages (or replies) forming a thread. In [Microsoft Exchange Server][1], these threads are termed as conversations. While working with MS Exchange Server programmatically, you may need to access and manage the conversations. To accomplish that, in this article, you will learn **how to find, copy, move and delete conversations on Microsoft Exchange Server in Java**.'
tags: ['Copy a Conversation on MS Exchange Server in Java', 'Delete a Conversation on MS Exchange Server in Java', 'Find Conversation on MS Exchange Server in Java', 'Java API to Work with Conversations on MS Exchange Server', 'Move a Conversation on MS Exchange Server in Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Work with Conversations on MS Exchange Server in Java">}}


Often, an email is composed of multiple messages (or replies) forming a thread. In [Microsoft Exchange Server][2], these threads are termed as conversations. While working with MS Exchange Server programmatically, you may need to access and manage the conversations. To accomplish that, in this article, you will learn **how to find, copy, move and delete conversations on Microsoft Exchange Server in Java**.

*   [Java API to Work with Conversations on MS Exchange Server][3]
*   [Find Conversation on MS Exchange Server in Java][4]
*   [Copy a Conversation on MS Exchange Server in Java][5]
*   [Move a Conversation on MS Exchange Server in Java][6]
*   [Delete a Conversation on MS Exchange Server in Java][7]

## Java API to Work with Conversations on MS Exchange Server {#API-to-Work-with-Conversations-in-MS-Exchange-Server}

To work with the conversations on Microsoft Exchange Server, we will use [Aspose.Email for Java][8]. It is an amazing API that provides a bunch of features to work with MS Exchange Server from within Java applications. You can either [download][9] the API or install it using the following Maven configurations.

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

## Find Conversations on MS Exchange Server in Java {#Find-Conversations-in-MS-Exchange-Server}

The following are the steps to find conversations from a folder in MS Exchange Server using Java.

*   First, create and initialize the _NetworkCredential_ object with username, password, and domain.
*   Then, initialize [IEWSClient][10] with mailbox URI and _NetworkCredential _object.
*   Call [IEWSClient.findConversations(IEWSClient.getMailboxInfo().getInboxUri())][11] method and get conversations in an [ExchangeConversation][12] array.
*   Finally, loop through each [ExchangeConversation][13] object in the array and retrieve its details.

The following code sample shows how to find conversations from a folder in MS Exchange Server in Java.

{{< gist aspose-com-gists 6dc20fbc731592afcdc8e14707120f21 "find-conversation.java" >}}

## Copy a Conversation on MS Exchange Server in Java {#Copy-a-Conversation-in-MS-Exchange-Server}

You can also copy the conversations from one folder to another. Let's have a look at how to copy conversations from the inbox to deleted items folder of Exchange Server in Java.

*   First, create and initialize the _NetworkCredential_ object with username, password, and domain.
*   Then, initialize [IEWSClient][14] with mailbox URI and _NetworkCredential _object.
*   Call [IEWSClient.findConversations(IEWSClient.getMailboxInfo().getInboxUri())][15] method and get conversations in an [ExchangeConversation][16] array.
*   Loop through each [ExchangeConversation][17] object in the array and filter required one(s).
*   Finally, copy conversation using [IEWSClient.copyConversationItems(ExchangeConversation.getConversationId(), IEWSClient.getMailboxInfo().getDeletedItemsUri())][18] method.

The following code sample shows how to copy a conversation in MS Exchange Server using Java.

{{< gist aspose-com-gists 6dc20fbc731592afcdc8e14707120f21 "copy-conversation.java" >}}

## Move a Conversation on MS Exchange Server in Java {#Move-a-Conversation-in-MS-Exchange-Server}

In the previous section, we just copied conversations from one folder to another. However, in certain cases, you may need to move a conversation to a particular folder. The following are the steps to move a conversation in MS Exchange Server in Java.

*   First, create and initialize the _NetworkCredential_ object with username, password, and domain.
*   Then, initialize [IEWSClient][19] with mailbox URI and _NetworkCredential _object.
*   Call [IEWSClient.findConversations(IEWSClient.getMailboxInfo().getInboxUri())][20] method and get conversations in an [ExchangeConversation][21] array.
*   Loop through each [ExchangeConversation][22] object in the array and filter required one(s).
*   Finally, move conversation using [IEWSClient.moveConversationItems(ExchangeConversation.getConversationId(), IEWSClient.getMailboxInfo().getDeletedItemsUri())][23] method.

The following code sample shows how to move a conversation in MS Exchange Server using Java.

{{< gist aspose-com-gists 6dc20fbc731592afcdc8e14707120f21 "move-conversation.java" >}}

## Delete a Conversation on MS Exchange Server in Java {#Delete-a-Conversation-in-MS-Exchange-Server}

In the end, let's have a look at how to delete a conversation from MS Exchange Server in Java.

*   First, create and initialize the _NetworkCredential_ object with username, password, and domain.
*   Then, initialize [IEWSClient][24] with mailbox URI and _NetworkCredential _object.
*   Call [IEWSClient.findConversations(IEWSClient.getMailboxInfo().getInboxUri())][25] method and get conversations in an [ExchangeConversation][26] array.
*   Loop through each [ExchangeConversation][27] object in the array and filter required one(s).
*   Finally, delete a conversation using [IEWSClient.deleteConversationItems(ExchangeConversation.getConversationId())][28] method.

The following code sample shows how to delete a conversation from MS Exchange Server in Java.

{{< gist aspose-com-gists 6dc20fbc731592afcdc8e14707120f21 "delete-conversation.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][29] to use Aspose.Email for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to manage conversations in Microsoft Exchange Server using Java. You have seen how to find, copy, move, and delete a conversation on MS Exchange Server programmatically in Java. In addition, you can explore the [documentation][30] to read more about Aspose.Email for Java. Also, you can ask your questions via our [forum][31].

## See Also

*   [Read Emails from MS Exchange Server in Java][32]




[1]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[2]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[3]: #API-to-Work-with-Conversations-in-MS-Exchange-Server
[4]: #Find-Conversations-in-MS-Exchange-Server
[5]: #Copy-a-Conversation-in-MS-Exchange-Server
[6]: #Move-a-Conversation-in-MS-Exchange-Server
[7]: #Delete-a-Conversation-in-MS-Exchange-Server
[8]: https://products.aspose.com/email/java/
[9]: https://downloads.aspose.com/email/java/
[10]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[11]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#findConversations(java.lang.String)
[12]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeConversation
[13]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeConversation
[14]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[15]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#findConversations(java.lang.String)
[16]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeConversation
[17]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeConversation
[18]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#copyConversationItems(java.lang.String,%20java.lang.String)
[19]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[20]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#findConversations(java.lang.String)
[21]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeConversation
[22]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeConversation
[23]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#moveConversationItems(java.lang.String,%20java.lang.String)
[24]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[25]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#findConversations(java.lang.String)
[26]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeConversation
[27]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeConversation
[28]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#deleteConversationItems(java.lang.String)
[29]: https://purchase.aspose.com/temporary-license
[30]: https://docs.aspose.com/email/java/
[31]: https://forum.aspose.com/
[32]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/




