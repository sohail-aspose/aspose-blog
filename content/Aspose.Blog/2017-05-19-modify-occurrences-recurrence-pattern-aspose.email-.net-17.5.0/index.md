---
title: 'Modify Occurrences from Recurrence Pattern in Outlook Calendar using C#'
date: Fri, 19 May 2017 17:26:51 +0000
draft: false
url: /2017/05/19/modify-occurrences-recurrence-pattern-aspose.email-.net-17.5.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Aspose.Email-for-.NET_-1.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for .NET 17.5.0][1]. This month’s release includes a new feature to modify or delete an occurrence from a recurrence pattern. It also includes several enhancements related to different API functionality. All these changes have been documented in the release notes section of the API documentation for the user’s reference.

## Modify or Delete Occurrence from Recurrence Pattern

Aspose.Email API allows working with recurrence patterns for Outlook Calendar items. This month’s release further enriches this feature of the API by allowing to [modify or delete a specific occurrence][2] from a recurrence pattern. This is achieved by adding an exception to the occurrences of a recurrence pattern as shown in the following code sample.

{{< gist aspose-com-gists 6e5185a63aec6fd70d83098e82b06a32 "Examples-CSharp-Outlook-ModifyDeleteOccurrenceInRecurrence-ModifyDeleteOccurrenceInRecurrence.cs" >}}

## Filter Messages by Message Size using EWS

Want to filter messages from the Exchange server based on message size? We have implemented this feature by incorporating the [MessageSize search parameter][3] in ExchangeQueryBuilder. Messages can be filtered from Exchange server based on message size as illustrated in the code sample below.

{{< gist aspose-com-gists 6e5185a63aec6fd70d83098e82b06a32 "Examples-CSharp-Exchange_EWS-FilterMessagesOnCriteriaUsingEWS-FilterMessagesByMessageSize.cs" >}}

## Forward Messages without loading using MailMessage

We have other good news for people whose environments consist of low resources such as system memory. Such a situation can give rise to problems sometimes including out of memory exceptions while loading large message files. This month’s version now provides the capability to load the file in file stream and send it using the [API’s SMTP client][4] without using MailMessage.

## Get Folder Type Information using EWS

This month’s release also provides the capability to get [folder type information][5] for the folders retrieved from Exchange server. The EWS API lets you get this information from ExchangeFolderInfo with the FolderType enumeration introduced in this month’s release.

## Get Message Class Information using EWS

You can also get [message class information][6] from the message’s summary information i.e. ExchangeMessageInfo. The information is available in the MessageInfoType property of ExchangeMessageInfo and gives the message class for the selected item.

## Other Improvements

This month’s release also fixes several bugs related to API functionality. Fixing these not only improves the overall API functionality but also stabilizes the API’s behaviors in terms of expected results.

## API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   [Product Documentation][7] – Provides detailed examples of working with the API
*   [API Reference Guide][8] – Details all the namespaces and classes of the API
*   [GitHub Examples][9] – Provides ready to run API example
*   [Support Forum][10] – Write to us if you have any query or inquiry about the API




[1]: https://downloads.aspose.com/email/net/new-releases/aspose.email-for-.net-17.5.0/
[2]: https://docs.aspose.com/display/emailnet/Working+with+Calendar+Items+in+PST+File#WorkingwithCalendarItemsinPSTFile-Modify/DeleteOccurrencesfromRecurrences
[3]: https://docs.aspose.com/display/emailnet/Filter+Messages+From+Exchange+Mailbox#FilterMessagesFromExchangeMailbox-FilterbyMessageSize
[4]: https://docs.aspose.com/display/emailnet/Sending+and+Forwarding+Messages#SendingandForwardingMessages-ForwardingEmailwithoutusingMailMessage
[5]: https://docs.aspose.com/display/emailnet/Working+with+Folders+on+Exchange+Server#WorkingwithFoldersonExchangeServer-GetFolderTypeInformationusingEWS
[6]: https://docs.aspose.com/display/emailnet/Working+with+Exchange+Mailbox+and+Messages#WorkingwithExchangeMailboxandMessages-GettingMessageTypeInformationfromExchangeMessageInfo
[7]: https://docs.aspose.com/display/emailnet/Home
[8]: https://www.aspose.com/api/net/email
[9]: https://github.com/asposeemail/Aspose_Email_NET
[10]: https://forum.aspose.com/c/email




