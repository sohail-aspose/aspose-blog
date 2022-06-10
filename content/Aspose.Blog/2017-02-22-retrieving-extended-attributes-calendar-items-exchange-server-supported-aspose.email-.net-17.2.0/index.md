---
title: 'Retrieve Extended Attributes for Calendar Items on Exchange Server'
date: Wed, 22 Feb 2017 11:52:24 +0000
draft: false
url: /2017/02/22/retrieving-extended-attributes-calendar-items-exchange-server-supported-aspose.email-.net-17.2.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[![][1]](http://www.aspose.com/products/email/net)

We are pleased to announce the release of [Aspose.Email for .NET 17.2.0][2]. This month’s release introduces new features and enhancements related to different API functionality such as retrieving extended attributes for calendar items on Exchange server, rendering email message to MHTML and working with MBox files. It also fixes several bugs reported with the last version of the API, resulting in improved and stable functionality. For a detailed note on what is new and fixed, please visit the [release notes section][3] of product documentation.

# New Features and Enhancements

**Retrieving Extended Attributes Information for Calendar Items:** This month’s release introduces the first ever change in EWS API towards support of different kind of MAPI objects, resulting in support for MapiCalendar. This feature lets you [retrieve extended (nammed) properties][4] for calendar items from Exchange Server using its EWS client. The following methods offered by IEWSClient API can be used to retrieve calendar items from Exchange server with named properties.

*   **FetchMapiCalendar (calendar URIs)** – can be used to retrieve calendars from Exchange server with support for Nammed properties
*   **FetchMapiCalendar (calendar URIs, custom Properties)** – can be used to retrieve calendars from Exchange server with specified custom properties

We are also planning to provide support for creating, retrieving, and updating Extended attributes for other items as well such as Tasks, Notes and Contacts in our future releases.

**Getting Total Number of Items in Thunderbird Storage File:** Aspose.Email for .NET API supports working with Thunderbird’s storage file format i.e. MBox. It’s support for reading and writing messages to and from this file format is well known and effective. This month’s release enriches this functionality by providing [total number of items][5] in an MBox file. This information can be used to develop applications showing the overall progress of processing large MBox files.

**Provision of Auto-Detection of To and From Fields in Output MHTML:** This month’s release also enhances the feature of message conversion to MHTML by auto-formatting the message headers. This wasn’t supported earlier and MhtMessageFormatter need to be used to get the desired output. Due to this enhancement, MthMessageFromatter class is no more required and has been marked as deprecated. You can use the MhtSaveOptions to specify the additional options for achieving desired results as shown in our documentation article, [Rendering Calendar Events][6].

# Update Your Codes to Improved Namespace API version

It is the third consecutive month we have been publishing the legacy version of Aspose.Email API in parallel to the one with [improved namespace][7] structure. It is important to note that we won’t be publishing any further releases of the legacy API after this and it can break your codes in production if you download new releases from nugget. Therefore, we strongly recommend you to update your code samples to revamped version of the API to avoid any inconvenience.

# API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   [Product Documentation][8] – Provides detailed examples of working with the API
*   [API Reference Guide][9] – Details all the namespaces and classes of the API
*   [GitHub Examples][10] – Provides ready to run API example
*   [Support Forum][11] – Write to us if you have any query or inquiry about the API




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2016/12/Aspose.Email-for-.NET_-1.png
[2]: https://downloads.aspose.com/email/net
[3]: https://docs.aspose.com/display/emailnet/Aspose.Email+for+.NET+17.2.0+Release+Notes
[4]: https://docs.aspose.com/display/emailnet/Working+with+Calendar+Items+on+Exchange+Server#WorkingwithCalendarItemsonExchangeServer-RetrievingExtendedAttributesInformationfromCalendarItems
[5]: https://docs.aspose.com/display/emailnet/Programming+with+Thunderbird#ProgrammingwithThunderbird-GettingTotalNumberofMessagesfromMBoxFile
[6]: https://docs.aspose.com/display/emailnet/Loading+and+Saving+Message#LoadingandSavingMessage-RenderingCalendarEventswhileConvertingtoMHTML
[7]: https://blog.aspose.com/2016/12/26/aspose.email-.net-improved-namespace-structure-available-now/
[8]: https://docs.aspose.com/display/emailnet/Home
[9]: https://www.aspose.com/api/net/email
[10]: https://github.com/asposeemail/Aspose_Email_NET
[11]: https://forum.aspose.com/c/email




