---
title: 'Read OST 2013 and 2016 Formats using C# with Aspose.Email for .NET 6.2.0'
date: Tue, 09 Feb 2016 15:16:04 +0000
draft: false
url: /2016/02/09/reading-ost-2013-and-2016-formats-supported-with-aspose.email-for-.net-6.2.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-net_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for .NET 6.2.0][1]. This month’s release includes a number of new features, enhancements and bug fixes that further aids to the list of features supported by the API. To get a quick view about what is new and fixed, please visit our product download page. For a complete list of API changes in this month's release, please visit our documentation section, public API Changes in Aspose.Email 6.2.0.

## Support for OST 2013/2016 Formats

This month of release introduces a new feature of reading Offline Storage (OST) files 2013 and 2016 formats. We refer to it as the most demanding feature from our customers as it was creating limitations for them in manipulating these specific OST formats. However, it should be noted that, at present, the API only supports reading these OST formats and support for writing/updating is unavailable.

## Paging for Listing Appointments from Exchange Server

This month’s release also enhances the functionality of listing appointments from Microsoft Exchange Server in case there are large number of appointments available. The functionality has been enhanced so that user can specify the number of items per page while listing appointments from server. This provides the capability to get list of appointments quickly by limiting the retrieved list’s count per page. A number of overload methods of _ListAppointments_ have been provided that also include the option of including MailQuery as input parameter. For a detailed and working example, please visit our documentation article, Listing Appointments with Paging Support.

## Paging for Listing Message using IMAP

In addition to listing appointments with paging support on Exchange server, this month’s release also provides paging support while retrieving messages using the API’s ImapClient. This helps retrieve messages from server as per requirements specified in items per page. For a detailed example on this feature, please visit our documentation article, Listing Messages with Paging Support.

## Managing Outlook MSG Attachments in Messages

This month’s release also includes a new feature of manipulating attachments in messages with RTF body. It introduces two new methods to insert and replace attachments in such a message. The **Insert** method allows to insert an embedded message at a specific index in RTF body. The **Replace** method provides the capability to replace the embedded message contents with the new ones. Our documentation article, Attachments Insertion and Replacement, provides a detailed example of these new methods.

## Getting Specific Contact from Exchange Server

Aspose.Email API already provides the capability to get contacts from Exchange server using its Exchange Web Service (EWS) client. However, it may not always be necessary to get all the contacts from Exchange server. In order to fetch only a single contact using its id, this month’s release provides a new method, GetContact, that can be used to fetch a contact from exchange server using the contact Id.

## Reading Complete Embedded Message from Attachment

Outlook messages may further contain embedded messages as attachments. The API’s _MapiMessage.FromProperties_ creates a bare bone email template from such embedded message’s properties but it is never a complete message. With this month’s release, it is now possible to extract complete message from such an attachment’s object data.

## Other Improvements

This month’s release also includes a number of bug fixes that further improve the overall API functionality. A list of bug fixes can be viewed by visiting the [release notes][2] of Aspose.Email for .NET 6.2.0.

## API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   Product Documentation – Provides detailed examples of working with the API
*   API Reference Guide – Details all the namespaces and classes of the API
*   [GitHub Examples][3] – Provides ready to run API example
*   [Support Forum][4] – Write to us if you have any query or inquiry about the API




[1]: https://www.aspose.com/templates/aspose/App_Themes/V3/images/words/272x272/aspose_words-for-net.png
[2]: https://www.aspose.com/templates/aspose/App_Themes/V3/images/words/272x272/aspose_words-for-net.png
[3]: https://github.com/asposeemail/Aspose_Email_NET
[4]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




