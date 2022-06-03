---
title: 'Write and Read Messages on Thunderbird Storage in C# .NET'
date: Sat, 19 Mar 2022 10:13:00 +0000
draft: false
url: /2022/03/19/write-and-read-messages-on-thunderbird-storage-in-csharp/
author: ''Usman Aziz''
summary: '[Thunderbird][1] is an open-source email client application that lets you configure multiple email servers and access their email messages. This makes it possible for you to manage emails from multiple accounts in a single place. In certain cases, you may need to create and access email messages in Thunderbird storage programmatically. Accordingly, in this article, you will learn **how to write and read messages on Thunderbird storage in C# .NET**.'
tags: ['CSharp DotNet Email API', 'DotNet API to Write and Read Messages on Thunderbird', 'Read Messages from Thunderbird Storage in CSharp', 'Write Messages on Thunderbird Storage in Csharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Write-and-Read-Messages-in-Thunderbird-CSharp.png" alt="Write and Read Messages on Thunderbird Storage in C# .NET">}}


[Thunderbird][2] is an open-source email client application that lets you configure multiple email servers and access their email messages. This makes it possible for you to manage emails from multiple accounts in a single place. In certain cases, you may need to create and access email messages in Thunderbird storage programmatically. Accordingly, in this article, you will learn **how to write and read messages on Thunderbird storage in C# .NET**.

*   [.NET API to Write and Read Messages in Thunderbird][3]
*   [Write Messages on Thunderbird Storage][4]
*   [Read Messages from Thunderbird Storage][5]

## C# .NET API to Write and Read Messages in Thunderbird Storage {#API-to-Write-and-Read-Messages-on-Thunderbird}

To write and read email messages in Thunderbird storage, we will use [Aspose.Email for .NET][6]. It is an email processing API that lets you manipulate emails and work with popular email clients such as Thunderbird, Outlook, etc. You can [download][7] the API’s DLL or install it from [NuGet][8] using the following command.

```
PM> Install-Package Aspose.Email
```

## Write a Message on Thunderbird Storage in C# .NET {#Write-Messages-on-Thunderbird}

You can create new messages and store them on Thunderbird's storage within a few steps using Aspose.Email for .NET. The following are the steps to perform this operation in C#.

*   First, load the MBOX file into a [FileStream][9] object.
*   Then, create an instance of [MboxrdStorageWriter][10] and initialize it with the stream.
*   After that, create a new [MailMessage][11] and set its properties.
*   Write message to storage using [MboxrdStorageWriter.WriteMessage(MailMessage)][12] method.
*   Finally, dispose of the writer and close the stream.

The following code sample shows how to write a message to Thunderbird storage in C# .NET.

{{< gist aspose-com-gists 6838570e1c206d16fa6053262c7d3fbb "write-message-thunderbird.cs" >}}

## Read Messages from Thunderbird Storage in C# {#Read-Messages-from-Thunderbird}

To read the messages from Thunderbird storage, we need to load the storage file using [MboxrdStorageReader][13] class. The following are the steps to read messages from Thunderbird in C#.

*   First, load the MBOX file into a [FileStream][14] object.
*   Then, create an instance of [MboxrdStorageReader][15] to read the storage file.
*   After that, read first message using [MboxrdStorageReader.ReadNextMessage()][16] method.
*   Then, start a loop to iterate through all the messages.
*   Read each message and save it on disk if required.
*   Finally, dispose of the reader at the end.

The following code sample shows how to read messages from Thunderbird storage in C#.

{{< gist aspose-com-gists 6838570e1c206d16fa6053262c7d3fbb "read-message-thunderbird.cs" >}}

## Get a Free API License

You can use Aspose.Email for .NET without evaluation limitations using a [free temporary license][17].

## Conclusion

Using Thunderbird, you can access email messages from multiple accounts at a single location. In this article, you have learned how to write messages to Thunderbird storage in C# .NET. Also, you have seen how to read messages from Thunderbird storage programmatically. Apart from that, you can visit the [documentation][18] to explore other features of Aspose.Email for .NET. In case you would have any questions, you can post to our [forum][19].

## See Also

*   [Read Emails from MS Exchange Server using C#][20]




[1]: https://en.wikipedia.org/wiki/Mozilla_Thunderbird
[2]: https://en.wikipedia.org/wiki/Mozilla_Thunderbird
[3]: #API-to-Write-and-Read-Messages-on-Thunderbird
[4]: #Write-Messages-on-Thunderbird
[5]: #Read-Messages-from-Thunderbird
[6]: https://products.aspose.com/email/net/
[7]: https://downloads.aspose.com/email/net/
[8]: https://www.nuget.org/packages/Aspose.Email
[9]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream
[10]: https://apireference.aspose.com/email/net/aspose.email.storage.mbox/mboxrdstoragewriter
[11]: https://apireference.aspose.com/email/net/aspose.email/mailmessage
[12]: https://apireference.aspose.com/email/net/aspose.email.storage.mbox/mboxrdstoragewriter/methods/writemessage
[13]: https://apireference.aspose.com/email/net/aspose.email.storage.mbox/mboxrdstoragereader
[14]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream
[15]: https://apireference.aspose.com/email/net/aspose.email.storage.mbox/mboxrdstoragereader
[16]: https://apireference.aspose.com/email/net/aspose.email.storage.mbox/mboxrdstoragereader/methods/readnextmessage
[17]: https://products.aspose.com/email
[18]: https://docs.aspose.com/email/net/
[19]: https://forum.aspose.com/
[20]: https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/




