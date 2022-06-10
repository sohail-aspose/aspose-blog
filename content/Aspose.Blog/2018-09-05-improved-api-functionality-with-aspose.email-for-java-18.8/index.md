---
title: 'Improved API Functionality with Aspose.Email for Java 18.8'
date: Wed, 05 Sep 2018 17:24:37 +0000
draft: false
url: /2018/09/05/improved-api-functionality-with-aspose.email-for-java-18.8/
author: Muzammil Khan
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="aspose-email-for-java">}}


We are pleased to announce the release of [Aspose.Email for Java 18.8][1]. This month’s release includes an enhancement for updating member in a PST distribution list (DL) and appending another distribution list (DL) to an existing one. It also includes several other improvements in terms of bug fixes that further add to the overall stability of the API. For a detailed note on what is new and fixed, you may visit the [release notes][2] section of API.

## Improvements in Aspose.Email for Java 18.8

This release includes improvements to the API’s functionality like creating a contact in sub-folder of contacts using EWS and support of adding attachments to MapiCalendarExceptionInfo. There are certain backward incompatibility changes as well which will need you to update the code samples with the new ones. Following is a list of issues fixed in this month’s release.

*   Creating MapiMessage using MapiMessage.fromMailMessage gets stuck
*   Aspose.Email reads message body as second attachment
*   Wrong CC field after save and reload the message
*   Resaving EML turns Japanese language to garbage
*   Opening PST file raises error
*   Html is added as inline to MapiMEssage
*   EML to MSG disturbs output
*   MHT to MSG embeds header information in message body
*   IEWSClient always returns UTF8 Encoding for Message.BodyEncoding
*   Updating MSG BodyHtml doesn't change description in Outlook View Pane
*   Sender Type changed from Exchange to SMTP
*   The output message text content is unexpectedly concatenated on couple places
*   Invalid ContentUnreadCount value after splitInto()
*   Task start date/time set to UTC instead of local time

# API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   [Product Documentation][3] – Provides detailed examples of working with the API
*   [API Reference Guide][4] – Details all the packages and classes of the API
*   [GitHub Examples][5] – Provides ready to run API examples
*   [Aspose.Email Forum][6] – Feel free to contact us on Aspose.Email forum for your queries




[1]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-email/18.8
[2]: https://docs.aspose.com/display/emailjava/Aspose.Email+for+Java+18.8+Release+Notes
[3]: https://docs.aspose.com/display/emailjava/Home
[4]: http://www.aspose.com/api/java/email
[5]: https://github.com/aspose-email/Aspose.Email-for-Java
[6]: https://forum.aspose.com/c/email




