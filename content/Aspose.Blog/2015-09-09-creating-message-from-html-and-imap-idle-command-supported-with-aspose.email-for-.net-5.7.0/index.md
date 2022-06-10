---
title: 'Creating Message from HTML and IMAP IDLE command supported with Aspose.Email for .NET 5.7.0'
date: Wed, 09 Sep 2015 14:24:35 +0000
draft: false
url: /2015/09/09/creating-message-from-html-and-imap-idle-command-supported-with-aspose.email-for-.net-5.7.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[![][1]](https://products.aspose.com/email)

We are pleased to announce the release of Aspose.Email for .NET 5.7.0. This month’s release brings new features, enhancements and a number of API improvements as a result of bug fixes. Our product download page, Public API Changes in Aspose.Email for .NET 5.7.0, lists all the changes that are part of this month’s release. To get further idea about what is new and fixed, please visit our [product download][2] page. In case of any query/inquiry related to the API, please write to us over [Aspose.Email forum][3] for assistance.

# New Features & Enhancments

**Loading MailMessage From HTML Content:** This month’s release includes a new feature of creating MailMessage from HTML file. The message is created with the specified html file and can include any inline images that are part of the html page. For this purpose, the resources on disc need to be specfieid using the load options.

**Support for IMAP Idle Command:** IMAP protocol in itself supports IDLE command. This month’s release enhances the IMAP client functionality and includes the support for this feature of IMAP protocol. The feature allows you to establish a connection and wait for a trigger when some message is received. This helps avoid polling the server all the time for any new incoming messages. The ImapClient’s StartMonitoring and StopMonitoring methods can be used to achieve this functionality. More Info

**Adding Headers to EWS Requests:** Microsoft Exchange Web Server (EWS) provides the facility of adding headers to the EWS client, in order to manage different Exchange level functionality. One such example is adding HttpHeaders such as X-AnchorMailbox that helps deal with the throtlling issues on Exchange Server. This month’s release enhances the API’s EWS Client to which headers can be added now. More Info

**Abillity to Perform Row-Wise Mail Merge:** Aspose.Email API provides the capability of creating/sending messages with dynamic content such as first name, last name, signature, etc. This is achieved using the API’s TemplateEngine class that adds the dynamic contetns and results in MessagesCollection. This month’s release further enhances this functionality by allowing row-wise mail merge. This gives control over the information added to the message as a single record and can be used to create meta-data about the generated message.

# Other Improvements

This month’s release also fixes a number of issues with the API in the form of bugs and exceptions. This includes:

*   Adding Calendar items to IPF.Note folder of PST
*   Issue with saving contents of an Outlook Contact
*   Problems with loading Aspose.Email’s generated messages in third party application
*   Exceptions related to Recurrence patterns
*   Problem with ListMessages method of the API’s EWS Client




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2015/09/aspose-Email-for-net_100.png "aspose-Email-for-net_100"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.email-for-.net/entry654649.aspx
[3]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




