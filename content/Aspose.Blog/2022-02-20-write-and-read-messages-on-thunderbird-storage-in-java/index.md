---
title: 'Write and Read Messages on Thunderbird Storage in Java'
seoTitle: "Write and Read Messages on Thunderbird Storage in Java"
description: "Use Java email library to access Thunderbird in Java. Write messages to Thunderbird storage in Java. Read messages from storage programmatically."
date: Sun, 20 Feb 2022 17:11:00 +0000
draft: false
url: /2022/02/20/write-and-read-messages-on-thunderbird-storage-in-java/
author: Usman Aziz
summary: '[Thunderbird][1] is an open-source application that allows you to configure your email accounts and access email messages from them. The application makes it possible to manage emails from multiple accounts in a single place. In certain cases, you may need to create and access email messages in Thunderbird storage programmatically. In accordance with that, this article shows **how to write and read messages on Thunderbird storage in Java**.'
tags: ['Java API to Write and Read Messages in Thunderbird Storage', 'Read Messages from Thunderbird Storage in Java', 'Write Messages on Thunderbird Storage in Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Write-and-Read-Messages-in-Thunderbird-Java.png" alt="Write and Read Messages on Thunderbird Storage in Java">}}


[Thunderbird][2] is an open-source application that allows you to configure your email accounts and access email messages from them. The application makes it possible to manage emails from multiple accounts in a single place. In certain cases, you may need to create and access email messages in Thunderbird storage programmatically. In accordance with that, this article shows **how to write and read messages on Thunderbird storage in Java**.

*   [Java API to Write and Read Messages in Thunderbird Storage][3]
*   [Write Messages on Thunderbird Storage][4]
*   [Read Messages from Thunderbird Storage][5]

## Java API to Write and Read Messages in Thunderbird Storage {#API-to-Write-and-Read-Messages-on-Thunderbird}

To write and read email messages in Thunderbird storage, we will use [Aspose.Email for Java][6]. It is an email processing API that lets you manipulate emails and work with popular email clients such as Thunderbird, Outlook, etc. You can either [download][7] the API or install it using the following Maven configurations.

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

## Write a Message on Thunderbird Storage in Java {#Write-Messages-on-Thunderbird}

You can create new messages and store them on Thunderbird's storage within a few steps using Aspose.Email for Java. The following are the steps to perform this operation in Java.

*   First, load the MBOX file into a [FileOutputStream][8] object.
*   Then, create an instance of [MboxrdStorageWriter][9] and initialize it with the stream.
*   After that, create a new [MailMessage][10] or load from file.
*   Write message to storage using [MboxrdStorageWriter.writeMessage(MailMessage)][11] method.
*   Finally, dispose of the writer and close the stream.

The following code sample shows how to write a message to Thunderbird storage in Java.

{{< gist aspose-com-gists 4587f4f70b733eebc36f247bd79c7fdc "write-message-thunderbird.java" >}}

## Read Messages from Thunderbird Storage in Java {#Read-Messages-from-Thunderbird}

To read the messages from Thunderbird storage, we need to load the storage file using [MboxrdStorageReader][12] class. The following are the steps to read messages from Thunderbird in Java.

*   First, load the MBOX file into a [FileInputStream][13] object.
*   Then, create an instance of [MboxrdStorageReader][14] to read the storage file.
*   After that, read first message using [MboxrdStorageReader.readNextMessage()][15] method.
*   Then, start a loop to iterate through all the messages.
*   Read each message and save it on disk if required.
*   Finally, dispose of the reader at the end.

The following code sample shows how to read messages from Thunderbird storage in Java.

{{< gist aspose-com-gists 4587f4f70b733eebc36f247bd79c7fdc "read-message-thunderbird.java" >}}

## Get a Free API License

You can use Aspose.Email for Java without evaluation limitations using a [free temporary license][16].

## Conclusion

Using Thunderbird, you can manage email messages from multiple accounts at a single location. In this article, you have learned how to write messages to Thunderbird storage in Java. Also, you have seen how to read messages from Thunderbird storage programmatically. Apart from that, you can visit the [documentation][17] to explore other features of Aspose.Email for Java. In case you would have any questions, you can post to our [forum][18].

## See Also

*   [Read Emails from MS Exchange Server in Java][19]




[1]: https://en.wikipedia.org/wiki/Mozilla_Thunderbird
[2]: https://en.wikipedia.org/wiki/Mozilla_Thunderbird
[3]: #API-to-Write-and-Read-Messages-on-Thunderbird
[4]: #Write-Messages-on-Thunderbird
[5]: #Read-Messages-from-Thunderbird
[6]: https://products.aspose.com/email/java/
[7]: https://downloads.aspose.com/email/java/
[8]: https://docs.oracle.com/javase/7/docs/api/java/io/FileOutputStream.html
[9]: https://apireference.aspose.com/email/java/com.aspose.email/MboxrdStorageWriter
[10]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage
[11]: https://apireference.aspose.com/email/java/com.aspose.email/MboxrdStorageWriter#writeMessage(com.aspose.email.MailMessage)
[12]: https://apireference.aspose.com/email/java/com.aspose.email/MboxrdStorageReader
[13]: https://docs.oracle.com/javase/7/docs/api/java/io/FileInputStream.html
[14]: https://apireference.aspose.com/email/java/com.aspose.email/MboxrdStorageReader
[15]: https://apireference.aspose.com/email/java/com.aspose.email/MboxrdStorageReader#readNextMessage()
[16]: https://products.aspose.com/email
[17]: https://docs.aspose.com/email/java/
[18]: https://forum.aspose.com/
[19]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/




