---
title: 'Reduced PST Size and Case-Sensitive Email Filtering Supported by Aspose.Email for .NET 4.7.0'
date: Tue, 04 Nov 2014 16:53:08 +0000
draft: false
url: /2014/11/04/reduced-pst-size-and-case-sensitive-email-filtering-supported-with-aspose.email-for-.net-4.7.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[![][1]](http://www.aspose.com/.net/email-component.aspx)We are pleased to announce the release of Aspose.Email for .NET 4.7.0. This month’s release brings a number of enhancements to the existing functionality of the API and fixes issues that were reported with our last month’s version. This further improves the overall functionality of the API and gives stability to the existing features. To get an idea about what is new and fixed, please visit our [product download page][2]. You may also visit our product documentation for detailed notes on Public API Changes in Aspose.Email for .NET 4.7.0.

## Enhancements

The enhancements included in this version are detailed as follow.

**Case-sensitive email filtering in email clients:** The API’s email clients - IMAP, POP3 and EWS - already provide the capability to retrieve emails from servers based on filter criteria. This feature has been further improved by case-sensitive filtering for all these clients.

**Setting timezone on Exchange task**: The Exchange Web Service (EWS) client offered by Aspose.Email provides the capability of working with Exchange tasks. This month’s release further improves this functionality by specifying the time zone for the client as well as the Exchange task. More info.

**Improved rendering options to MHTML**: Aspose.Email can render emails to MHTML format. This month’s release further improves this functionality by providing the capability of writing the To, From, CC and BCC fields to the output. This enables developers to control the output as per requirements during conversion of email messages to MHTML. More info.

**Move items on Exchange Server**: This month’s release brings further improvements to the functionality of moving email messages from one folder to another folder. The earlier versions of the Aspose.Email API required users to manually write the exact destination folder URI for such purpose. Now, this operation requires only the source message URI and destination folder URI statement. More info.

**Provision of body compression:** Aspose.Email now makes it possible to reduce the message size by using RTF body compression. This allows developers to create a smaller size PST, though at the cost of speed. If speed is desired, then set the UseBodyCompression property to false to turn compression off. More info.

**Creating TNEF MailMessage from MapiMessage:** Outlook MSG files sometimes contain information such as tables and text styles that may get disturbed when converted to EML. Creating TNEF messages from such MSG files allows developers to retain the formatting and even sending such messages via the email clients. The InterpretAsTnef property is used to achieve this. More Info

## Bug Fixes

This month’s release also fixes a number of bugs that were reported with our last month’s version. Fixing these further improves the overall functionality of the API and includes:

*   Pop3Client functionality with Hotmail email.
*   Improved PST creation speed.
*   Encoding issues during message conversions.
*   Outlook opening issues in PSTs.
*   Exceptions such as saving calendar items to memory stream, fetching messages using EWS and loading messages from file.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/11/aspose-Email-for-net_100.png "aspose-Email-for-net_100"
[2]: https://www.aspose.com/templates/aspose/App_Themes/V3/images/words/272x272/aspose_words-for-net.png




