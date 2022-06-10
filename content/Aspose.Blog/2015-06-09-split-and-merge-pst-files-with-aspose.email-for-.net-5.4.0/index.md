---
title: 'Split and Merge PST Files using C# or VB.NET'
date: Tue, 09 Jun 2015 17:41:05 +0000
draft: false
url: /2015/06/09/split-and-merge-pst-files-with-aspose.email-for-.net-5.4.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-net_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for .NET 5.4.0][1]. This month’s release brings new features and enhancements related to various functional areas of the API. In addition, it also includes a number of API improvements by fixing a number of bugs reported with our earlier version. For a complete list of API changes, you may visit our documentation article [Public API Changes in Aspose.Email 5.4.0][2]

## Split and Merge PST files using C#

This month’s release introduces the long-awaited feature of splitting large PST files and merging small PST files into a single file.

A PST can be split into multiple smaller files using the _SplitInto_ method of the _PersonalStorage_ class that allows specifying the size of the resultant PST files and the destination folder to store these.

For merging multiple PST files into a single file, the _PersonalStorage_ class provides the method _MergeWith_ method. This merges the files from the specified folder with the loaded PST file. The feature also provides the capability to merge folders from another PST file using the overloaded member of _MergeWith_.

For detailed code samples, please visit our online documentation article [Splitting and Merging PST files][3].

## Processing of Bounced Messages

Messages sent to recipients may often fail to deliver for a number of reasons such as invalid recipient addresses. This month’s release now provides the capability to process such bounced messages and extract the service information from such a message. The API introduces new class, _BounceResult_, which contains the information if a message is bounced. For sample code, please visit our documentation article [Processing of Bounced Messages][4].

## Enhancements

**Saving Exchange Task to Disc:** Aspose.Email’s EWS client already provides support for working with Tasks on Exchange server. This month’s release provides the capability to [save Exchange Task][5] to disc in Outlook MSG format.

**OAuth Support for EWS with Office 365:** Sometimes it is desired to access Office 365 mailbox without providing username and password such as in case of the corporate environment. We are pleased to share that Aspose.Email for .NET now provides this capability by connecting to the Office 365 EWS using OAuth. [More Info][6]

**Other Enhancements:** This month’s release also includes some other API enhancements for improved API functionality. These include:

*   Support for Cryillic characters to message headers
*   Setting SentRepresentingEmailAddress to Exchange format address
*   Support for Asynchronous operations based on sequence number to the IMAP and POP3 client

# Bug Fixes

This month’s release also includes a number of bug fixes that further improves the overall API functionality. Complete details of these are available at our [Product download page][7]. These include:

*   Issues related to the encoding while converting message to different formats
*   Hanging issues while loading certain email messages
*   Issues with message encryption, decryption and signing
*   Multiple issues related to Outlook tasks
*   Exceptions while saving certain messages, deleting tasks and resolving contacts from Exchange server, and loading certain calendar files




[1]: https://downloads.aspose.com/email/net
[2]: http://docs.aspose.com/display/emailnet/Public+API+Changes+in+Aspose.Email+5.4.0
[3]: http://docs.aspose.com/display/emailnet/Splitting+and+Merging+PST+files
[4]: https://docs.aspose.com/display/emailnet/Utility+Features+-+MailMessage#UtilityFeatures-MailMessage-ProcessingofBouncedMessages
[5]: http://docs.aspose.com/display/emailnet/Working+with+Tasks+on+Exchange+Server#WorkingwithTasksonExchangeServer-SaveTask
[6]: https://docs.aspose.com/
[7]: https://downloads.aspose.com/email/net




