---
title: 'Saving Distribution Lists in MSG Format and Accessing Search Folders in OST supported with Aspose.Email for .NET 5.5.0'
date: Thu, 09 Jul 2015 19:12:26 +0000
draft: false
url: /2015/07/09/saving-distribution-lists-in-msg-format-and-accessing-search-folders-in-ost-supported-with-aspose.email-for-.net-5.5.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[![][1]](https://products.aspose.com/email)We are pleased to announce the release of [Aspose.Email for .NET 5.5.0][2]. This month’s release includes enhancements to the existing functionality of the API such as saving email distribution lists and traverse search folders from PST files. Our documentation section, Public API Changes in Aspose.Email 5.5.0, lists all the changes that are part of this month’s release. If you have any query or inquiry related to the API, please feel free to contact us over [Aspose.Email forum][3].

# Enhancements

Following are the enhancements included in this month’s release.

**Provision of Saving Email Distribution Lists:** Aspose.Email had the capability to create distribution lists, similar to Microsoft Outlook, and add contacts to these. This distribution list could then be added to a PST. This month’s release further enhances this feature by providing support for saving email distribution lists to disc. A distribution list is saved to disc in standard Outlook MSG format and can be opened in MS Outlook.

**Capability to Parse Searchable Folders in a PST:** A PST or OST file may contain search as well as normal type of folders. Traversing through folders of such a PST file ignored the search folders until now when the API provides the capability to include items from search folders as well while retrieving contents. The FolderKind.Search|FolderKind.Normal enumerator is used to specify the kind of folders for consideration.

# Other Improvements

This month’s release also fixes a number of bugs that were reported with our earlier version. These further improve the overall functionality and performance of the API. These include, but not limited to:

*   Encoding issues while converting messages to other formats
*   Issue while reading EML attachments
*   Missing contents from Aspose created MSG files in Outlook
*   Missing contents of Search folders from OST/PST
*   Exceptions such as loading TNEF files, listing messages using IMAP client, splitting OST files and loading NDR messages




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2015/07/aspose-Email-for-net_1001.png "aspose-Email-for-net_100"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.email-for-.net/entry640252.aspx
[3]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




