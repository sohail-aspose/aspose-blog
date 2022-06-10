---
title: 'Split PST Files with defined Criterion using C#'
date: Thu, 11 Aug 2016 17:26:32 +0000
draft: false
url: /2016/08/11/splitting-pst-file-with-defined-criterion-supported-with-aspose.email-for-.net-6.8.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Aspose.Email-for-.NET_.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for .NET 6.8.0][1]. This month’s release a new feature of splitting a PST based on specific search criterion. It also provides enhancement to the API’s IMAP client that is now able to move folders to other folders of a mailbox. This month’s release also fixes a number of bugs that further adds to the overall stability of the API. For further details on what is new and fixed, please visit the [release notes section][2] of this month’s release.

## Split PST File Based on Search Criterion in C#

Aspose.Email API already provides the capability of splitting a single large PST file into multiple small PST files. This month’s release further enhances this feature by providing the capability to [split PST][3] based on defined criterion. The API now provides support for specifying multiple criterion using _PersonalStorageQueryBuilder_. This allows to include multiple search criterion such as time and subject simultaneously for splitting the PST.

## Detection of Message as TNEF

This month’s release also provides the capability of detecting whether the loaded email message was originally TNEF. The _MailMessage_ API now provides the _OriginalIsTnef_ property that detects the [message as TNEF][4].

## Retrieving Message Summary Information using Message’s Unique Id

A message’s unique id is always its representation and can be used to store a reference of the message as meta-data.  Retrieving of the same message from the email server can be obtained through the same. This month’s release further enhances the POP3 Client of the API to retrieve message summary information from the server using this unique id of the message. This provides quick access to the message’s short information without first retrieving the complete message from the server.

## Other Improvements

In addition to new features and enhancements, this month’s release also fixes a number of bugs that were reported with the previous version of the API. It further enhances the stability and reliability of the API functionality.

## API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   [Product Documentation][5] – Provides detailed examples of working with the API
*   [API Reference Guide][6] – Details all the namespaces and classes of the API
*   [GitHub Examples][7] – Provides ready to run API example
*   [Support Forum][8] – Write to us if you have any query or inquiry about the API




[1]: http://www.aspose.com/downloads/email/net
[2]: http://docs.aspose.com/display/emailnet/Aspose.Email+for+.NET+6.8.0+Release+Notes
[3]: http://docs.aspose.com/display/emailnet/Splitting+and+Merging+PST+files#SplittingandMergingPSTfiles-SplitPstOnCriterion
[4]: https://docs.aspose.com/display/emailnet/Utility+Features+-+MailMessage#UtilityFeatures-MailMessage-EmailmessagescontainingTNEFattachments
[5]: http://docs.aspose.com/display/emailnet/Programmers+Guide
[6]: http://docs.aspose.com/display/emailnet/Aspose.Email+for+.NET++API+Reference
[7]: https://github.com/asposeemail/Aspose_Email_NET
[8]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




