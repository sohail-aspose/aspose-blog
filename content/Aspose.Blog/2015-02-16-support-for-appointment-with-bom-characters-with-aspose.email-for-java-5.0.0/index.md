---
title: 'Appointments having BOM Characters supported with Aspose.Email for Java 5.0.0'
date: Mon, 16 Feb 2015 18:23:07 +0000
draft: false
url: /2015/02/16/support-for-appointment-with-bom-characters-with-aspose.email-for-java-5.0.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

![](https://blog.aspose.com/wp-content/uploads/sites/2/2015/02/aspose-Email-for-Java_100.png "aspose-Email-for-Java_100")

We are pleased to share the release of Aspose.Email for Java 5.0.0. Ported form its equivalent .NET version, it incorporates the same enhancements and bug fixes. For a complete list of API changes, you may visit the public API changes in Aspose.Email for Java 5.0.0 page of our documentation section. For any query/inquiry related to the API, please feel free to write to us [Aspose.Email forum][1].

# Enhancements

Enhancements included in this month’s release are as follow:

**Support for Managing Password property of a PST:** Aspose.Email already provides the support for checking a PST for password protection. This month’s release further enhances this capability by allowing user to reset the password property of the PST using the PST’s message store. In order to remove/reset this property, the value is set to zero (0) for getting it removed. A new property, known as Store, has been introduced in this month’s release for this purpose. For a working code sample, please have a look at our documentation article, Working with PST Password Protection Properties.

**Support for loading Appointments with Byte Order Mark (BOM) Characters:**  With this month’s release, you can load appointments having Byte Order Mark (BOM) characters at their start. Though BOM use is optional, this was not supported earlier with the API. The same Appointment class’s load method can be used to load such appointments.

# Bug Fixes

This month’s release fixes all those bugs that were reported in the equivalent .NET version or directly with the Java API. These include:

*   Issues with text color during conversion of messages to other formats
*   Encoding issues while saving appointment files
*   Exporting appointments to message formats
*   Exceptions arose during MSG to XPS conversion, and TNEF




[1]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




