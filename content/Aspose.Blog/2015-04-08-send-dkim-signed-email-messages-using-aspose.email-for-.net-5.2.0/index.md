---
title: 'Send DKIM Signed Email Messages using C# with Aspose.Email for .NET 5.2.0'
date: Wed, 08 Apr 2015 06:02:36 +0000
draft: false
url: /2015/04/08/send-dkim-signed-email-messages-using-aspose.email-for-.net-5.2.0/
author: Muhammad Waqas
summary: ''
tags: ['Sign email messages with DKIM in CSharp', 'send DKIM signed emails using Csharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-net_100.png" alt="">}}


We are pleased to announce the release of Aspose.Email for .NET 5.2.0 that includes new features, enhancements, and a number of functionality improvements. With this month’s release, you can now send DKIM signed emails. We have also provided the facility to fetch message size from the Exchange server before the whole message is fetched. For a complete list of improvements, please visit our [product download page][1]. Our documentation article, [Public API changes][2] in Aspose.Email for .NET 5.2.0, contains a list of all the changes that are part of this release.

## Send DKIM Signed Emails in C#

This month’s release provides the feature of signing email messages with DKIM (Domain Keys Identified Mail) that enables organizations to take responsibility for the message that is in transit. A digital signature is added to the email message headers using the user-defined private keys. The API’s _MailMessage_ class provides the method _DKIMSign_ that uses the Crypto Service Provider and DKIM Signature Info for signing the message. Once signed, the message can be sent using the API’s SMTP as well as Exchange Clients. The following code sample shows how to create and send DKIM signed emails using C#.

{{< gist aspose-com-gists 6e5185a63aec6fd70d83098e82b06a32 "Examples-CSharp-Email-SignEmailsWithDKIM-SignEmailsWithDKIM.cs" >}}

For further details, please visit [sing emails with DKIM][3].

## Pre-Fetch Message Size

Outlook InterOp provides the feature of retrieving message size before actually fetching the complete message from the Exchange server. In the case of Aspose.Email API, the summary information retrieved from the Exchange server is represented by _ExchangeMessageInfo_ class and represents the only information that is fetched before actually retrieving the whole message. This month’s release enhances the functionality provided by this class to [fetch message size][4] as well before the complete message is fetched from the server. This information is represented by the _Size_ property of the class.

## Using Encoding in ImapQueryBuilder

We have also enhanced the ImapQueryBuilder for specifying [search string encoding][5] while listing messages from the IMAP server. This helps to query the strings that are, for example, in Unicode format and were not supported earlier. An example is Turkish characters such as ğüşıöç.

## Other Improvements

This month’s release also fixes a number of bugs that were discovered by our valued customers while working with our API. We have fixed them all, resulting in improved API functionality. Some of these include:

*   Issues related to TNEF messages sending via SMTP and Exchange clients
*   Encoding issues while converting messages to other formats
*   Issues related to PST during exporting messages
*   Exceptions while listing messages from IMAP client, loading certain message files, converting messages to TIFF and Exchange Server

As always, we welcome your feedback about the new release. Please feel free to contact us for your queries on [Aspose.Email forum][6].




[1]: http://downloads.aspose.com/email/net
[2]: http://docs.aspose.com/display/emailnet/Public+API+Changes+in+Aspose.Email+5.2.0
[3]: https://docs.aspose.com/display/emailnet/Creating+and+setting+contents+of+Emails#CreatingandsettingcontentsofEmails-SignEmailswithDKIM
[4]: https://docs.aspose.com/display/emailnet/Working+with+Exchange+Mailbox+and+Messages#WorkingwithExchangeMailboxandMessages-Pre-FetchMessageSize
[5]: https://docs.aspose.com/display/emailnet/Filter+Messages+from+Server+using+IMAP+Client
[6]: http://forum.aspose.com




