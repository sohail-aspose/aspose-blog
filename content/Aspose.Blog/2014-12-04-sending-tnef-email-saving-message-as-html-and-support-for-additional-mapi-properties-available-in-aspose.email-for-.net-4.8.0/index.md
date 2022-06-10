---
title: 'Send TNEF Email, Save Message as HTML and Additional MAPI Properties Available in Aspose.Email for .NET 4.8.0'
date: Thu, 04 Dec 2014 15:41:02 +0000
draft: false
url: /2014/12/04/sending-tnef-email-saving-message-as-html-and-support-for-additional-mapi-properties-available-in-aspose.email-for-.net-4.8.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[![][1]](https://products.aspose.com/email)We are pleased to announce the release of Aspose.Email for .NET 4.8.0. This month’s release comes with a number of enhancements and bug fixes that bring more stability to the API functionality. Improvements include saving message to HTML, a feature for saving generic contacts, sending messages as TNEF, and support for additional MAPI properties. For further details about what is new and fixed, please visit the [product download page][2].

## Enhancements

This month’s release brings the following enhancements to the API.

**Sending email as TNEF:** This month’s release provides the capability to send an email in Transport Neutral Encapsulation Format (TNEF).  This helps preserve the message contents that may get disturbed during transmission otherwise. The SmtpClient’s UseTnef property can be set to true for all such TNEF emails before they are sent. More info.

**Provision of additional MAPI properties:** This month’s release provides support for some additional MAPI properties. These include PT\_MV\_FLOAT, PT\_MV\_R4, PT\_MV\_DOUBLE, PT\_MV\_R8, PT\_MV\_CURRENCY, PT\_MV\_APPTIME, PT\_MV\_I8, PT\_MV\_LONGLONG, PT\_MV\_CLSID, PT\_MV\_SHORT, PT\_MV\_SYSTIME, PT\_MV\_BOOLEAN, PT\_MV\_BINARY AND PT\_NULL. Find out more.

**Message conversion with additional options:** This month’s release introduces more generic classes for saving email messages to different output formats. These include SaveOptions, EmlSaveOptions, MsgSaveOptions and MhtSaveOptions. Each of these classes provide additional options for converting messages to other formats with specific requirements. Read more.

**Saving contacts:** This month’s release provides the capability to save contacts, retrieved from a Gmail client, in MSG as well as VCF format. This can be achieved by calling the Contact class' Save method.

**Enhanced message filtering based on date range:** The API’s ExchangeQueryBuilder allows you to retrieve emails from a Microsoft Exchange mailbox with specified criteria. This month’s release further strengthens this functionality by specifically searching for emails between date ranges.

## Bug Fixes

We have also fixed a number of bugs in this month’s release which further improves the overall API functionality. These include:

*   Encoding issues while conversion of messages to other formats.
*   Changes in appointment time during MSG to MHTML conversion.
*   Exceptions arose during EML to TIFF conversion, checking message signature, MSG to EML, loading specific EMLs, and others.
*   Additional contents rendering when converting a message to MHTML.

For a complete list of API changes, please visit our documentation section Public API changes in Aspose.Email for .NET 4.8.0. You may also share your feedback with us in the [Aspose.Email forum][3] for further assistance.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/12/aspose-Email-for-net_100.png "aspose-Email-for-net_100"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.email-for-.net/category1411.aspx
[3]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




