---
title: 'Manage PST Password Property using C# with Aspose.Email for .NET 5.0.0'
date: Thu, 12 Feb 2015 15:55:47 +0000
draft: false
url: /2015/02/12/managing-pst-password-property-using-aspose.email-for-.net-5.0.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-net_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for .NET][1] 5.0.0. This month’s release brings improvements to the existing functionality of the API by introducing enhancements and fixing a number of bugs. For a complete list of public API changes, please visit our documentation article, Public API Changes in Aspose.Email 5.0.0. In case of any query/inquiry, please feel free to contact us over [Aspose.Email forum][2].

## Manage Password Property of a PST using C#

The PR\_PST\_PASSWORD property of a PST file represents the password protection of a PST file. Removal of this property cannot be achieved as other properties are removed from a message store. Instead, we need to set its value to zero (0) in order to get it removed. This month’s release introduces a new property for PST files, known as _Store_. It allows to access store properties of PST instead of MessageStoreProperties of PST for resetting the property. More Info

## Load Appointments with Byte Order Mark (BOM) Characters

This month’s release provides support for loading appointments having Byte Order Mark (BOM) characters at their start. BOM use is optional and appears at the start of the text stream when used. Earlier, this was a non-supported appointment type by Aspsoe.Email but this month’s release now adds the capability to load such type of appointments for further processing and manipulation. The same Appointment class’s Load method can be used to load such appointments.

## Other Improvements

This month’s release also includes a number of bug fixes that further ads to the overall functionality of the API. Specifically, these include bug fixes related to:

*   Text color issues while conversion of messages to MHTML
*   Characters encoding issue while saving appointment files
*   Issues related to exporting appointments to message format
*   Exceptions raised such as MSG to XPS conversion, creating voting options using Exchange clients, interpreting messages as TNEF and conversion of some messages to TNEF




[1]: https://products.aspose.com/email/net
[2]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




