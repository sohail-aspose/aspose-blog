---
title: 'Working with Secondary Calendar Items on Office 365 supported with Aspose.Email for .NET 6.5.0'
date: Mon, 09 May 2016 14:44:20 +0000
draft: false
url: /2016/05/09/working-with-secondary-calendar-items-on-office-365-supported-with-aspose.email-for-.net-6.5.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[![][1]](https://products.aspose.com/email)We are pleased to announce the release of [Aspose.Email for .NET 6.5.0][2]. It includes new features, enhancements and bug fixes that not only enriches the API functionality but also brings further stability to the API. The product release notes of Aspose.Email for .NET contains all the information that is part of this month’s release and can also be referred for public API changes.

# New Features and Enhancements

**Binding SMTP Client to Specific IP on Host:** The possibility of a host having multiple IPs available for communication with external world cannot be ruled out. For example, consider the scenario where a server is equipped with multiple network cards, resulting in more than one IP addresses. In such case, the requirement may arise to bind the email sending client to a specific IP on the host for sending out emails. This can be achieved with Aspose.Email API using the SmtpClient's BindIPEndPoint property which is a new feature introduced in this month’s release.

**Inserting Header at Specific Location in Mail Headers:** The _Add_ method of _HeadersCollection_ inserts the header at the end of the collection. However, it may sometimes be necessary to insert a header at a specific location. In such case, the _Add_ method won't be of help. To achieve this, use the _Insert method_ of the _HeadersCollection_. If collection contains headers with the same name, this header will be inserted before other headers with the same name.

**Working with Events on Secondary Calendar using EWS:** Office 365 allows creating more than one Calendar folder and add appointment items to it. With this month’s release, Aspose.Email API now lets you create a secondary Calendar folder on Exchange Server using the _IEWSClient_. Appointments can then be added, updated or cancelled from the secondary calendar using the _CreateAppointment_, _UpdateAppointment_ and _CancelAppointment_ methods that are already provided by the API since a long time.

# Other Improvements

As mentioned earlier, this month’s release fixes a number of bugs that were reported by our valued customers with our last month’s version. In addition, these also include a number of other functional improvements as a result of our in-house quality testing.

# API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   Product Documentation – Provides detailed examples of working with the API
*   API Reference Guide – Details all the namespaces and classes of the API
*   [GitHub Examples][3] – Provides ready to run API example
*   [Support Forum][4] – Write to us if you have any query or inquiry about the API




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2016/05/Aspose.Email-for-.NET_.png "Aspose.Email for .NET"
[2]: http://www.aspose.com/downloads/email-family/net
[3]: https://github.com/asposeemail/Aspose_Email_NET
[4]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




