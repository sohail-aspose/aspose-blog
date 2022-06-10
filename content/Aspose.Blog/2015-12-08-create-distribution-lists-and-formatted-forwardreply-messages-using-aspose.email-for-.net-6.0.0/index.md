---
title: 'Create Distribution Lists and Formatted Forward/Reply Messages using Aspose.Email for .NET 6.0.0'
date: Tue, 08 Dec 2015 15:29:43 +0000
draft: false
url: /2015/12/08/create-distribution-lists-and-formatted-forwardreply-messages-using-aspose.email-for-.net-6.0.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[![][1]](http://www.aspose.com/.net/email-component.aspx)

[Aspose.Email for .NET 6.0.0][2] has been released. We have included new features and enhancements in this month’s release to reduce the gap between the MS Outlook and Aspose.Email for .NET API features. It also includes fixes to a number of issues that were reported by our valued customers. Our documentation section, public API changes, includes details about the API changes in this month’s release.

# New Features

**Working with Distribution Lists on Exchange Server:** Microsoft Outlook provides the capability to add distribution lists to Exchange server account. This month’s release of Aspose.Email API provides the capability of working with Distribution lists on Exchange Server. It provides the support for:

*   Creating Private Distribution List
*   Fetching Distribution List from Exchange Server
*   Adding Members to Private Distribution List
*   Delete Members from a Distribution List
*   Delete the Distribution List
*   Sending Message to a Distribution List
*   Creating MailAddress from Distibution List Id
*   Expanding Public Distribution List

For a complete example, please visit our documentation article, Working with Distribution Lists on Exchange Server.

**Creation and Formatting Forward and Reply Messages:** This month’s release also includes a new feature of creating and formatting Forward and Reply messages. Such type of messages can be generated using the MapiMessage as well as MailMessage classes of the API. User can add required information to the generated messages as specified by the OriginalMessageAdditionMode enumerator. It has three options as follow:

*   **OriginalMessageAdditionMode.None** - The original message is not included in response message.
*   **OriginalMessageAdditionMode.Attachment** - The original message is included as attachment in response message
*   **OriginalMessageAdditionMode.Textpart** - The original message is included as text in body of response message

# Enhancements

**Getting Exchange Message Summary Information from Message URI:** Exchange server provides summary about messages retrieved in the form of _ExchangeMessageInfo_. It contains information such as Subject, Recipients, Time, and some other fields along with message unique identifier i.e. Message URI. It is a good idea to store message URIs for lateral referencing and later on retrieve the summary information using this identifier. This month’s release provides the capability to achieve this by providing an overloaded method of _ListMessages_ that accepts a list of string identifiers. This overloaded method returns _ExchangeMessageInfoColleciton_ that is a collection of summary information of all the messages for provided URIs. More Info

**Performance Improvement:** This month’s release also addresses an issue with the API performance where the _MailMessage_ API takes a lot of memory and considerable CPU utilization. The issue has been fixed, resulting in improvement of the API performance.

# Other Improvements

This month's release also fixes a number of bugs that were reported with our last month's release. A complete list of these can be viewed by visiting our [product download page][3].

# API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   Product Documentation – Provides detailed examples of working with the API
*   API Reference Guide – Details all the namespaces and classes of the API
*   [GitHub Examples][4] – Provides ready to run API example
*   [Support Forum][5] – Write to us if you have any query or inquiry about the API




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2015/12/aspose-Email-for-net_100.png "aspose-Email-for-net_100"
[2]: https://www.aspose.com/templates/aspose/App_Themes/V3/images/words/272x272/aspose_words-for-net.png
[3]: https://www.aspose.com/templates/aspose/App_Themes/V3/images/words/272x272/aspose_words-for-net.png
[4]: https://github.com/asposeemail/Aspose_Email_NET
[5]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




