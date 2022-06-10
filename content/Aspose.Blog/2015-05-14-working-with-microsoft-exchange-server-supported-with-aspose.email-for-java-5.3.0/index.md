---
title: 'Working with Microsoft Exchange Server using Aspose.Email for Java 5.3.0'
date: Thu, 14 May 2015 06:50:28 +0000
draft: false
url: /2015/05/14/working-with-microsoft-exchange-server-supported-with-aspose.email-for-java-5.3.0/
author: Muhammad Waqas
summary: ''
tags: ['Connect to Exchange Servers in Java', 'Java Email API for Microsoft Exchange Server']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="">}}


We are excited to share the release of [Aspose.Email for Java 5.3.0][1] that provides the capability of working with Microsoft Exchange Server. This month’s release also brings other enhancements and improvements by fixing a number of bugs. For a complete list of API changes, please visit our documentation section, [Public API Changes][2] in Aspose.Email 5.3.0. You can contact us directly on [Aspose.Email][3] forum in case you have any queries or inquiries related to the API.

## Working with Exchange Server in Java

Yes, you have heard it right! Aspose.Email for Java API now supports working with Exchange servers. This support is based on WebDav and Exchange Web Service (EWS) protocols that enable users to connect to Microsoft Exchange servers 2007, 2010 and 2013. In addition, it can be used to connect to Office 365 online servers via the EWS protocol. The API supports:

*   Connecting to Exchange Server using WebDav and EWS protocols
*   Listing messages from Mailbox
*   Fetching and saving messages to disc
*   Filtering messages from mailbox
*   Access and download messages from Public folders on Exchange server
*   Delete messages from mailbox
*   Getting MailTips from Server
*   Getting Mailbox information from server
*   Connecting to Exchange Server using IMAP
*   Working with Conversation Items
*   Managing Rules on Exchange Server
*   Managing User configuration on Exchange Server
*   Reading emails from other user’s mailbox
*   Move messages between mailbox folders
*   Create and Send message using the API’s Exchange clients
*   Send meeting requests using Exchange Server
*   Synchronizing folder items
*   Retrieving contacts information from Exchange Server

For working code samples, please visit our documentation section [Working with Exchange][4].

# Other Enhancements

This month’s release also provides a number of enhancements as detailed below:

**Detecting Messages for Encryption:** The _MailMessage_ class now provides the method of detecting if a message is encrypted or not. The _IsEncrypted_ method can be used to check a message for encryption.

**Support for adding PT\_MV\_LONG Multivalue Property:** This month’s release provides the capability of adding a new multivalue property, PT\_MV\_LONG.  The property can be added to the _NamedPropertyMapping_ or as a Custom property to the message store, as shown in our [Setting Outlook Mapi Properties][5] article.

# Code Baseline Moved to Java 6

JDK 1.4 and 1.5 have been discontinued by Sun/Oracle. Even the commercial (non-open) support of JDK 1.5 is no more available. As a result, we also had to discontinue the support for these older versions of JDK. Starting from January release of Aspose.Email for Java 5.0.0, we no more support Java 1.4 and 1.5, and we have already moved our code base to Java 6. Since the last available Java JDK is 1.8 64-bit, we can compile 1.8 baseline to 1.6 production JAR for release publication.

# Other Improvements

There are a number of other improvements that are part of this release as a result of bug fixes. These are related to:

*   Incorrect time zone display when retrieving message’s date information
*   Loss of Contact Notes while downloading contact information from Exchange server
*   Formatting issues during message conversions between various formats
*   Exceptions such as working with Mono Framework using the API, loading certain messages and appointments files, and adding/deleting messages to a PST




[1]: https://downloads.aspose.com/email/java
[2]: http://docs.aspose.com/display/emailjava/Public+API+Changes+in+Aspose.Email+5.3.0
[3]: http://forum.aspose.com
[4]: http://docs.aspose.com/display/emailjava/Working+with+Exchange
[5]: https://docs.aspose.com/display/emailjava/Working+with+MAPI+Properties




