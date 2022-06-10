---
title: 'Send Calendar Invitations and Move Messages with IMAP Client in C#'
date: Sun, 17 Apr 2016 06:30:42 +0000
draft: false
url: /2016/04/17/sending-calendar-invitations-and-moving-messages-with-imap-client-using-aspose.email-for-.net-6.4.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Aspose.Email-for-.NET_.png" alt="Aspose.Email for .NET">}}


We are pleased to announce the release of [Aspose.Email for .NET 6.4.0][1] that comes with a number of new features, enhancements, and improvements. These include enhancements to the Exchange, MailMessage, MapiMessage, and Thunderbird storage processing APIs of the library. In order to get a complete list of changes and bug fixes that are part of this month’s release, please visit [Aspsoe.Email for .NET 6.4.0 Release notes][2].

# Send Calendar Invitation using C#

Aspose.Email API now lets you send [calendar invitations][3] using its Exchange Web Service (EWS) client. This requires, however, to delegate user rights to the receiver who the calendar invitation is sent.  The invitation must be sent by converting from MSG format to TNEF EML format using the IEWSClient of the API as illustrated in our documentation article, sending a calendar invitation.

## Move Message to other Folder with IMAP Client

This month's release introduces a new feature where the ImapClient API has been enhanced for [moving a message][4] from one folder to another. The _MoveMessage_ method of _ImapClient_ API provides this functionality using the message's unique id or sequence number.

## Search Messages with Paging Support using IMAP

We have also enhanced the API's IMAP client for searching messages with paging support simultaneously. The API now provides the _ListMessagesByPage_ method that takes ImapQueryBuilder and number of items per page as input parameters. This allows [listing filtered messages][5] from the server with control on the number of items to be retrieved per page.

## Save Messages as Microsoft Office Template (OFT) File

This month's release introduces another enhancement of saving messages as Microsoft Office Template (OFT) file. The [MailMessage][6], as well as [MapiMessage][7] API, can be used to save the messages as OFT file format.

## Independent implementation of Paging Support in Email Clients

We introduced features of paging support for listing messages, appointments and folders in IMAP as well as Exchange clients in one of our previous releases. The implementation, though providing the functionality, was not that much user friendly. This month's release now enhances this functionality by implementing it in separate classes. The new implementation provides ease of use and better understanding of the functionality.

## Set TimeZone Support for EWS Client

Aspose.Email API now provides support for setting the Timezone context for EWS Client. This can be achieved by setting the Timezone id as shown in the code sample below:

```
using (IEWSClient client = TestUtil.CreateEwsClient(server.User1))
{
  client.TimezoneId = "Central Europe Standard Time";
}
```

## Create Task with Zero Occurrences

This month’s release also enhances the functionality of creating a task. The API now supports creating an Outlook task with zero occurrences similar to Microsoft Outlook. This can be achieved by using the StartDate and EndDate properties of MapiCalendarRecurrencePattern.

## Other Improvements

This month's release also fixes a number of bugs reported with our earlier versions of the API. The product release notes of this month's version list all of these along with the status.

## API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   [Product Documentation][8] – Provides detailed examples of working with the API
*   [API Reference Guide][9] – Details all the namespaces and classes of the API
*   [GitHub Examples][10] – Provides ready to run API example
*   [Support Forum][11] – Write to us if you have any query or inquiry about the API




[1]: https://downloads.aspose.com/email/net
[2]: https://docs.aspose.com/display/emailnet/Aspose.Email+for+.NET+6.4.0+Release+Notes
[3]: https://docs.aspose.com/display/emailnet/Working+with+Calendar+Items+on+Exchange+Server
[4]: https://docs.aspose.com/display/emailnet/Working+with+Exchange+Mailbox+and+Messages#WorkingwithExchangeMailboxandMessages-MovingMessagesbetweenFolders
[5]: https://docs.aspose.com/display/emailnet/Filter+Messages+from+Server+using+IMAP+Client
[6]: https://docs.aspose.com/display/emailnet/Loading+and+Saving+Message
[7]: https://docs.aspose.com/display/emailnet/Managing+Message+Files+with+Aspose.Email.Outlook#ManagingMessageFileswithAspose.Email.Outlook-ReadingandWritingOutlookTemplateFile(.OFT)
[8]: https://docs.aspose.com/display/emailnet/Developer+Guide
[9]: https://apireference.aspose.com/email/net
[10]: https://github.com/aspose-email/Aspose.Email-for-.NET
[11]: http://forum.aspose.com




