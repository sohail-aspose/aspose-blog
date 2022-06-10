---
title: 'Forward Messages Using SMTP Client and Access Follow-Up Response using C#'
date: Fri, 06 Nov 2015 16:07:05 +0000
draft: false
url: /2015/11/06/forward-messages-using-smtp-client-and-access-follow-up-response/
author: Muhammad Waqas
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-net_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for .NET][1] 5.9.0. This month’s release contains a number of enhancements related to the API’s communication clients, message properties and recurrence patterns. It further improves the overall API functionality by fixing a number of issues reported with our last month’s release. A complete list of public API changes can be viewed by examining our documentation article, Public API changes in Aspose.Email for .NET 5.9.0.

## Forward Messages using SMTP with C#

In almost all commercially available email communication systems, email message forwarding is a common requirement where a message can be forwarded to specific recipients. This month’s release enhances the API’s SmtpClient to forward messages to specific recipients using the Forward method.

## Generating Recurrence from Recurrence Rule using C#

Aspose.Email API has the capability to parse Recurrence Rule, also known as RRULE defined as per RFC 5545 iCal specifications. This month’s release further enhances this functionality by providing the capability of generating Recurrence Pattern from such recurrence rules. The API’s _MapiCalendarRecurrencePatternFactory_ class provides the method to achieve this as demonstrated in our documentation article. More Info

## Access Follow-Up Information from Message

Follow up information refers to details shared by the receiver of message in response to sender’s request. This includes information such as delivery notification, read receipt delivery time, voting results and vote submission time. This month’s release adds new Mapi properties for retrieving such information from received messages. These properties are:

*   PR\_RECIPIENT\_TRACKSTATUS\_TIME\_DELIVERY
*   PR\_RECIPIENT\_TRACKSTATUS\_TIME\_READ
*   PR\_RECIPIENT\_AUTORESPONSE\_PROP\_RESPONSE
*   PR\_RECIPIENT\_TRACKSTATUS\_TIME

These can be retrieved as demonstrated in our documentation article, Accessing Follow-Up Information from Message.

## Copy Message from One Exchange Folder to another Folder

Aspose.Email API allows copying a message from one folder to another using the CopyItem method. This method has further been enhanced to return the copied message’s unique identifier that was not possible earlier. More Info

## Improved Exchange Connectivity Speed

We have enhanced the API’s Exchange Web Service (EWS) client in terms of connectivity speed as compared to other commercially available APIs. With this improvement, the API now connects to Exchange server with notable improvements.

## Other Improvements

This month’s release also fixes a number of bugs related to various functional areas of the API. For a complete of these, please visit our product download page.

## API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   [Product Documentation][2] – Provides detailed examples of working with the API
*   [API Reference Guide][3] – Details all the namespaces and classes of the API
*   [GitHub Examples][4] – Provides ready to run API example
*   [Support Forum][5] – Write to us if you have any query or inquiry about the API




[1]: https://products.aspose.com/email/net
[2]: https://docs.aspose.com/email/net
[3]: https://apireference.aspose.com/email/net
[4]: https://github.com/asposeemail/Aspose_Email_NET
[5]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




