---
title: 'Create and Send Messages using Microsoft Graph API in C#'
date: Mon, 18 Apr 2022 07:10:00 +0000
draft: false
url: /2022/04/18/create-and-send-messages-using-microsoft-graph-api-in-csharp/
author: ''Usman Aziz''
summary: 'Microsoft offers [Graph API][1] to access the services of Office 365 and Microsoft Cloud programmatically from within your applications. Furthermore, you can use the Graph API to manage folders, send messages, and perform various other operations. In this article, you will learn **how to create and send messages using Microsoft Graph API in C#**.'
tags: ['Create Messages using Microsoft Graph API in CSharp', 'DotNet Microsoft Graph API', 'DotNet Microsoft Graph API to Create and Send Messages', 'Send Messages using Microsoft Graph API in CSharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Using-Microsoft-Graph-API-1024x542.jpg" alt="Create and Send Messages using Microsoft Graph API in C#">}}


Microsoft offers [Graph API][2] to access the services of Office 365 and Microsoft Cloud programmatically from within your applications. Furthermore, you can use the Graph API to manage folders, send messages, and perform various other operations. In this article, you will learn **how to create and send messages using Microsoft Graph API in C#**.

*   [.NET Microsoft Graph API to Create and Send Messages][3]
*   [Create Messages using Microsoft Graph API in C#][4]
*   [Send Messages using Microsoft Graph API in C#][5]

## C# .NET Microsoft Graph API to Create and Send Messages {#Microsoft-Graph-API-to-Create-and-Send-Messages}

[Aspose.Email for .NET][6] is an amazing API to create and send emails from within .NET applications. In addition, it allows you to use Microsoft Graph API and manage folders, messages, etc. We will use this API to create and send messages using Microsoft Graph API. You can [download][7] the API's DLL or install it from [NuGet][8] using the following command.

```
PM> Install-Package Aspose.Email
```

## Create a Message using Microsoft Graph API in C# {#Create-Messages-using-Microsoft-Graph-API}

To communicate with the Graph API, you need to first implement the [ITokenProvider][9] interface for authenticating the requests. The following is the basic implementation of _ITokenProvider_.

{{< gist aspose-com-gists 1990e8661551f5ac642d4c08a35b7ceb "token-provider.cs" >}}

The following are the steps to create a message using Microsoft Graph API in C#.

*   First, get an instance of Microsoft Graph client using [GraphClient.GetClient(ITokenProvider, string)][10] method.
*   Then, create an instance of [MapiMessage][11] class.
*   After that, set the subject, body, and other properties of the message.
*   Finally, create the message in desired folder using [IGraphClient.CreateMessage(GraphKnownFolders, MapiMessage)][12] method.

The following code sample shows how to create a message using Microsoft Graph API in C#.

{{< gist aspose-com-gists 1990e8661551f5ac642d4c08a35b7ceb "create-message.cs" >}}

## Send Messages using Microsoft Graph API in C# {#Send-Messages-using-Microsoft-Graph-API}

Let's now have a look at how to send a message using Microsoft Graph API in C#.

*   First, get an instance of Microsoft Graph client using [GraphClient.GetClient(ITokenProvider, string)][13] method.
*   Then, create an instance of [MapiMessage][14] class.
*   After that, set the subject, body, and other properties of the message.
*   Finally, send the message using [IGraphClient.Send(MapiMessage)][15] method.

The following code sample shows how to send a message using Microsoft Graph API in C#.

{{< gist aspose-com-gists 1990e8661551f5ac642d4c08a35b7ceb "send-message.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][16] to use Aspose.Email for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to use Microsoft Graph API to create and send messages in C#. You can simply install Aspose.Email and integrate the provided code samples into your .NET applications. In addition, you can have a look at other features offered by Aspose.Email for .NET using the [documentation][17]. Also, in case you would have any questions, you can post to our [forum][18].

## See Also

*   [Read Emails from MS Exchange Server using C#][19]




[1]: https://en.wikipedia.org/wiki/Microsoft_Graph
[2]: https://en.wikipedia.org/wiki/Microsoft_Graph
[3]: #Microsoft-Graph-API-to-Create-and-Send-Messages
[4]: #Create-Messages-using-Microsoft-Graph-API
[5]: #Send-Messages-using-Microsoft-Graph-API
[6]: https://products.aspose.com/email/net/
[7]: https://downloads.aspose.com/email/net/
[8]: https://www.nuget.org/packages/Aspose.Email
[9]: https://apireference.aspose.com/email/net/aspose.email.clients/itokenprovider
[10]: https://apireference.aspose.com/email/net/aspose.email.clients.graph.graphclient/getclient/methods/1
[11]: https://apireference.aspose.com/email/net/aspose.email.mapi/mapimessage
[12]: https://apireference.aspose.com/email/net/aspose.email.clients.graph/igraphclient/methods/createmessage
[13]: https://apireference.aspose.com/email/net/aspose.email.clients.graph.graphclient/getclient/methods/1
[14]: https://apireference.aspose.com/email/net/aspose.email.mapi/mapimessage
[15]: https://apireference.aspose.com/email/net/aspose.email.clients.graph/igraphclient/methods/send
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/email/net/
[18]: https://forum.aspose.com/
[19]: https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/




