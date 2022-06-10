---
title: 'Sign Email Messages with DKIM using Java Email API'
date: Thu, 09 Apr 2015 16:09:44 +0000
draft: false
url: /2015/04/09/sign-messages-with-dkim-using-aspose.email-for-java-5.2.0/
author: Muhammad Waqas
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="">}}


[Aspose.Email for Java][1] 5.2.0 has been released. We are pleased to share that the feature of signing messages with DKIM has been implemented in this month’s release. In addition, the API also provides the capability to specify search string encoding while searching for messages using ImapQueryBuilder. For a detailed list of API changes, please consider visiting our documentation section, Public API changes in Aspose.Email for Java 5.2.0. If you have any query/inquiry related to the API, please feel free to write to us over [Aspose.Email forum][2].

## Send DKIM Signed Messages using Java

With this month’s release, the API now provides the feature of signing email messages with DKIM (Domain Keys Identified Mail). The _MailMessage_ class’s _dKIMSign_ method provides the usage of this feature by using the private key file and DKIM signature Info. Once signed, the message can be sent using the API’s SMTP client.

## Using Encoding in ImapQueryBuilder

Aspose.Email provides the capability of listing messages from IMAP server mailbox, with the capability of applying criterion based searches using _ImapQueryBuilder_. This month’s release further enhances the functionality of searching messages by specifying search string encoding. This helps querying the mailbox for different search strings based on the specified encoding e.g. Turkish characters such as ğüşıöç.

## Other Improvements

This month’s release also includes a number of bug fixes as part of either ported from its equivalent .NET version or reported actually with the Java version of the API. These include:

*   A number of issues related to TNEF messages conversion and display at receiver’s end
*   Message content encoding issues during message conversion to different formats
*   Limitation on adding more than 1020 inline images while adding message to PST
*   Exceptions while message conversion to TIFF, loading certain EML files and adding messages to PST files




[1]: https://products.aspose.com/email/java
[2]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




