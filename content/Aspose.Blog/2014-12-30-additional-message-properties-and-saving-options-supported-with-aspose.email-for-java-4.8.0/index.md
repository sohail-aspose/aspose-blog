---
title: 'Additional Message Properties and Saving Options in Java Email API'
date: Tue, 30 Dec 2014 09:56:15 +0000
draft: false
url: /2014/12/30/additional-message-properties-and-saving-options-supported-with-aspose.email-for-java-4.8.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for Java][1] 4.8.0 that comes with a number of enhancements and bug fixes.  These improvements include saving message to HTML, provision of additional properties to Outlook task and introduction of new options for saving messages. To get further details about what is new and fixed; please visit the [product download page][2]. For a list of public API changes in this month’s release, please visit the Public API changes in Aspose.Email for Java 4.8.0 documentation section.

**Provision of Additional Properties in MapiTask**

Aspose.Email already supports creating Outlook Tasks with setting a number of properties. This month’s release implements further properties of MapiTask from Office 365. Some of these include information related to company, category, mileage, billing, user information, sensitivity and status information. Some of these are also related to MapiMessage level and are common between these. More Info

## Saving message as HTML

This month’s release includes saving message body to HTML along with resources i.e. images. The API allows embedding resources as base 64 data in the HTML output. The SaveOptions can be used to control this embedding in the output HTML. More Info

## Additional Saving Options for MailMessage

With this month’s release, Aspose.Email now introduces more generic classes for saving email messages to different output formats. These include SaveOptions, EmlSaveOptions, MsgSaveOptions and MhtSaveOptions. These now enable users to convert messages to other formats with specific requirements. Find out more

## Provision of Additional MAPI Properties

This month’s release provides support for some additional MAPI properties. These include PT\_MV\_FLOAT, PT\_MV\_R4, PT\_MV\_DOUBLE, PT\_MV\_R8, PT\_MV\_CURRENCY, PT\_MV\_APPTIME, PT\_MV\_I8, PT\_MV\_LONGLONG, PT\_MV\_CLSID, PT\_MV\_SHORT, PT\_MV\_SYSTIME, PT\_MV\_BOOLEAN, PT\_MV\_BINARY AND PT\_NULL. Read More

## Bug Fixes

This month’s release also includes bug fixes as following:

*   Encoding lost while message conversion to other formats
*   MSG to MHTML conversion resulting in change of time
*   Rendering attachment contents to MHTML during conversion
*   Exceptions related to loading some ICS files and sending messages.




[1]: https://products.aspose.com/email/java
[2]: https://downloads.aspose.com/email/java




