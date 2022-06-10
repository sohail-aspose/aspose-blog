---
title: 'Split PST Files with Specific Criterion using Java'
date: Wed, 17 Aug 2016 18:22:24 +0000
draft: false
url: /2016/08/17/split-pst-files-with-specific-criterion-using-aspose.email-for-java-6.8.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="">}}


[Aspose.Email for Java 6.8.0][1] has been released. Ported from its equivalent .NET version, this month’s release includes the same new features, enhancements, and bug fixes. Specifically, it allows splitting a PST based on defined criterion using the _PersonalStorageQueryBuilder, the option to detect if a loaded message is TNEF, and getting the_ message’s summary information using its unique id with Pop3Client of the API. For detailed information about what is new and fixed, please visit the release notes section of our documentation.

## Split PST File Based on Defined Criterion

This month’s release introduces a new feature of [splitting a PST][2] file into multiple PST files by specifying a combination of criteria. The _PersonalStorageQueryBuilder_ class can be used to define criteria that meet user requirements. The new method, _splitInto_, introduced by the _PersonalStorage_ class, provides the capability to split the PST file using these input criteria.

## Detect a Message for TNEF

This month’s release also provides the capability to detect if the message loaded using _MailMessage_ was originally [TNEF][3] or not. The _getOriginalIsTnef_ method exposed by _MailMessage_ class can be used to identify the format of the message for this.

## Retrieve Message Summary Information using Unique Id

This month’s release also introduces a new feature where the API’s POP3 client provides the capability to retrieve [message summary information][4] using its Unique Id. The _getMessageInfo_ method lets you obtain the _Pop3MessageInfo_ object for a message by specifying its unique Id.

## Other Improvements

This month’s release also fixes a number of bugs that were reported with the earlier version of the API. This further aids to the overall improvement and stability of the API functionality.

## API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   [Product Documentation][5] – Provides detailed examples of working with the API
*   [API Reference Guide][6] – Details all the packages and classes of the API
*   [GitHub Examples][7] – Provides ready to run API examples
*   [Aspose.Email Forum][8] – Feel free to contact us on Aspose.Email forum for your queries




[1]: https://downloads.aspose.com/email/java
[2]: https://docs.aspose.com/email/java/splitting-and-merging-pst-files/#SplittingandMergingPSTFiles-SplitPstOnCriterion
[3]: https://docs.aspose.com/email/java/utility-features-mailmessage/#detect-if-a-message-is-tnef
[4]: https://docs.aspose.com/email/java/working-with-messages-from-server/#WorkingwithMessagesfromServer-GettingMessageSummaryInformation
[5]: https://docs.aspose.com/email/java/
[6]: http://www.aspose.com/api/java/email
[7]: https://github.com/aspose-email/Aspose.Email-for-Java
[8]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




