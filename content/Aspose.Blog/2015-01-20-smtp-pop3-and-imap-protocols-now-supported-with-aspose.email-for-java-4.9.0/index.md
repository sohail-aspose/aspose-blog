---
title: 'Use SMTP, POP3 and IMAP Protocols with Aspose.Email for Java 4.9.0'
date: Tue, 20 Jan 2015 14:44:30 +0000
draft: false
url: /2015/01/20/smtp-pop3-and-imap-protocols-now-supported-with-aspose.email-for-java-4.9.0/
author: Kashif Iqbal
summary: ''
tags: ['Java Mail API for MIME SMTP POP3 IMAP', 'Java mail library', 'Work with Outlook messages in Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="">}}


We are really excited to share that Aspose.Email for Java now supports communication protocols. What this means is that you can now send and receive emails using the most common email protocols such as SMTP, POP3, and IMAP. This month’s release also brings other enhancements to the API functions such as sending tasks requests and removing MAPI Properties from messages and message attachments. For complete details about what is new and fixed, please visit the [product download page][1].

# New Features

**Sending Email Messages with SMTP:** With this month’s release, Aspose.Email for Java now supports sending email messages using the Simple Mail Transfer Protocol (SMTP). You can use the API for sending emails right from within your applications using the SMTP settings from popular email services such as Gmail, Yahoo, Hotmail or any other server. The SMTP client provides the following features:

*   [Sending email messages][2]
*   [Sending meeting requests][3]
*   [Sending Tasks Requests][4]
*   [Sending emails via proxy servers][5]
*   [Listing Server Extensions][6]

**Managing Email Messages with POP3:** Aspose.Email for Java now supports Post Office Protcol (POP) v 3.0 for connecting and retrieving email messages from mail servers. The Pop3Client class provides the entire necessary interface for instantiating communication with mail servers for manipulating messages. The POP3 Client provides the following features for retrieving messages:

*   [Connecting to Non-SSL and SSL-Enab][7][l][8][ed POP3 Servers][9]
*   [Getting Mailbox Information][10]
*   [Listing Server Extensions][11]
*   [Retrieving Email Headers][12]
*   [Retrieving Email Messages][13]

**Managing Email Messages with IMAP:** Internet Message Access Protocol (IMAP) allows clients to connect and manage email messages on the mail server. Aspsoe.Email for Java API now supports the IMAP communication protocol for connecting to mail servers and retrieving email messages. The IMAP client provides the following functionality for retrieving messages:

*   [Connecting to Non-SSL and SSL-Enabled IMAP Servers][14]
*   [Getting Folders Information from the Server][15]
*   [Adding a new message to a folder][16]
*   [Changing Message flags][17]
*   [Retrieve list of messages from IMAP server][18]
*   [Fetching messages using Sequence number][19]
*   [Fetching messages using Unique Message Id][20]
*   [Retrieving “N” number of messages][21]
*   [Deleting messages from the server][22]

# Bug Fixes

This month’s release includes a number of bug fixes that further improves the overall API functionality. These include:

*   Encoding issues while converting the message to other formats
*   Loss of body contents and detection of attachments as inline items
*   Issues related to the [removal of MAPI properties][23] from MSG as well as attachments
*   Exceptions while loading messages, listing messages and interpreting messages as TNEF

If you have any queries or inquiries related to the existing/new features of the API, please feel free to contact us over the Aspose.Email [forum][24]. We’ll be glad to assist you further.




[1]: https://downloads.aspose.com/email/java
[2]: https://docs.aspose.com/display/emailjava/Sending+and+Forwarding+Messages
[3]: https://docs.aspose.com/display/emailjava/Sending+and+Forwarding+Messages#SendingandForwardingMessages-SendingMeetingRequest
[4]: https://docs.aspose.com/
[5]: https://docs.aspose.com/display/emailjava/Connecting+to+SMTP+Server#ConnectingtoSMTPServer-ConnectingtoSMTPServerviaHTTPProxyServer
[6]: https://docs.aspose.com/display/emailjava/Utility+Features+-+SMTP+Client#UtilityFeatures-SMTPClient-ListingExtensionServersusingSmtpClient
[7]: http://docs.aspose.com/display/EmailJava/Connecting+to+POP3+Server
[8]: https://docs.aspose.com/
[9]: http://docs.aspose.com/display/EmailJava/Connecting+to+POP3+Server
[10]: https://docs.aspose.com/display/emailjava/Working+with+Messages+from+Server#WorkingwithMessagesfromServer-GettingMailboxInformation
[11]: https://docs.aspose.com/display/emailjava/Listing+Server+Extensions+using+POP3Client
[12]: https://docs.aspose.com/display/emailjava/Working+with+Messages+from+Server#WorkingwithMessagesfromServer-RetrievingEmailHeaders
[13]: https://docs.aspose.com/display/emailjava/Working+with+Messages+from+Server#WorkingwithMessagesfromServer-RetrievingEmailMessagesandSaving
[14]: https://docs.aspose.com/display/emailjava/Connecting+to+IMAP+Server
[15]: https://docs.aspose.com/display/emailjava/Working+with+Folders+on+IMAP+Server
[16]: https://docs.aspose.com/display/emailjava/Working+with+Folders+on+IMAP+Server#WorkingwithFoldersonIMAPServer-AddingaNewMessageinaFolder
[17]: https://docs.aspose.com/display/emailjava/Changing+Message+Flags
[18]: https://docs.aspose.com/display/emailjava/Fetching+Messages+and+Saving+to+Disc
[19]: https://docs.aspose.com/display/emailjava/Fetching+Messages+and+Saving+to+Disc#FetchingMessagesandSavingtoDisc-FetchMessagesBySequenceNumberandSavetoDisc
[20]: https://docs.aspose.com/display/emailjava/Fetching+Messages+and+Saving+to+Disc#FetchingMessagesandSavingtoDisc-FetchMessagesByMessageIdandSavetoDisc
[21]: https://docs.aspose.com/display/emailjava/Fetching+Messages+and+Saving+to+Disc#FetchingMessagesandSavingtoDisc-Retrieve%22N%22numberofMessagesfromServer
[22]: https://docs.aspose.com/display/emailjava/Delete+Messages
[23]: https://docs.aspose.com/display/emailjava/Working+with+MAPI+Properties
[24]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




