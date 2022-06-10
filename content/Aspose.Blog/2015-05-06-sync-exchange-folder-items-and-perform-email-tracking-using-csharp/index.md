---
title: 'Sync Exchange Folder Items and Perform Email Tracking using C#'
date: Wed, 06 May 2015 07:31:20 +0000
draft: false
url: /2015/05/06/sync-exchange-folder-items-and-perform-email-tracking-using-csharp/
author: Muhammad Waqas
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-net_100.png" alt="">}}


[Aspose.Email for .NET 5.3.0][1] has been released. This month’s release includes new features, enhancements and bug fixes that contribute more towards the value of the product. These features are related to various functional areas of the API including Outlook properties of a message, Exchange client, and Microsoft Outlook tasks and messages encryption. We have published the complete details of API changes in our documentation article Public API Changes in Aspose.Email for .NET 5.3.0 for reference.

## Syncing Exchange Server Folder Items

With this month’s release of Aspose.Email for .NET, you can now sync Exchange server items for changes incurred to an Exchange folder. This is done by calling the _SyncFolder_ method of the API’s _IEWSClient_ and specifying the respective folder. This helps detect the changes such as new message arrival, changed message items, deleted items and changes in message read status. For a sample code, you may refer to our documentation article, Syncing Folder Items on Exchange Server.

## **Support for Email Tracking**

This month’s release also includes a new feature of email tracking using Message Disposition Notification (MDN) support. This is achieved by requesting the read receipts and creating the required information. The _MailMessage_ class’s _ReadReceiptTo_ property gets or sets the set read receipt address. The _CreateReadReceipt_ and _ReadReceiptRequested_ methods are used for creating and retrieving the information whether read receipts are requested. We have illustrated the usage of this feature with the help of sample code that can be consulted for getting an idea.

## Enhancements

**Detecting Message for Encryption:** This month’s release of Aspose.Email has further enhanced the MailMessage class with inclusion of _IsEncrypted_ property. The property can be used to check a received/load message file for encryption. This is different to the already available _IsSigned_ property that shows if message is signed. Our online documentation article, Message Encryption and Decryption, demonstrates the usage of this property with the help of sample code.

**Support for additional MultiValue Property:** Aspose.Email API already supports adding multi value Mapi properties to a message’s store. We have added the support for MV\_LONG property in this month’s release which allows adding this property using both NamedProperty and Custom property message store. Please refer to our documentation article, Setting Mapi Properties for working sample code.

**Setting Notes format for Contact:** This month’s release has further enhanced setting the format of Outlook Contact notes. The _Aspose.Email.Mail.Contact.NotesFormat_ property can be used to get the notes format. The possible values of this are represented by the _Aspose.Email.TextFormat_ enumerator that can also be used to select a specific format for setting purpose.

## Bug Fixes

We have also fixed a number of bugs related to various areas of API functionality. These include issues related to:

*   Encoding issues during message conversion to other formats
*   Missing information during messages conversion to MHTML
*   Wrong message body type detection by MailMessage
*   Loss of linked resource images when sending email using the API
*   Exceptions such as using the IEWSClient of API with Mono framework, conversion to messages to MailMessage, loading certain email message files, and malformed address compilation

If you have any query related to the API, you can share your feedback with us on [Aspose.Email forum][2] for further assistance.




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.email-for-.net/entry625864.aspx
[2]: http://forum.aspose.com




