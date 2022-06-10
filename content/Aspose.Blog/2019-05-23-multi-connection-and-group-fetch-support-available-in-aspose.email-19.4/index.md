---
title: 'Multi Connection and Group Fetch Message using Aspose.Email 19.4'
date: Thu, 23 May 2019 18:44:35 +0000
draft: false
url: /2019/05/23/multi-connection-and-group-fetch-support-available-in-aspose.email-19.4/
author: Mudassir
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[![][1]](https://products.aspose.com/email/net)Hello Guys! In today's blog, I am going to give you walk through of many new exciting features and enhancements carried out in latest Aspose.Email 19.4. The best thing about Aspose team is that it publishes both .NET and Java based API having same features sets every month simultaneously. This way, the users of both API's can make use of new features irrespective of application and platform type. In following sections, I will shed some light on new features available in API and how to use them.

## Working with MultiConnection

The [ImapClient][2], SmtpClient and [Pop3Client][3] provide a [UseMultyConnection][4] property which can be used to create multiple connections for heavy operations. It allows one to set the number of connections to be used during multiconnection mode by using [ImapClient.ConnectionsQuantity][5], [SmtpClient.ConnectionsQuantity][6] and [Pop3Client.ConnectionsQuantity][7] respectively. The use of MultiConnection approach may increase the performance but it is not guaranteed. With this feature support, you can perform activities like:

*   Listing messages
    
*   Add multiple messages
    
*   Sending emails using MultiConnection
    

In the following example [Pop3Client][8] is being used to open multi connection and listing messages. The [UseMultyConnection][9] property is used to create multiple connections by setting the number of connections to be used during multiconnection mode by using [Pop3Client.ConnectionsQuantity][10].

{{< gist aspose-com-gists 522d47278b8ca448dc1d7eb97193322c "Examples-CSharp-POP3-Pop3ListMessagesWithMultiConnection-1.cs" >}}

The similar Java based example for this is:

{{< gist aspose-com-gists 709d733586ce50505c3bca3f6e8bd18d "Examples-src-main-java-com-aspose-email-examples-pop3-Pop3ListMessagesWithMultiConnection-1.java" >}}

One can add multiple messages by using the [AppendMessages][11] method provided by the [ImapClient][12] classes. The [AppendMessages][13] method accepts a list of [MailMessage][14] and adds it to the current folder if the folder is not provided as a parameter.The following example shows how to add multiple messages by using the MultiConnection mode.

{{< gist aspose-com-gists 522d47278b8ca448dc1d7eb97193322c "Examples-CSharp-IMAP-ImapGroupAppendWithMultiConnection-1.cs" >}}

The similar Java based example for this is:

{{< gist aspose-com-gists 709d733586ce50505c3bca3f6e8bd18d "Examples-src-main-java-com-aspose-email-examples-imap-ImapGroupAppendWithMultiConnection-1.java" >}}

In the following example, MultiConnection mode has set in SmtpClient for sending multiple messages.

{{< gist aspose-com-gists 522d47278b8ca448dc1d7eb97193322c "Examples-CSharp-SMTP-SendWithMultiConnection-1.cs" >}}

The similar Java based example for this is:

{{< gist aspose-com-gists 709d733586ce50505c3bca3f6e8bd18d "Examples-src-main-java-com-aspose-email-examples-smtp-SendWithMultiConnection-1.java" >}}

## Group Fetch Message

[Pop3Client][15] and [ImapClient][16] provide a [FetchMessages][17] method which accepts iterable of Sequence Numbers or Unique ID and returns a list of [MailMessage][18]. The following example demonstrates the use of the [FetchMessages][19] method to fetch messages by Sequence Numbers and Unique ID.

{{< gist aspose-com-gists 522d47278b8ca448dc1d7eb97193322c "Examples-CSharp-IMAP-ImapFetchGroupMessages-1.cs" >}}

The similar Java based example for this is:

{{< gist aspose-com-gists 709d733586ce50505c3bca3f6e8bd18d "Examples-src-main-java-com-aspose-email-examples-imap-ImapFetchGroupMessages-1.java" >}}

## Connecting to Server in Read-Only mode {#ConnectingtoIMAPServer-ConnectingtoServerinRead-Onlymode}

The [ImapClient][20] class provides a [ReadOnly][21] property which when set to **true**, indicates that no changes should be made to the permanent state of the mailbox. In the following example we have demonstrated the use of [ImapClient.ReadOnly][22] property. In example, it gets the count of unread messages, then fetches one message and then gets the count of unread messages again in read-only mode. The count of the unread messages remains the same indicating that the permanent state of the mailbox was not changed.

{{< gist aspose-com-gists 522d47278b8ca448dc1d7eb97193322c "Examples-CSharp-IMAP-ImapReadOnlyMode-1.cs" >}}

The similar Java based example for this is:

{{< gist aspose-com-gists 709d733586ce50505c3bca3f6e8bd18d "Examples-src-main-java-com-aspose-email-examples-imap-ImapReadOnlyMode-1.java" >}}

## Ability to save Contact in Version 3 VCF Format {#WorkingwithOutlookContacts-SaveContactinVersion3VCFFormat}

In this new version, you have ability to save contact in version 3 VCF format. In order to save the contact in version 3 VCF format, one need to use the [VCardVersion][23] enumerable to set the [VCardSaveOptions.Version][24] property. In the following example, the use of [VCardVersion][25] enumerable to save the contact VCF version 3 format has been demonstrated.  

{{< gist aspose-com-gists 522d47278b8ca448dc1d7eb97193322c "Examples-CSharp-Outlook-CreateV30Contact-1.cs" >}}

The similar Java based example for this is:

{{< gist aspose-com-gists 709d733586ce50505c3bca3f6e8bd18d "Examples-src-main-java-com-aspose-email-examples-outlook-msg-CreateV30Contact-1.java" >}}

## Accessing List-Unsubscribe Header Information

The List-Unsubscribe header contains the URL for unsubscribing from email lists e.g. advertisements, newsletters, etc. In order to get the List-Unsubscribe header, one need to use the [ListUnsubscribe][26] property of the [ImapMessageInfo][27] class. The following example demonstrate the use of the [ListUnsubscribe][28] property to get the List-Unsubscribe header.

{{< gist aspose-com-gists 522d47278b8ca448dc1d7eb97193322c "Examples-CSharp-IMAP-GetListUnsubscribeHeader-1.cs" >}}

The similar Java based example for this is:

{{< gist aspose-com-gists 709d733586ce50505c3bca3f6e8bd18d "Examples-src-main-java-com-aspose-email-examples-imap-GetListUnsubscribeHeader-1.java" >}}

There's many other features, enhancement, and bug fixes included in this release. [Here you can get the detail!][29]

When time allows you can check out API [examples at Github][30], talk about this release and other API related issues in our [forum][31].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2016/12/Aspose.Email-for-.NET_.png
[2]: https://apireference.aspose.com/net/email/aspose.email.clients.imap/imapclient
[3]: https://apireference.aspose.com/net/email/aspose.email.clients.pop3/pop3client
[4]: https://apireference.aspose.com/
[5]: https://apireference.aspose.com/net/email/aspose.email.clients/emailclient/properties/connectionsquantity
[6]: https://apireference.aspose.com/net/email/aspose.email.clients/emailclient/properties/connectionsquantity
[7]: https://apireference.aspose.com/net/email/aspose.email.clients/emailclient/properties/connectionsquantity
[8]: https://apireference.aspose.com/net/email/aspose.email.clients.pop3/pop3client
[9]: https://apireference.aspose.com/java/email/com.aspose.email/EmailClient#setUseMultyConnection(int)
[10]: https://apireference.aspose.com/java/email/com.aspose.email/EmailClient#setConnectionsQuantity(int)
[11]: https://apireference.aspose.com/net/email/aspose.email.clients.imap/imapclient/methods/appendmessages/index
[12]: https://apireference.aspose.com/net/email/aspose.email.clients.imap/imapclient
[13]: https://apireference.aspose.com/net/email/aspose.email.clients.imap/imapclient/methods/appendmessages/index
[14]: https://apireference.aspose.com/net/email/aspose.email/mailmessage
[15]: https://apireference.aspose.com/net/email/aspose.email.clients.pop3/pop3client
[16]: https://apireference.aspose.com/net/email/aspose.email.clients.imap/imapclient
[17]: https://apireference.aspose.com/net/email/aspose.email.clients.pop3/pop3client/methods/fetchmessages/index
[18]: https://apireference.aspose.com/net/email/aspose.email/mailmessage
[19]: https://apireference.aspose.com/net/email/aspose.email.clients.pop3/pop3client/methods/fetchmessages/index
[20]: https://apireference.aspose.com/net/email/aspose.email.clients.imap/imapclient
[21]: https://apireference.aspose.com/net/email/aspose.email.clients.imap/imapclient/properties/readonly
[22]: https://apireference.aspose.com/net/email/aspose.email.clients.imap/imapclient/properties/readonly
[23]: https://apireference.aspose.com/net/email/aspose.email.personalinfo.vcard/vcardversion
[24]: https://apireference.aspose.com/net/email/aspose.email.personalinfo.vcard/vcardsaveoptions/properties/version
[25]: https://apireference.aspose.com/net/email/aspose.email.personalinfo.vcard/vcardversion
[26]: https://apireference.aspose.com/net/email/aspose.email.clients/messageinfobase/properties/listunsubscribe
[27]: https://apireference.aspose.com/net/email/aspose.email.clients.imap/imapmessageinfo
[28]: https://apireference.aspose.com/net/email/aspose.email.clients/messageinfobase/properties/listunsubscribe
[29]: https://docs.aspose.com/display/emailnet/Aspose.Email+for+.NET+19.4+Release+Notes
[30]: https://github.com/aspose-email
[31]: https://forum.aspose.com/c/email




