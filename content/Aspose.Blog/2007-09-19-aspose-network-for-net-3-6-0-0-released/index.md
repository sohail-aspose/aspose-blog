---
title: 'Aspose.Network for NET 3.6.0.0 Released'
date: Wed, 19 Sep 2007 03:00:00 +0000
draft: false
url: /2007/09/19/aspose-network-for-net-3-6-0-0-released/
author: Iret
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

**Introduction**

This release contains new features, features enhancement and bug fixes since v3.5.  Please check following description for more detail information.

**What's New?**

3756 - Support to render multipart/mixed type part in EML format.

           A new property Attachment.EmptyAttachment is added for this feature.

           \[Sample\]

           MailMessage msg = MailMessage.Load(@"c:\\ExchangeMessage.eml", MessageFormat.Eml);

           msg.Attachments.Add(Attachment.EmptyAttachment);

           msg.Save(@"c:\\exchangeeml.eml");

3758 - Support to delete attachments in Outlook Message files.

           \[Sample\]

           MailMessage.DestroyAttachments(@"c:\\attachment.msg");

3759 - Support converting undeliverable report message (Outlook Message files) to Eml format.

**What's Fixed?**

3751 - Multi-Language bug in reading the subject of Outlook Message files.

3752 - Cannot show the name of embeded Ole document when converting Outlook Message files to EML format.

3753 - Empty attachments are removed when converting Outlook Message files to EML format.

3754 - MapiAttachment.Save thows exception when saving an empty attachment.

3755 - Loading Eml messages will hung in MailMessage class

3757 - MailMessage throws exception when loading Eml files with invalid mail address in MailMessage class

Download URL: [http://www.aspose.com/Downloads/Aspose.Network/Default.aspx][1]




[1]: http://www.aspose.com/Downloads/Aspose.Network/Default.aspx




