---
title: 'Listing Messages and Folders From Exchange Server with Paging Support using Aspose.Email for Java 5.8.0'
date: Wed, 14 Oct 2015 05:57:40 +0000
draft: false
url: /2015/10/14/listing-messages-and-folders-from-exchange-server-with-paging-support-using-aspose.email-for-java-5.8.0/
author: Muhammad Waqas
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

![](https://blog.aspose.com/wp-content/uploads/sites/2/2015/10/aspose-Email-for-Java_1001.png "aspose-Email-for-Java_100")

We are pleased to announce the release of Aspose.Email for Java 5.8.0. This month’s release includes enhancements to the existing functionality of the API and bug fixes that results in the overall API stability. It provides the capability to retrieve messages and folders from the Exchange Server with paging support. You can find complete list of changes in this month’s release by visiting our documentation article, Public API Changes in Aspose.Email for Java 5.8.0.

# Enhancements

**Folders Enumeration with Paging Support in EWS:** This month’s release provides the capability to retrieve folders information from Exchange server with paging support. Folders from exchange server can, thus, be retrieved in multiple server responses by specifying the maximum number of folders to fetch. More Info

**Enumerating Messages with Paging Support in EWS:** Similar to Folders enumeration with paging support, the API now provides the capability to list messages from Exchange server with paging support in EWS. This helps in retrieving the message’s summary information from large mailboxes that, otherwise, take much time. More Info

**Options for Loading Specific Message Types:** This month’s release also provides specific classes for loading various message types. Each type of message can be loaded using these new classes and specifying additional options. The old classes have been marked as deprecated and will be removed in future versions of the API. The new classes are as follow:

*   _EmlLoadOptions_
*   _HtmlLoadOptions_
*   _MhtmlLoadOptions_
*   _MsgLoadOptions_
*   _TnefLoadOptions_
*   _EmlxLoadOptions_

Our documentation article, Update and Save an Email, demonstrates the usage of these new message loading options.

# Performance Improvements

This month's release improves the performance of Exchange API on Mac OS. Earlier, the API took much time to connect to Exchange Server and retrieve the list of messages. This has now been improved. In addition, the API also improves the speed of loading messages having large number of recipients.

# Bug Fixes

This month’s release also fixes a number of bugs that caused hampering in achieving the desired output. A complete list of bug fixes can be found by visiting our [product download page][1].

# API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   Product Documentation – Provides detailed examples of working with the API
*   API Reference Guide – Details all the packages and classes of the API
*   [GitHub Examples][2] – Provides ready to run API examples
*   [Aspose.Email Forum][3] – Feel free to contact us on Aspose.Email forum for your queries




[1]: http://www.aspose.com/community/files/72/java-components/aspose.email-for-java/entry662459.aspx
[2]: https://github.com/aspose-email/Aspose.Email-for-Java
[3]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




