---
title: 'Performing Mail Merge and Setting Password on PST supported with Aspose.Email for Java 5.6.0'
date: Mon, 17 Aug 2015 16:05:40 +0000
draft: false
url: /2015/08/17/performing-mail-merge-and-setting-password-on-pst-supported-with-aspose.email-for-java-5.6.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

![](https://blog.aspose.com/wp-content/uploads/sites/2/2015/08/aspose-Email-for-Java_100.png "aspose-Email-for-Java_100")

[Aspose.Email for Java 5.6.0][1] has been released. This month’s release includes a new feature of performing Mail Merge similar to the .NET equivalent version of the API. In addition, it contains a number of enhancements related to various API functional areas. For a complete list of API changes, please visit our documentation section, Public API Changes in Aspose.Email for Java 5.6.0.

# New Features & Enhancements

**Performing Mail Merge:** Aspose.Email for .NET already provided support for performing Mail Merge using the TemplateEngine class. This feature helps create and send a batch of similar email messages. The core of the emails is the same but the content can be personalized. This month’s release of Aspose.Email for Java API provides the same functionality of performing Mail Merge for creating and sending emails of the same nature.

**Rendering Calendar Events:** With this month release, Aspose.Email for Java provides the capability to render calendar events while converting messages to MHTML. This can be achieved using the _MhtFormatOptions.RenderCalendarEvent_ enumerator. More Info

**Password Protecting a PST:** This month’s release also includes an enhancement of setting or changing a PST password. This is achieved by setting the password using the _changePassword_ method of PST store. The same method can be used to remove the password of the PST as well. More Info

**Retrieving Attachment Description:** Information about the contents of an attachment can now be retrieved using the attachment header. This information is contained and can be retrieved from the “Content-Description” header of an attachment.

**Getting Recipient Status from MapiCalendar:** Calendar events contain information about the recipient’s status for attending the meeting. This information can now be retrieved using the Aspose.Email API from the response message. The _MapiRecipient_ class’s _getRecipientTrackStatus_ method returns the status of the recipient. More Info

# Other Improvements

In addition the new features and enhancements, the API contain a number of other improvements as a result of bug fixes. Since the API is auto-ported from its equivalent .NET version, all the bug fixes contained in .NET version are also part of this month’s release. For a complete list of all the bug fixes, please visit the [product download page][2].

# API Resources and Forum Support

You may visit our documentation section of the API for further details about all the  functional capabilities. In addition, you may also visit Aspose.Email for Java [GitHub repository][3] for downloading the ready-to-use examples. In case you have any query, please feel free to write to us over [Aspose.Email forum][4].




[1]: http://www.aspose.com/community/files/72/java-components/aspose.email-for-java/entry648821.aspx
[2]: http://www.aspose.com/community/files/72/java-components/aspose.email-for-java/entry648821.aspx
[3]: https://github.com/aspose-email/Aspose.Email-for-Java
[4]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




