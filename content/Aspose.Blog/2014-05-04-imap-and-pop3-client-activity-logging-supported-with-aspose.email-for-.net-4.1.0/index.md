---
title: 'IMAP and POP3 Client Activity Logging using C# or VB.NET'
date: Sun, 04 May 2014 19:51:33 +0000
draft: false
url: /2014/05/04/imap-and-pop3-client-activity-logging-supported-with-aspose.email-for-.net-4.1.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-net_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for .NET][1] 4.1.0. As always, this month’s release includes a number of bug fixes for issues reported by our customers in last month’s version. In addition, it also introduces new features and enhancements to the existing API as detailed below.

## Activity Logging for IMAP and POP3 Clients

Server-client communication is based on a command-response mechanism and can be monitored in order to observe the communication behavior of the underlying connection. Aspose.Email API already provides the capability of [SMTP activity logging][2], however, the same was missing for IMAP and POP3 clients. As part of our continuous efforts for improvements, we are pleased to share that this month’s release now supports activity logging for [IMAP][3] and [POP3][4] clients.

## Replying or Forwarding Messages using Exchange Web Service Client

Aspose.Email’s Exchange Web Service (EWS) client already provides support for [sending email messages][5]. Though this is usually enough for communication needs, it is often required to reply or forward a certain email message, a very common practice. We are pleased to share that Aspose.Email’s EWS client now supports [replying or forwarding][6] messages.

## Filter and Display Messages based on Internal Date

Aspose.Email's IMAP client already provides the capability to retrieve messages from mailbox based on some search criteria. This is achieved using the ImapQueryBuilder with search criteria specified on the Date of the messages. Though this works in most cases, it may not list all the messages that fulfill the search criteria for the reason that the server timezone is different (for example like GMAIL which is not UTC). This month's release enhances the ImapQueryBuilder by introducing a new member as InternalDate which further helps in [filtering the messages][7] based on the server internal's date.

For further information on changes to the public API, fixed bugs and enhancements, please visit the [product download page][8]. As always, we appreciate your feedback and you can reach us any time for assistance via the [Aspose.Email forum][9].




[1]: https://products.aspose.com/email/net
[2]: https://docs.aspose.com/email/net/utility-features-smtp-client/#smtp-client-activity-logging
[3]: https://docs.aspose.com/email/net/imapclient-activity-logging/
[4]: https://docs.aspose.com/email/net/pop3client-activity-logging/
[5]: https://docs.aspose.com/email/net/working-with-exchange-mailbox-and-messages/#sending-email-messages
[6]: https://docs.aspose.com/email/net/developer-guide/
[7]: https://docs.aspose.com/email/net/filter-messages-from-server-using-imap-client/
[8]: http://downloads.aspose.com/email/net
[9]: http://forum.aspose.com




