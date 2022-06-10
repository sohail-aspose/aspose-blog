---
title: 'Permanently Delete Messages from PST in C# using Aspose.Email for .NET'
date: Tue, 11 Apr 2017 15:51:15 +0000
draft: false
url: /2017/04/11/permanently-delete-messages-pst-using-aspose.email-.net/
author: Kashif Iqbal
summary: ''
tags: ['Delete Messages for PST in CSharp', 'PST Library .NET']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Aspose.Email-for-.NET_-1.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for .NET 17.4.0][1]. This month’s release comes with several enhancements related to Outlook messages and Storage files i.e. PST/OST. We have also fixed a number of bugs that further improves the overall functionality and stability of the API in terms of expected output. For a detailed note on what is new and fixed, please visit the [release notes][2] section of Aspose.Email for .NET 17.4.0.

## Delete Messages for PST in C#

**Deleting messages from PST permanently:** Consider a scenario where you are given a PST file and a set of messages that have been designated as attorney-client privileged. Given a list of entry IDs for those privileged messages, you are supposed to remove those messages and forward the PST to opposing legal counsel. If the deleted messages are recoverable by forensic tools, this defeats the purpose.

To help you with this, we are glad to share that this month’s release enhances the functionality of [deleting messages from a PST file][3] permanently. This means these messages are no more recoverable from the PST file with recovery tools. There is no public API change that you need to incorporate in your code to achieve this. Your existing code sample for deleting messages from the PST file will do the job for you with this latest release of the API.

{{< gist aspose-email 9e8fbeb51a8cbc4129dc71ca8cd55f0b "Examples-CSharp-Outlook-DeleteMessagesFromPSTFiles-DeleteMessagesFromPSTFiles.cs" >}}

## Support for PT\_FLOAT MAPI Property

This month’s release also provides support for a new Mapi property i.e. [PT\_FLOAT][4]. The API already supports other properties as well and the addition of this new one further enhances the list of such properties. The following code sample shows how to add such type of MAPI property to an Outlook message.

{{< gist aspose-com-gists 6e5185a63aec6fd70d83098e82b06a32 "Examples-CSharp-Outlook-SetAdditionalMAPIProperties-SetAdditionalMAPIProperties.cs" >}}

## Other Improvements

In addition to the enhancements mentioned above, this month’s release also includes several bug fixes for the issues reported by API users. Details about these can be found in the release notes section of our documentation.

## API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   [Product Documentation][5] – Provides detailed examples of working with the API
*   [API Reference Guide][6] – Details all the namespaces and classes of the API
*   [GitHub Examples][7] – Provides ready to run API example
*   [Support Forum][8] – Write to us if you have any query or inquiry about the API




[1]: https://downloads.aspose.com/email/net
[2]: https://docs.aspose.com/display/emailnet/Aspose.Email+for+.NET+17.4.0+Release+Notes
[3]: https://docs.aspose.com/display/emailnet/Working+with+Messages+in+a+PST+File#WorkingwithMessagesinaPSTFile-DeleteMessagesfromPSTFiles
[4]: https://docs.aspose.com/display/emailnet/Working+with+MAPI+Properties#WorkingwithMAPIProperties-SomeAdditionalProperties
[5]: https://docs.aspose.com/display/emailnet/Home
[6]: https://www.aspose.com/api/net/email
[7]: https://github.com/asposeemail/Aspose_Email_NET
[8]: https://forum.aspose.com/c/email




