---
title: 'Work with Conversations on MS Exchange Server in C#'
date: Thu, 31 Mar 2022 06:05:38 +0000
draft: false
url: /2022/03/31/work-with-conversations-in-ms-exchange-server-in-csharp/
author: 'Usman Aziz'
summary: 'The conversations on [Microsoft Exchange Server][1] are referred to as the group of email messages in a thread. In simple words, an email and all its replies are known to be a conversation. In this article, we will show you how to work with conversations in MS Exchange Server programmatically. Particularly, you will learn **how to find, copy, move and delete conversations on MS Exchange Server in C# .NET**.'
tags: ['API to Work with Conversations in MS Exchange Server in Csharp', 'Copy a Conversation in MS Exchange Server Csharp', 'Delete a Conversation in MS Exchange Server Csharp', 'Find Conversations in MS Exchange Server Csharp', 'Move a Conversation in MS Exchange Server Csharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Work with Conversations in MS Exchange Server in C#">}}


The conversations on [Microsoft Exchange Server][2] are referred to as the group of email messages in a thread. In simple words, an email and all its replies are known to be a conversation. In this article, we will show you how to work with conversations in MS Exchange Server programmatically. Particularly, you will learn **how to find, copy, move and delete conversations on MS Exchange Server in C# .NET**.

*   [C# .NET API to Work with Conversations on MS Exchange Server][3]
*   [Find Conversations on MS Exchange Server in C#][4]
*   [Copy a Conversation on MS Exchange Server in C#][5]
*   [Move a Conversation on MS Exchange Server in C#][6]
*   [Delete a Conversation on MS Exchange Server in C#][7]

## C# .NET API to Work with Conversations on MS Exchange Server {#API-to-Work-with-Conversations-in-MS-Exchange-Server}

To manage the conversations on Microsoft Exchange Server, we will use [Aspose.Email for .NET][8]. It is a powerful API that provides a range of features to implement email client applications. Also, it allows you to access various services of MS Exchange Server seamlessly. You can either [download][9] the API’s DLL or install it from [NuGet][10] using the following command.

```
PM> Install-Package Aspose.Email
```

## Find Conversations on MS Exchange Server in C# {#Find-Conversations-in-MS-Exchange-Server}

The following are the steps to find conversations from a folder in MS Exchange Server in C#.

*   First, create and initialize the [NetworkCredential][11] object with username, password, and domain.
*   Then, initialize [IEWSClient][12] with mailbox URI and _NetworkCredential _object.
*   Call [IEWSClient.FindConversations(IEWSClient.MailboxInfo.InboxUri)][13] method and get conversations in an [ExchangeConversation][14] array.
*   Finally, loop through each [ExchangeConversation][15] object in the array and retrieve its details.

The following code sample shows how to find conversations from a folder in MS Exchange Server in C#.

{{< gist aspose-com-gists 3cd2f5b427b5f7837a575250ce147fa9 "find-conversation.cs" >}}

## Copy a Conversation on MS Exchange Server in C# {#Copy-a-Conversation-in-MS-Exchange-Server}

You can also copy the conversations from one folder to another without writing a complex code. For demonstration, let's have a look at how to copy conversations from the inbox to deleted items folder of Exchange Server in C# .NET.

*   First, create and initialize the [NetworkCredential][16] object with username, password, and domain.
*   Then, initialize [IEWSClient][17] with mailbox URI and _NetworkCredential _object.
*   Call [IEWSClient.FindConversations(IEWSClient.MailboxInfo.InboxUri)][18] method and get conversations in an [ExchangeConversation][19] array.
*   Loop through each [ExchangeConversation][20] in the array and filter the required one(s).
*   Finally, copy conversation using [IEWSClient.CopyConversationItems(ExchangeConversation.ConversationId, client.MailboxInfo.DeletedItemsUri)][21] method.

The following code sample shows how to copy a conversation in MS Exchange Server using C# .NET.

{{< gist aspose-com-gists 3cd2f5b427b5f7837a575250ce147fa9 "copy-conversation.cs" >}}

## Move a Conversation on MS Exchange Server in C# {#Move-a-Conversation-in-MS-Exchange-Server}

In the previous section, we just copied conversations from one folder to another. However, in certain cases, you may need to move a conversation to a particular folder. The following are the steps to move conversations in MS Exchange Server in C# .NET.

*   First, create and initialize the [NetworkCredential][22] object with username, password, and domain.
*   Then, initialize [IEWSClient][23] with mailbox URI and _NetworkCredential _object.
*   Call [IEWSClient.FindConversations(IEWSClient.MailboxInfo.InboxUri)][24] method and get conversations in an [ExchangeConversation][25] array.
*   Loop through each [ExchangeConversation][26] in the array and filter the required one(s).
*   Finally, move conversation using [IEWSClient.MoveConversationItems(ExchangeConversation.ConversationId, client.MailboxInfo.DeletedItemsUri)][27] method.

The following code sample shows how to move a conversation in MS Exchange Server using C# .NET.

{{< gist aspose-com-gists 3cd2f5b427b5f7837a575250ce147fa9 "move-conversation.cs" >}}

## Delete a Conversation on MS Exchange Server in C# {#Delete-a-Conversation-in-MS-Exchange-Server}

Last but not the least, let's have a look at how to delete a conversation from MS Exchange Server in C#.

*   First, create and initialize the [NetworkCredential][28] object with username, password, and domain.
*   Then, initialize [IEWSClient][29] with mailbox URI and _NetworkCredential _object.
*   After that, call [IEWSClient.FindConversations(IEWSClient.MailboxInfo.InboxUri)][30] method and get conversations in an [ExchangeConversation][31] array.
*   Loop through each [ExchangeConversation][32] in the array and filter the required one(s).
*   Finally, delete a conversation using [IEWSClient.DeleteConversationItems(ExchangeConversation.ConversationId)][33] method.

The following code sample shows how to delete a conversation from MS Exchange Server in C# .NET.

{{< gist aspose-com-gists 3cd2f5b427b5f7837a575250ce147fa9 "delete-conversation.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][34] to use Aspose.Email for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to manage conversations in Microsoft Exchange Server using C#. You have seen how to find, copy, move, and delete conversations on MS Exchange Server programmatically in C#. In addition, you can explore the [documentation][35] to read more about Aspose.Email for .NET. Also, you can ask your questions via our [forum][36].

## See Also

*   [Read Emails from MS Exchange Server using C#][37]




[1]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[2]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[3]: #API-to-Work-with-Conversations-in-MS-Exchange-Server
[4]: #Find-Conversations-in-MS-Exchange-Server
[5]: #Copy-a-Conversation-in-MS-Exchange-Server
[6]: #Move-a-Conversation-in-MS-Exchange-Server
[7]: #Delete-a-Conversation-in-MS-Exchange-Server
[8]: https://products.aspose.com/email/net
[9]: https://downloads.aspose.com/email/net
[10]: https://www.nuget.org/packages/Aspose.Email/
[11]: https://docs.microsoft.com/en-us/dotnet/api/system.net.networkcredential
[12]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[13]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/findconversations
[14]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/exchangeconversation
[15]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/exchangeconversation
[16]: https://docs.microsoft.com/en-us/dotnet/api/system.net.networkcredential
[17]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[18]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/findconversations
[19]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/exchangeconversation
[20]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/exchangeconversation
[21]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/copyconversationitems
[22]: https://docs.microsoft.com/en-us/dotnet/api/system.net.networkcredential
[23]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[24]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/findconversations
[25]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/exchangeconversation
[26]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/exchangeconversation
[27]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/moveconversationitems
[28]: https://docs.microsoft.com/en-us/dotnet/api/system.net.networkcredential
[29]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[30]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/findconversations
[31]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/exchangeconversation
[32]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/exchangeconversation
[33]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/deleteconversationitems
[34]: https://purchase.aspose.com/temporary-license
[35]: https://docs.aspose.com/email/net/
[36]: https://forum.aspose.com/
[37]: https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/




