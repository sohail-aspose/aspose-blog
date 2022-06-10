---
title: 'PST Messages Bulk Deletion and Update supported with Aspose.Email for .NET 6.6.0'
date: Sat, 11 Jun 2016 06:31:22 +0000
draft: false
url: /2016/06/11/pst-messages-bulk-deletion-and-update-supported-with-aspose.email-for-.net-6.6.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[![Aspose.Email for .NET][1]](https://products.aspose.com/email)

We are pleased to announce the release of [Aspose.Email for .NET 6.6.0][2]. This month’s release includes a number of new features, enhancements and bug fixes that further enrich the API functionality and brings more stability to the product. Specifically, bulk operations have been supported for deletion of items from PST and mailbox servers using the API’s IMAP client. For a complete list of what is new and fixed, please visit the Product Release Notes page of Aspose.Email for .NET 6.6.0.

# New Features & Enhancements

**Bulk Deletion of Messages from PST:** This month’s release introduces a new feature of deleting messages in bulk from a PST file for optimized I/O operations. This functionality was the dire need of our customers who were facing performance issues while deleting messages from PST one by one. The _DeleteChildItems_ method introduced in this month’s release provides the interface to accept a list of entry id strings for messages to be deleted from the PST file.

**Updating Message Properties in Bulk within a PST:** This month’s release also provides the capability to update message properties within a PST file without retrieving them first. Similar to the bulk deletion of messages from a PST file, properties of multiple messages can be updated in bulk using the _ChangeMessages_ method. This accepts message properties collection to update messages using the specified entry ids list.

**Copying Multiple Messages Across Mailbox Folders using IMAP:** It may often be required to copy multiple messages from one folder of mailbox to another folder. This month’s release further enhances the copying messages feature of the API’s ImapClient to copy multiple messages using a single command to the server. Multiple messages can be copied using the _CopyMessages_ that has different variants of implementation as follow:

*   Copies a list of messages using the messages’ unique ids
*   Copies a list of messages using the messages’ sequence numbers
*   Ability to copy multiple messages using the collection specified by _ImapMessageInfoCollection_

**Deleting Multiple Messages using IMAP:** This month’s release also enhances the deletion functionality of the API’s IMAP client by providing the capability of deleting multiple messages using a single API call. The _DeleteMessages_ method introduced in this month’s release accepts a list of messages’ unique ids or sequence numbers that can be used to delete these messages via a single API call.

**Support for IMAP Extensions:** This month’s release also provides additional IMAP and IMAP4 extensions to the set of functionality supported by the API’s IMAP client. This includes the support for IMAP4 ID Extension and IMAP4 Extended List command.

**Support for Connecting to Server using IP address:** Certain mail servers may not have reverse DNS available that may give error while connecting to the server using its IP address. This month’s release enhances the API’s POP3 and IMAP clients so that they can connect to the mail server using its IP address.

# Other Improvements

This month’s release also fixes a number of bugs that were reported with our last release by our customers. Fixing these brings further stability and value to the API functionality.

# API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   Product Documentation – Provides detailed examples of working with the API
*   API Reference Guide – Details all the namespaces and classes of the API
*   [GitHub Examples][3] – Provides ready to run API example
*   [Support Forum][4] – Write to us if you have any query or inquiry about the API




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2016/06/Aspose.Email-for-.NET_.png "Aspose.Email for .NET"
[2]: http://www.aspose.com/downloads/email/net
[3]: https://github.com/asposeemail/Aspose_Email_NET
[4]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




