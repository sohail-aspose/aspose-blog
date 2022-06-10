---
title: 'Extract Attachments from PST Messages using Aspose.Email for .NET 6.1.0'
date: Fri, 01 Jan 2016 07:48:23 +0000
draft: false
url: /2016/01/01/extract-attachments-from-pst-messages-using-aspose.email-for-.net-6.1.0/
author: Muhammad Waqas
summary: ''
tags: ['Extracting attachments from messages in PST', 'Getting parent folder Information of a message in PST']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-net_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for .NET 6.1.0][1]. This month’s release includes a number of enhancements to various functional areas of the API. These are specifically related to the API’s Exchange Server client and Personal Storage (PST) functionality. It also includes a number of bug fixes that further add to the stability of the API. To get further details about what is new and fixed, please visit our product download page. You may also be interested in visiting our product documentation section to get an idea about the overall [API changes][2] in this month’s release.

# New Features and Enhancements

**Extracting Attachments from Messages within PST:** Working with PST files is one of the key features of Aspose.Email API. It not only provides the capability to generate PST files, but also manipulate these for extraction of messages, appointments, calendar and other Outlook message types. This month’s release further enhances the capabilities of working with PST files by providing the feature of [extracting message attachments][3] without extracting the complete message first. Thus, attachments can be extracted directly from the email message using the Message summary information (MessageInfo) or unique string id of the message as shown in the following code sample.

{{< gist aspose-email 9e8fbeb51a8cbc4129dc71ca8cd55f0b "Examples-CSharp-Outlook-ExtractAttachmentsFromPSTMessages-ExtractAttachmentsFromPSTMessages.cs" >}}

**Getting Parent Folder Information of a Message in PST:** This month’s release also includes an enhancement of accessing a message’s [parent folder information][4] in a PST. This can be achieved using the GetParentFolderInfo of the PersonalStorage class. The API uses the message’s summary information object, MessageInfo, or the stringId of the message for retrieving the message’s parent folder information.

**Setting MapiCalendar Timezone Information:** Aspose.Email API now provides the capability to initialize a calendar’s time zone information from standard Time zone object provided by the .NET framework. The overloaded member of MapiCalendarTimezone can be used to initialize a [calendar’s timezone][5] to local time zone object. Please note that this feature is available in .NET 3.5 and above.

**Provision of Including Special Characters in Folder Names:** Aspose.Email’s Exchange Web Service (EWS) API already provides the capability of creating folders and sub-folders in an Exchange Mailbox. However, the API had an issue while creating a folder name with “/” in it. It resulted in creating sub-folder after the “/”. This month’s release now provides IEWSClient.UseSlashAsFolderSeparate property to treat slash as folder separator and [create sub-folder][6] in mailbox.

# Other Improvements

This month’s release also includes a number of bug fixes that were faced by our valued customers while working with the previous version. Our product download page contains information about all the bug fixes and can be consulted for reference.

# API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   [Product Documentation][7] – Provides detailed examples of working with the API
*   [API Reference Guide][8] – Details all the namespaces and classes of the API
*   [GitHub Examples][9] – Provides ready to run API example
*   [Support Forum][10] – Write to us if you have any query or inquiry about the API




[1]: https://downloads.aspose.com/email/net
[2]: http://docs.aspose.com/display/emailnet/Public+API+Changes+in+Aspose.Email+6.1.0
[3]: https://docs.aspose.com/display/emailnet/Working+with+Messages+in+a+PST+File#WorkingwithMessagesinaPSTFile-ExtractAttachmentswithoutExtractingCompleteMessage
[4]: http://docs.aspose.com/display/emailnet/Read+Outlook+PST+File+and+Get+Folder+and+Subfolder+Information
[5]: https://docs.aspose.com/display/emailnet/Working+with+Outlook+Calendar+Items
[6]: https://docs.aspose.com/display/emailnet/Working+with+Folders+on+Exchange+Server
[7]: https://docs.aspose.com/display/emailnet/Home
[8]: https://apireference.aspose.com/net/email
[9]: https://github.com/asposeemail/Aspose_Email_NET
[10]: http://forum.aspose.com




