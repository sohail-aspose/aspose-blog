---
title: 'Move Items Between PST Folders using C# with Aspose.Email for .NET'
date: Mon, 03 Mar 2014 05:33:45 +0000
draft: false
url: /2014/03/03/aspose.email-for-.net-3.9.0-supports-moving-items-between-pst-folders-and-loading-tasks-from-ics-files/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[Aspose.Email for .NET][1] 3.9.0 has been released with new features, enhancements and bug fixes.

## Move Items Between PST Folders using C#

Moving items from one PST folder to another wasn’t supported until now and items need to be moved to other folders one by one. With this month’s release, Aspose.Email supports moving items to other folders in the same PST. This includes moving messages as well as folders along with their contents to other folders.

This month’s release also provides support for loading Google Task from iCalendar format. The API’s MapiTask class exposes a static method, FromVTodo, for loading a task from an ICS file and save it as Outlook Message format or add to a Personal Storage (PST) file.

This month’s release also includes a number of improvements to the SMTP, POP and IMAP clients as listed below:

*   Aspose.Email’s SMTP, [POP3][2] and [IMAP][3] clients now support listing server extensions such as IDLE, UNSELECT, QUOTE, etc. This helps identifying an extension's availability before using the client for that particular functionality
*   The asynchronous methods in SMTP, IMAP and POP3 clients earlier used a single network connection to communicate with the server. This month’s release supports multiple connections for these mail clients for asynchronous operations.
*   Aspose.Email’s IMAP client now supports fetching and deleting messages using a message’s unique ID.
*   This version of Aspose.Email’s API also provides the support for keeping the IMAP as well as POP3 connections open indefinitely.
*   The asynchronous methods for IMAP client of Aspose.Email has been enhanced to allow listing messages from server specifying filtering criteria with the MailQuery parameter

This month’s release also includes a number of bug fixes that further improves the overall functionality of the API. These include fixes to issues like message conversion, inline attachments visibility, moving items using an Exchange client, conversions to MHTML and some exceptions. For more details on what is new and fixed, please refer to the [product download page][4].




[1]: https://products.aspose.com/email/net
[2]: http://docs.aspose.com/display/emailnet/Listing+Server+Extensions+using+Pop3Client
[3]: http://docs.aspose.com/display/emailnet/Listing+Server+Extensions+using+Pop3Client
[4]: https://downloads.aspose.com/email/net




