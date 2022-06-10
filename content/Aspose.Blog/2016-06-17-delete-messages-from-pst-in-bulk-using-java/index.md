---
title: 'Delete Messages from PST in Bulk using Java'
date: Fri, 17 Jun 2016 17:10:14 +0000
draft: false
url: /2016/06/17/delete-messages-from-pst-in-bulk-using-java/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="">}}


After the release of [Aspose.Email for .NET][1], we are pleased to announce the release of [Aspose.Email for Java 6.6.0][2]. This month’s release includes the same new features, enhancements and bug fixes that were part of the .NET version of the API. You can find complete list of new and fixed issues by visiting the Release Notes of the API in our documentation section.

## Deleting messages in bulk from PST File

Ported from its equivalent .NET version, this release of Aspose.Email for Java includes the new feature of deleting multiple messages in bulk from a PST file. The deleteChildItems method provides this functionality by accepting a list of message entry ids from the PST file.

## Updating Items in bulk in a PST file

Similar to deleting items in bulk from a PST file, the API now provides the capability to update messages’ properties in bulk within a PST file. The changeMessages method accepts a list of message entry ids along with the collection of properties that need to be updated for all the messages at once.

## Deleting Set of Messages from Mailbox using IMAP Client

This month’s release also enhances the IMAP client of the API for deleting set of messages from the mailbox using a single API call. Messages can be deleted in group using the message ids as well as sequence numbers. The deleteMessagesByUids and deleteMessagesBySequenceNumbers method provide this new functionality of the IMAP client API.

## Copying Multiple Messages using IMAP Client

This month’s release also enhances the IMAP client of the API for copying multiple messages across mailbox folders using a single API call. This can be achieved using the copyMessagesByUids and copyMessagesBySequenceNumbers methods by specifying the source messages ids or sequence numbers.

## Support for IMAP4 Extensions

With this month’s release, we have also enhanced the IMAP client of the API for supporting IMAP4 Extensions and extended list command. Though these extensions are not supported by all the servers, the API provides support for these extensions and can be used where applicable.

## Other Improvements

This month’s release also fixes a number of bugs that further aid to the overall stability of the API. These also include the fix for issues reported with the .NET version of the API as the Java version is auto-ported from this .NET version.

## API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   [Product Documentation][3] – Provides detailed examples of working with the API
*   [API Reference Guide][4] – Details all the packages and classes of the API
*   [GitHub Examples][5] – Provides ready to run API examples
*   [Aspose.Email Forum][6] – Feel free to contact us on Aspose.Email forum for your queries




[1]: https://products.aspose.com/email/net
[2]: https://products.aspose.com/email/java
[3]: https://docs.aspose.com/email/java
[4]: https://apireference.aspose.com/email/java
[5]: https://github.com/aspose-email/Aspose.Email-for-Java
[6]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




