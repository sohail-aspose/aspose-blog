---
title: 'Aspose.Network 3.5.1.0 Released'
date: Tue, 05 Jun 2007 02:04:00 +0000
draft: false
url: /2007/06/05/aspose-network-3-5-1-releasenote/
author: Iret
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

Dear Customers,

We have released Aspose.Network 3.5.1.0. In this release, we enhanced the functionality of loading and parsing Microsoft Outlook Message Format (.Msg), according to the community feed backs.

What's new:

*   Add a new function to indicate the embedded Outlook Message, MapiObjectProperty.IsOutlookMessage
*   Support reading/saving embedded objects (Ole object) from Outlook message.
*   Enhance the format transfering from Outlook Message format to EML format.
    *   If the mime header is empty, we will try to load information from the relative mapi properties.
    *   Convert Rtf formatted body to Html body
    *   Load embedded objects of Outlook messages to Eml attachments
*   Fix the bug in GetDateTime function of MapiProperty.
*   Fix the bug in multi-language.

Known issues in this release:

*   Do not support table/color in the Rtf body to Html body.
*   Do not support embedded ole objects to Html body.
*   Although the embedded Outlook message can be saved locally, it cannot be opened by Outlook. Because the embedded Outlook message itself does not have proper file property header of normal Outlook message files.

How to download:

http://www.aspose.com/Downloads/Aspose.Network/Default.aspx








