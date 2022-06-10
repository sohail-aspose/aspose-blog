---
title: 'Improved API Performance with Aspose.Email for .NET 18.8'
date: Thu, 30 Aug 2018 11:47:09 +0000
draft: false
url: /2018/08/30/improved-api-performance-with-aspose.email-for-.net-18.8/
author: Muhammad Ahmad
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Aspose.Email-for-.NET_.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for .NET 18.8][1]. This release is sort of maintenance release where the API functionality has been improved as result of several bug fixes. For a detailed note on what is new and fixed, please visit the [release notes][2] section of API.

## Improvements in Aspose.Email for .NET 18.8

This release includes several improvements to the API’s functionality like creating a contact in sub-folder of contacts using EWS, support of adding attachments to MapiCalendarExceptionInfo and updating member in a PST distribution list(DL). There are certain backward incompatibility changes as well which will need you to update the code samples with the new ones. Following is a list of issues fixed in this month’s release.

*   Message body read as a second attachment.
*   Wrong CC field is shown after saving and reloading the message.
*   Resaving EML turns the Japanese language to garbage.
*   Opening PST file raises an error.
*   Html is added as inline to MapiMessage.
*   EML to MSG conversion disturbs the output.
*   MHT to MSG conversion embeds header information in the message body.
*   IEWSClient always returns UTF8 Encoding for Message.BodyEncoding.
*   Updating MSG BodyHtml doesn't change the description in Outlook View Pane.
*   Sender Type changed from Exchange to SMTP.
*   The output message text content is unexpectedly concatenated on couple places.
*   Invalid "ContentUnreadCount" value after splitInto().

## API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   [Product Documentation][3] – Provides detailed examples of working with the API
*   [API Reference Guide][4] – Details all the namespaces and classes of the API
*   [GitHub Examples][5] – Provides ready to run API example
*   [Support Forum][6] – Write to us if you have any query or inquiry about the API




[1]: https://www.nuget.org/packages/Aspose.Email/
[2]: https://docs.aspose.com/display/emailnet/Aspose.Email+for+.NET+18.8+Release+Notes
[3]: https://docs.aspose.com/display/emailnet/Home
[4]: https://apireference.aspose.com/net/email
[5]: https://github.com/asposeemail/Aspose_Email_NET
[6]: https://forum.aspose.com/c/email




