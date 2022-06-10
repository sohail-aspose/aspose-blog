---
title: 'Work with Zimbra and IBM Notes using C# or Java'
date: Thu, 19 Sep 2019 11:08:16 +0000
draft: false
url: /2019/09/19/zimbra-and-ibm-notes-support-included-in-aspose.email/
author: Mudassir
summary: ''
tags: ['Work with IBM Notes in csharp', 'Work with Zimbra in csharp', 'work with ibm notes in java', 'work with zimbra in java']
categories: ['Aspose.Email Product Family']
---

[![][1]](https://products.aspose.com/email/net)Hello firends! in today's blog, I am going to introduce you to what new features have been included in Aspose.Email 19.8. The API has been published for both .NET and Java and having same features sets. This way, the users of both API's can make use of new features irrespective of application and platform type. In following sections, I will shed some light on new features available in API and how to use them.

## Working with Zimbra

Zimbra is an email, calendar and collaboration suite built for the cloud. Zimbra includes complete email, contacts, calendar, file sharing, tasks and messaging/videoconferencing, all accessed from the Zimbra Web Client from any device.

Aspose.Email provides the TgzReader class to read Zimbra TGZ storage files. The following example demonstrates the use of the TgzReader class to read all messages from the file.

{{< gist aspose-com-gists 522d47278b8ca448dc1d7eb97193322c "Examples-CSharp-Email-ReadAllMessagesFromZimbraTgzStorage-1.cs" >}}

The similar Java-based example for this is:

{{< gist aspose-com-gists 709d733586ce50505c3bca3f6e8bd18d "Examples-src-main-java-com-aspose-email-examples-email-ReadAllMessagesFromZimbraTgzStorage-1.java" >}}

One can also save all the messages with directory structure from the Zimbra TGZ storage file. For this, the TgzReader class provides a method ExportTo which takes the output path as a parameter. The following example demonstrates the use of the TgzReader.ExportTo method to save all messages from the Zimbra TGZ storage file.

{{< gist aspose-com-gists 522d47278b8ca448dc1d7eb97193322c "Examples-CSharp-Email-SaveMessagesFromZimbraTgzStorage-1.cs" >}}

The similar Java-based example for this is:

{{< gist aspose-com-gists 709d733586ce50505c3bca3f6e8bd18d "Examples-src-main-java-com-aspose-email-examples-email-SaveMessagesFromZimbraTgzStorage-1.java" >}}

## Working with IBM Notes

IBM Notes is the client and IBM Domino is the server of a collaborative client-server software platform. IBM Notes provides collaboration features like email, calendars, to-do lists, contacts management, etc. The database file used by IBM Notes is saved in the Notes Storage Facility (NSF) format.

Aspose.Email provides the NotesStorageFacility class to read NSF storage files. The NotesStorageFacility class provides the EnumerateMessages method which iterates over the messages in the NSF storage file. The following sample code demonstrates the use of the NotesStorageFacility class and the EnumerateMessages method to read messages from the NSF storage file.

{{< gist aspose-com-gists 522d47278b8ca448dc1d7eb97193322c "Examples-CSharp-Email-ReadMessagesFromNSFStorage-1.cs" >}}

The similar Java-based example for this is:

{{< gist aspose-com-gists 709d733586ce50505c3bca3f6e8bd18d "Examples-src-main-java-com-aspose-email-examples-email-ReadMessagesFromNSFStorage-1.java" >}}

There are many other features, enhancement, and bug fixes included in this release. [Here you can get the detail!][2]

When time allows you can check out API [examples at Github][3], talk about this release and other API related issues in our [forum][4].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2016/12/Aspose.Email-for-.NET_.png
[2]: https://docs.aspose.com/display/emailnet/Aspose.Email+for+.NET+19.8+Release+Notes
[3]: https://github.com/aspose-email
[4]: https://forum.aspose.com/c/email




