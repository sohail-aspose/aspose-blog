---
title: 'Search PST File for Messages using Java'
date: Sat, 08 Nov 2014 16:25:02 +0000
draft: false
url: /2014/11/08/search-pst-file-for-messages-using-java/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for Java][1] 4.7.0. It includes a number of enhancements to the existing functionality of the API along with fixes for issues reported in previous versions. Specifically, it includes search capabilities for messages in a PST, improving PST size and speed, and creating TNEF messages from MapiMessage. To get complete details about what is new and fixed, please visit the [product download page][2].

## Searching PST for Messages

This month’s release provides the capability of searching a PST for messages based on specified criteria using the PersonalStorageQueryBuilder class. The feature offers searching messages based on:

*   Message importance
*   Message class
*   Presence of attachments
*   Message size
*   Unread messages
*   Unread messages with attachments, and
*   Folders with specific subfolder name

The documentation article, Searching Messages and folders in PST, demonstrates how to use this feature.

## Creating TNEF MailMessage from MapiMessage

This month’s release includes a new feature that allows you to create TNEF EML messages from Outlook MSG files. It can preserve the contents of MSG files such as tables and text styles if the converted message is sent out. The InterpretAsTnef property is used to achieve this as shown in the TNEF attachment example.

## Creating Messages with Body Compression

Aspose.Email now allows developers to reduce the message size by using RTF body compression. This, as a result, creates a smaller size PST but at the cost of speed.  If speed is a requirement, then set the UseBodyCompression property to false to turn compression off. Read more.

## Message Conversions to MHTML

Aspose.Email already provides the capability to convert emails to MHTML format. Until now, there were limited options for controlling header fields during the conversion. This month’s release brings further improvements to this functionality by providing the capability of writing the To, From, CC and BCC fields to the output. Find out more.

## Bug Fixes

This month’s release includes a number of bug fixes which further aids the API functionality improvement. Bugs fixed in this month’s release include corrupt message creation with MapiRecipient, contact Notes formatting issues, and all the ported issues from our .NET version of Aspose.Email.




[1]: https://products.aspose.com/email/java
[2]: https://downloads.aspose.com/email




