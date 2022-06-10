---
title: 'Reading Multiple Events from ICS Calander in C# .NET'
date: Wed, 12 Jul 2017 06:16:39 +0000
draft: false
url: /2017/07/12/reading-multiple-events-ics-file-aspose.email-.net-17.7/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Aspose.Email-for-.NET_-1.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for .NET 17.7][1]. This month’s release includes several enhancements to various functional areas of the API. It also fixes a number of bugs previously reported by our valued customers. You can find a complete list of what is new and fixed in [release notes][2] section of the API documentation.

## Read Multiple Events from ICS Calander in C#

Aspose.Email API can now read multiple events from the Calendar file as an individual appointment. Reading multiple events from the ICS file was not supported earlier. With this enhancement, events from the ICS file can now be retrieved and stored as a collection of Appointments in the user’s defined code as shown below.

{{< gist aspose-com-gists 6e5185a63aec6fd70d83098e82b06a32 "Examples-CSharp-Email-ReadMultilpleEventsFromICS-ReadMultilpleEventsFromICS.cs" >}}

## Filtering Messages with Paging from Exchange Server

This month’s release also provides support for [filtering messages][3] from the Exchange server with paging support. This helps manage the list of messages retrieved from the server for handling them easily.

{{< gist aspose-com-gists 6e5185a63aec6fd70d83098e82b06a32 "Examples-CSharp-Exchange_EWS-FilterMessagesOnCriteriaUsingEWS-FilterMessagesWithPagingSupport.cs" >}}

## Preserving Embedded Message Format

MIME messages can have further embedded messages as attachments. The API used to convert these embedded messages to EML format by default which may not be the expected behavior in some user scenarios. This month’s release provides more control to the user for [preserving embedded message][4] format using the EMLLoadOptions class.

## Getting Message Size from Thunderbird MBox

This month’s release also gives the facility to [get message size][5] while reading from MBox file.

## API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   [Product Documentation][6] – Provides detailed examples of working with the API
*   [API Reference Guide][7] – Details all the namespaces and classes of the API
*   [GitHub Examples][8] – Provides ready to run API example
*   [Support Forum][9] – Write to us if you have any query or inquiry about the API




[1]: https://downloads.aspose.com/email/net
[2]: https://docs.aspose.com/display/emailnet/Aspose.Email+for+.NET+17.7+Release+Notes
[3]: https://docs.aspose.com/display/emailnet/Filter+Messages+From+Exchange+Mailbox#FilterMessagesFromExchangeMailbox-FilteringMessageswithPagingSupport
[4]: https://docs.aspose.com/display/emailnet/Loading+and+Saving+Message#LoadingandSavingMessage-PreservingEmbeddedMessageFormatduringLoading
[5]: https://docs.aspose.com/display/emailnet/Programming+with+Thunderbird#ProgrammingwithThunderbird-GetCurrentMessageSize
[6]: https://docs.aspose.com/display/emailnet/Home
[7]: https://www.aspose.com/api/net/email
[8]: https://github.com/asposeemail/Aspose_Email_NET
[9]: https://forum.aspose.com/c/email




