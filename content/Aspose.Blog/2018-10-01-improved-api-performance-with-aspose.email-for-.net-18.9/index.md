---
title: 'Improved API Performance with Aspose.Email for .NET 18.9'
date: Mon, 01 Oct 2018 05:59:57 +0000
draft: false
url: /2018/10/01/improved-api-performance-with-aspose.email-for-.net-18.9/
author: Muzammil Khan
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Aspose.Email-for-.NET_.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for .NET 18.9][1]. This release is sort of maintenance release where the API functionality has been improved as result of several bug fixes. For a detailed note on what is fixed, please visit the [release notes][2] section of API.

## Improvements in Aspose.Email for .NET 18.9

This release includes several improvements to the API’s functionality. There are certain backward incompatibility changes as well which will need you to update the code samples with the new ones. Following is a list of issues fixed in this month’s release.

*   Issues with converting meeting requests to MHTML
*   Multiple issues with MapiContact modification
*   Date header returns wrong date when read from some MSG files
*   Loading FileStream in MailMessage is taking a long time
*   Setting MhtSaveOptions.SaveAttachments to "false" removes attachment names from the generated mhtml
*   Organizer cannot accept the time proposed by attendee
*   Attachment corrupted when converting PST to MSG using PersonalStorage.SaveMessageToStream
*   The email attachment name becomes blank in MHTML output
*   A Linefeed at the beginning of messageID causes imapclient.ListMessages() to throw an exception
*   The subject isn't properly normalized after loading EML message
*   Email sent using MailMessage configured .msg is missing Text Formatting and missing Images from body of the email
*   The retrieved delivery time isn't correct
*   Text Missing While Using mapiMessage.ToMailMessage API
*   FetchItem method throws a null reference exception
*   Email to mhtml to png fails with the latest version - Infinite Loop Error
*   The Mapi message isn't properly saved to MSG format

## API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   [Product Documentation][3] – Provides detailed examples of working with the API
*   [API Reference Guide][4] – Details all the namespaces and classes of the API
*   [GitHub Examples][5] – Provides ready to run API example
*   [Support Forum][6] – Write to us if you have any query or inquiry about the API




[1]: https://www.nuget.org/packages/Aspose.Email/
[2]: https://docs.aspose.com/display/emailnet/Aspose.Email+for+.NET+18.9+Release+Notes
[3]: https://docs.aspose.com/display/emailnet/Home
[4]: https://apireference.aspose.com/net/email
[5]: https://github.com/asposeemail/Aspose_Email_NET
[6]: https://forum.aspose.com/c/email




