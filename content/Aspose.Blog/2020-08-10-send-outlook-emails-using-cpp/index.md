---
title: 'Send Outlook Emails (MSG, EML, EMLX) using C++'
seoTitle: ""
description: ""
date: Mon, 10 Aug 2020 15:10:30 +0000
draft: false
url: /2020/08/10/send-outlook-emails-using-cpp/
author: Usman Aziz
summary: ''
tags: ['send bulk emails in cpp', 'send email as tnef using cpp', 'send emails with smtp using cpp', 'send outlook email using cpp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Send-Outlook-Emails-in-C.jpg" alt="Send Outlook Emails in C++">}}


In the [previous article][1], you have seen how to create MS Outlook emails including [MSG][2], [EML][3], and [EMLX][4] programmatically using [C++][5]. In this post, you'll learn how to **send Outlook emails from within C++ applications**. The emails can be created on the runtime or loaded from already saved email files such as _.msg_, _.emlx_, or etc.

*   [C++ Email Library][6]
*   [Send Outlook Emails using in C++][7]
*   [Send Outlook Emails with Alternate View using C++][8]
*   [Create and Send Bulk Emails using C++][9]
*   [Send Emails as TNEF using C++][10]

## Send Emails with C++ Email Library - Free Download {#C++-Email-Library}

Likewise the [previous post][11], we'll use [Aspose.Email for C++][12] to send the Outlook emails. You can download the library files from the [Downloads][13] section or install it using [NuGet][14].

## Send Outlook Emails using C++ {#Send-Outlook-Emails-using-SMTP-in-C++}

The following are the steps to send an Outlook email with SMTP client using Aspose.Email for C++.

*   Create an Outlook email or load it from a file using the [MailMessage][15] class.
*   Create an object of [SmtpClient][16].
*   Set host, username, password, and port number.
*   Set security options.
*   Send email using _SmtpClient->Send()_ method.

The following code sample shows how to send an Outlook email using C++.

{{< gist aspose-com-gists d72533ad16b377f605e3af93f410cb26 "send-outlook-email.cpp" >}}

## C++ Send Outlook Emails with Alternate View {#Send-Outlook-Emails-with-Alternate-View-using-C++}

You may also specify an alternate view of the email to create a copy of the message in a different format. For instance, if your message is in HTML format, you can create an alternate view having a plain text. In order to create an alternate view, you can use [MailMessage->get\_AlternateViews()->Add(AlternateView::CreateAlternateViewFromString(u"text"))][17] method.

The following code sample shows how to send an email with an alternate view using C++.

{{< gist aspose-com-gists d72533ad16b377f605e3af93f410cb26 "send-outlook-email-alternate-view.cpp" >}}

## Send Bulk Emails using C++ {#Create-and-Send-Bulk-Emails-using-C++}

There might be the case when you need to send a bulk of emails at a time. For such cases, Aspose.Email for C++ provides [MailMessageCollection][18] class to encapsulate multiple email messages. The following are steps to send the bulk of emails.

*   Create or load email messages using the [MailMessage][19] class.
*   Create an object of the [MailMessageCollection][20] class.
*   Add email messages to the collection using _MailMessageCollection->add()_ method.
*   Create an object of the [SmtpClient][21] class.
*   Send bulk emails using _SmtpClient->Send(MailMessageCollection)_ method.

The following code sample shows how to send the bulk of emails using C++.

{{< gist aspose-com-gists d72533ad16b377f605e3af93f410cb26 "send-outlook-email-bulk.cpp" >}}

## C++ Send Emails as TNEF {#Send-Emails-as-TNEF-using-C++}

MS Outlook uses [Transport Neutral Encapsulation Format][22] (TNEF) to send the emails having RTF bodies. In this case, the formatting is extracted from the email and it is encoded as TNEF. At the receiving end, if the client supports TNEF, it assembles the plain text and the TNEF attachment to create the RTF email. Otherwise, the email is displayed as plain text. In order to send emails as TNEF, you can use _SmtpClient->set\_UseTnef(bool)_ method.

The following code sample shows how to send an Outlook email as TNEF using C++.

{{< gist aspose-com-gists d72533ad16b377f605e3af93f410cb26 "send-outlook-email-tnef.cpp" >}}

## Conclusion

In this post, you have seen how to **send Outlook emails using C++**. In addition, you have come to know how to send bulk emails, send emails with an alternate view, or send emails as TNEF within C++ applications. You can explore more about Aspose's C++ email library using the [documentation][23].

## See Also

*   [Create and Send Outlook Emails using C#][24]




[1]: https://blog.aspose.com/2020/08/07/create-outlook-email-msg-eml-emlx-using-cpp/
[2]: https://docs.fileformat.com/email/msg/
[3]: https://docs.fileformat.com/email/eml/
[4]: https://docs.fileformat.com/email/emlx/
[5]: https://docs.fileformat.com/programming/cpp/
[6]: #C++-Email-Library
[7]: #Send-Outlook-Emails-using-SMTP-in-C++
[8]: #Send-Outlook-Emails-with-Alternate-View-using-C++
[9]: #Create-and-Send-Bulk-Emails-using-C++
[10]: #Send-Emails-as-TNEF-using-C++
[11]: https://blog.aspose.com/2020/08/07/create-outlook-email-msg-eml-emlx-using-cpp/
[12]: https://products.aspose.com/email/cpp
[13]: https://downloads.aspose.com/email/cpp
[14]: https://www.nuget.org/packages/Aspose.email.cpp
[15]: https://apireference.aspose.com/email/cpp/class/aspose.email.mail_message
[16]: https://apireference.aspose.com/email/cpp/namespace/aspose.email.clients.smtp
[17]: https://apireference.aspose.com/email/cpp/class/aspose.email.mail_message#a680053eb2a28e287e908bd8908b304b6
[18]: https://apireference.aspose.com/email/cpp/class/aspose.email.mail_message_collection/
[19]: https://apireference.aspose.com/email/cpp/class/aspose.email.mail_message
[20]: https://apireference.aspose.com/email/cpp/class/aspose.email.mail_message_collection/
[21]: https://apireference.aspose.com/email/cpp/namespace/aspose.email.clients.smtp
[22]: https://en.wikipedia.org/wiki/Transport_Neutral_Encapsulation_Format
[23]: https://docs.aspose.com/email/cpp/developer-guide/
[24]: https://blog.aspose.com/2020/01/23/create-send-outlook-email-eml-msg-csharp-net-core/





