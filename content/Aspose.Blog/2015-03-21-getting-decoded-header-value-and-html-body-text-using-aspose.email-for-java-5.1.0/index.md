---
title: 'Decode Email Header Value and Extract Message Information from HTML Body in Java'
date: Sat, 21 Mar 2015 15:29:59 +0000
draft: false
url: /2015/03/21/getting-decoded-header-value-and-html-body-text-using-aspose.email-for-java-5.1.0/
author: Kashif Iqbal
summary: ''
tags: ['Decode email header value in Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="">}}


We are pleased to announce the release of Aspose.Email for Java 5.1.0 that includes a number of enhancements and improvements to the API. For a complete list of enhancements and improvements, please visit the product download page. A complete list of API changes in this recent version can be found in our documentation article, [Public API Changes][1] in Aspose.Email for Java.

# Enhancements

This month’s release includes the following enhancements:

**Getting Decoded Header Value:** Message headers include encoding characters along with normal message text. This month’s release provides the capability of getting decoded header values using the _getDecodedValue_ method of _HeaderCollection_. [More Info][2]

**Preserving Original Email Address:** This month’s release also includes the enhancement of preserving original email addresses that may contain malformed/invalid characters. Such characters can be part of the mail address in cases, for example, where the email is received internally within the organization from the Exchange server. The _[setPreserverOriginalAddresses][3]_ can be used to ignore the validity check while converting _MailMessage_ to _MapiMessage_.

**Getting Textual Message Information from Message’s HTML Body:** This month’s release also includes an enhancement where message’s HTML body equivalent text can be retrieved if the HTML information is malformed due to some reason. This can be achieved using the _[getHtmlBodyText][4]_ method of _MailMessage_ class.

# Other Improvements

Ported from its equivalent .NET version, this month’s release also includes a number of bug fixes which further improves the API functionality. These include:

*   Issues related to PST such as sender name not shown in PST, corrupt task and meeting body while adding tasks to PST, and exceptions while extracting messages from a PST
*   Encoding issues while converting messages from one format to another
*   Exception while loading appointment from ICS, loading EML files and EML to MHT conversions

As always, we encourage you to contact us for any query/inquiry related to the API. We’ll be glad to address your issues and assist you further over [Aspose.Email forum][5].




[1]: http://docs.aspose.com/display/emailjava/Public+API+Changes+in+Aspose.Email+5.1.0
[2]: http://docs.aspose.com/display/emailjava/Customizing+Email+Headers
[3]: https://docs.aspose.com/display/emailjava/Creating+and+Saving+MSG+files#CreatingandSavingMSGfiles-PreservingOriginalEmailAddress
[4]: https://docs.aspose.com/display/emailjava/Extracting+Message+Contents+from+Emails
[5]: http://forum.aspose.com




