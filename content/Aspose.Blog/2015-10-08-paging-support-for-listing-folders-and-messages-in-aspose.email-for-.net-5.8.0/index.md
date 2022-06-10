---
title: 'Use Paging for Listing Folders and Messages in Exchange Mailbox using C#'
date: Thu, 08 Oct 2015 15:26:27 +0000
draft: false
url: /2015/10/08/paging-support-for-listing-folders-and-messages-in-aspose.email-for-.net-5.8.0/
author: Muhammad Waqas
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-net_1001.png" alt="">}}


[Aspose.Email for .NET][1] 5.8.0 has been released. It includes enhancements and bug fixes to a number of API functional areas. Specifically, it provides the capability of paging while retrieving information from Exchange Mailbox and offers new load options for loading specific type of messages. Our documentation section, Public API Changes in Aspose.Email for .NET 5.8.0, provides complete list of changes that are part of this month’s release.

## Enumerating Folders with Paging Support using EWS

The Exchange Web Service (EWS) client of the API now supports enumerating folders with paging support. This feature provides the capability to retrieve the list of folders from the exchange server in multiple server responses. User can now specify the maximum number of folders information to be retrieved from the server in a go.  For an illustration example of this feature, please visit our documentation article, Listing Sub Folders from Exchange Server.

## Enumerating Messages with Paging Support using EWS

The API provides the paging support for listing messages as well in addition to listing sub folders. This is very helpful where the mailbox has a large number of messages and requires a lot of time for retrieving the summary information about these. Example usage of this enhancement can be seen in our documentation article, Fetch Messages from Exchange Server.

## New Loading Options for Specific Message Types

This month’s release provides new message loading options for specific message types. This standardizes loading messages with standard load options that can be used to specify the message specific arguments. These new classes are:

*   EmlLoadOptions
*   HtmlLoadOptions
*   MhtmlLoadOptions
*   MsgLoadOptions
*   TnefLoadOptions
*   EmlxLoadOptions

Old classes for loading messages have been marked as deprecated and will be removed in subsequent versions. Our documentation article, importing and exporting messages, gives detailed example of using these new message loading options.

## Other Improvements

We have also fixed a number of bugs reported with our last month’s release. Our [product download page][2] lists all of these along with new features and enhancements.

## API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   [Product Documentation][3] – Provides detailed examples of working with the API
*   [API Reference Guide][4] – Details all the namespaces and classes of the API
*   [GitHub Examples][5] – Provides ready to run API example
*   [Support Forum][6] - Write to us if you have any query or inquiry about the API




[1]: https://products.aspose.com/email/net
[2]: https://downloads.aspose.com/email/net
[3]: https://docs.aspose.com/email/net
[4]: https://apireference.aspose.com/email/net
[5]: https://github.com/asposeemail/Aspose_Email_NET
[6]: http://forum.aspose.com




