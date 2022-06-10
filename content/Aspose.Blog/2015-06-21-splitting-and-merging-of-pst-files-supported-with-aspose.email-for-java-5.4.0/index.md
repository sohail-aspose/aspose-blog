---
title: 'Split and Merge PST Files using Java Email API'
date: Sun, 21 Jun 2015 16:31:36 +0000
draft: false
url: /2015/06/21/splitting-and-merging-of-pst-files-supported-with-aspose.email-for-java-5.4.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for Java 5.4.0][1]. This month’s release, followed by its equivalent .NET version, introduces new features of splitting/merging PST files and processing delivery failure messages. It also enhances the functionality of working with Exchange tasks by saving them to disc. The release also brings improvement in the API functionality by fixing a number of bugs that were reported with our earlier version. For a complete list of API changes in this month’s release, please visit our documentation section article, Public API changes in Aspose.Email for Java 5.4.0. In case of any query related to Aspsoe.Email API, please feel free to contact us over [Aspose.Email forum][2].

## Splitting & Merging PST files using Java

Aspsoe.Email for Java API now provides the capability of splitting large PST files and merging small PST files. Thus, a large PST file can now be split into multiple small PST files by specifying the desired PST files size and location to store. Similarly, the API provides the capability to merge multiple small PST files to result in a single large PST file. It can also merge specific folders from a source PST to a destination PST file. Our documentation article, Splitting & Merging PST file, provides further details about this new feature with illustrative examples.

## Processing Bounced Messages

This month’s release also introduces the feature of processing bounced (Delivery Failure Notifications) messages. Such messages can now be processed to get details about the type of message notification (delayed, failed to deliver, etc.), recipient, reason and status. More Info

## Saving Exchange Task to Disc

Aspose.Email API introduced working with Exchange server with our last month’s release. This month’s release further enhances the Exchange task functionality by saving Exchange task to disc in Outlook MSG format that can be opened in MS Outlook then. More Info

## Other Improvements

This month’s release also includes improvements by fixing a number of bugs and exceptions that were reported by our valued customers with our earlier version of the API. These include:

*   Encoding issues while converting messages to other formats
*   Issues with communication clients such as exceptions while fetching Signing messages and resolving contacts information
*   Issues working with MapiTasks for creating recurrences
*   Exceptions loading Outlook messages and Exchange transmitted TNEF messages

## Goodbye to Examples Dashboard

From this release onwards, we have removed all Examples Dashboard stuff from our release version. All the examples are published on the social coding website GitHub.com where these are readily available for [download and execution][3]. For more details, please check out our blog post: Welcome to Social Coding and Goodbye to Examples Dashboard




[1]: https://products.aspose.com/email/java
[2]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx
[3]: https://github.com/aspose-email/Aspose.Email-for-Java




