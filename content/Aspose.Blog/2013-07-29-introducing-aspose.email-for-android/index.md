---
title: 'Android Email API - Introducing Aspose.Email for Android'
date: Mon, 29 Jul 2013 08:44:57 +0000
draft: false
url: /2013/07/29/introducing-aspose.email-for-android/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Total Product Family', 'Aspose.Email Product Family']
---

We are pleased to announce the launch of [Aspose.Email for Android][1], an API that empowers software developers to design Android applications for managing and manipulating email messages without getting lost in the complexities of Microsoft Outlook file format implementation. This is good news for Android developers and users who would like to include the functionality of creating, reading and manipulating Outlook messages in their mobile apps.

Aspose.Email for [.NET][2] and [Java][3] have been out for a long time already and has field-proven performance for creating, reading, and manipulating Outlook messages in applications. The power lies in its capabilities to make developers independent Microsoft Outlook automation in applications - they don't even need Outlook installed on the system where the application is running.

## Aspose.Email for Android

Aspose.Email for Android is a message creation, reading and manipulating component for Android developers and users. At its base, Aspose.Email for Android has the strong foundations of its Java ancestor which is already proven for creating, reading and converting email messages to different formats as well as reading, creating and manipulating message storage files, i.e. PST and OST.

## How to Use Aspose.Email for Android

Aspose.Email for Android library comes as a JAR file that can be included in applications like any other JAR file. You can get started with Aspose.Email for Android in no time with Android Developers Toolkit (ADT), bundled with a pre-configured version of Eclipse. With the vast range of articles and documentation samples, the API empowers you to quickly program with the Aspose.Email API and test your app for the desired functionality. To get started, download [Aspose.Email for Android][4] now and follow the steps in our online guide to create your first application with Aspose.Email for Android.

## Email Messages Manipulation

You can not only read message files, but also modify the contents of a message and save it back. With Aspose.Email, you can retrieve email information such as sender, receiver, subject, and body from message files.  Embedded objects, such as in-line images, can be added as well as extracted as linked resources from a message body and saved to disc. The API also lets you manipulate message attachments with just a few lines of code. You can not only extract regular attachments from a message, but also process nested messages that are part of a message. The same is true for adding any type of attachments to messages that you are creating.

Using Aspose.Email, you get complete control over customizing email [message headers][5]. You can add headers to a message, read all headers, and [extract headers][6] from a message file. Similarly, for outlook MSG files, it gives you complete access to the message’s MAPI properties.

## Supported Email Formats

Aspose.Email supports all the well-known email formats supported by Outlook:

*   Outlook message files (MSG)
*   Outlook Template files (OFT)
*   EML
*   EMLX
*   TNEF
*   MHT
*   PST
*   OST

## Supported Conversion Types

Aspose.Email supports conversion between various message formats and you can inter-convert between various message formats with just a couple of lines of code. For example, the following lines of code converts a message from MSG to EML:

```
MailMessage mailMsg = MailMessage.load("sourceMsg.msg", MessageFormat.getMsg());
mailMsg.save("targetEML.eml", MailMessageSaveType.getEmlFormat());
```

Aspose.Email supports:

*   MSG to EML
*   EML to MSG
*   MSG to MHT
*   MHT to MSG
*   EML to MHT
*   MHT to EML

## Support for Message Storage Files (PST/OST)

Aspose.Email not only supports manipulating message files, but also gives complete control to manage message storage files, that is Personal Storage Files (PST) and Offline Storage Files (OFT). You can create PST files and add messages to them in no time. With its well-structured API, Aspose.Email gives you complete access to a PST file’s folders, sub-folders and messages for reading and extraction.

## Supported Operations

Aspose.Email supports wide range of operations on message storage files (both PST and OST). These are:

*   Creating PST file.
*   Reading PST file.
*   Adding predefined folders to the PST.
*   Adding/extracting messages from a PST.
*   Adding/saving contacts from a PST.
*   Adding/saving calendar items from a PST.
*   Adding MapiNotes, journals, notes, tasks, and distribution lists to a PST.
*   Deleting items from a PST.

## Creating and Reading PST/OST Files

With Aspose.Email, you can easily create PST and OST files from scratch and add folders to them. At present, only Unicode versions are supported. You can create and save PST files directly to disc as well as to memory stream. Similarly, reading PST files from disc as well as memory stream is also facilitated by Aspose.Email where information about folders and subfolders and messages can be retrieved.

## Adding Predefined Folders to a PST/OST

Predefined folders such as Inbox, Sent Items, Drafts, Contacts, etc. can quickly be added to a PST using the Aspose.Email library.  Adding these folders make the PST ready to accept messages that are added to these folders.

## Adding MAPI Items to a PST/OST

With Aspose.Email, you can add different types of items to PST file. It supports adding:

*   Messages
*   Contacts
*   Calendar items
*   Notes
*   Journals, and
*   Tasks

to predefined PST folders.

## Extracting Messages from a PST/OST

Aspose.Email enables you to access each folder of a PST and extract messages from it. You can extract and save messages either to disc or memory stream. Aspose.Email provides the facility to save the messages as Microsoft OIutlook MSG files or to Mail Message format using the MailMessageInterpretorFactory class. Thus, messages can be saved in MSG, EML, EMLX, and MHTML formats once they are made available as mail message.

## Extracting Contacts from a PST/OST

Aspose.Email gives you access to a PST file's Contacts folder for managing its contents. You can access the contacts information of each contact using the MapiContact class and can save the item either as Outlook MSG or VCard formats.

## Managing Calendar Items

Aspose.Email provides full capability for generating calendar items such as appointments and meetings with the option to add recurring information as well as optional fields to the created item. Appointments can be created and saved to disc in draft format or added to a PST's calendar items. The MapiCalendar class offers all the properties required to completely define a calendar. It also enables you to access and extract MapiCalendar items from PST and save to ICS format.

## Checking for Password Protection

Microsoft Outlook lets users password protect PST files to restrict access to them. Aspose.Email can detect password protection on a PST file and also provides the means to check the validity of the password.

Aspose.Email for Android gives Android developers enough power to manage messages and message storage files without the need of installing Outlook. We are continuously improving our product with new features and enhancements. In addition, our detailed online documentation provides a number of samples for getting started with Aspose.Email in no time. You can reach us out for support on [Aspose.Email forum][7] where our support team assists you with your inquiries.




[1]: https://products.aspose.com/email/android-java
[2]: https://products.aspose.com/email/net
[3]: https://products.aspose.com/email/java
[4]: https://products.aspose.com/email/android-java
[5]: https://docs.aspose.com/email/java
[6]: https://docs.aspose.com/email/java
[7]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




