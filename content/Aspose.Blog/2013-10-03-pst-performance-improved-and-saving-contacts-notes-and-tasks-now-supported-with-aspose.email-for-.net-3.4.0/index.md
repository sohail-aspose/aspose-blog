---
title: 'Improved PST Performance and Saving Contacts, Notes and Tasks Supported in Aspose.Email for .NET 3.4.0'
date: Thu, 03 Oct 2013 14:33:46 +0000
draft: false
url: /2013/10/03/pst-performance-improved-and-saving-contacts-notes-and-tasks-now-supported-with-aspose.email-for-.net-3.4.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Email-for-net_100.png)Aspose.Email for .NET 3.4.0 has been released with a number of enhancements and new features along with bug fixes.

This month’s release includes a major enhancement to the PST functionality that improves its performance when adding large amounts of data. This enhancement reduces the overall disc I/O operations and, as a result, enhances the overall speed of adding Outlook MSG files to the PST. In addition, the AddMessages method has been added, It lets you copy a collection of messages to a PST folder. For a detailed example, refer to the Adding Bulk Messages article from our online documentation.

Creating contacts, tasks and notes and adding them to PST had been supported in our earlier versions. However, saving these as an MSG file to disc or stream was not available. With this month’s release, creating and saving contacts, tasks and notes as MSG files is supported. In addition, adding photo data to an Outlook contact, a feature that was missing, is also supported.

With this month’s release, conversion of S/MIME messages from EML to MSG (and vice versa) with preserving digital signatures is supported. The preserveSignature parameter in the MapiMessage.FromMailMessage method preserves the digital signature during conversion.

This month’s release also includes a number of bug fixes reported by our customers. Specific to PST, the issue of large PST file size (created with Aspose.Email) as compared to those created with Outlook, has been fixed. Other issues such as message encoding disturbance during conversion of MSG to EML, message ID truncation, linked resources and others have also been fixed in this month’s release.

For more details about what is new and fixed, please visit the [Aspose.Email for .NET][2] release page.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Email-for-net_100.png "Aspose.Email for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.email-for-.net/category1411.aspx




