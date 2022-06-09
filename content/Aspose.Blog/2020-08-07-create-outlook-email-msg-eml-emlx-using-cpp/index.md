---
title: 'Create Outlook Emails (MSG, EML, EMLX) using C++'
seoTitle: ""
description: ""
date: Fri, 07 Aug 2020 15:33:07 +0000
draft: false
url: /2020/08/07/create-outlook-email-msg-eml-emlx-using-cpp/
author: Usman Aziz
summary: ''
tags: ['cpp outlook email API', 'create emails in cpp', 'create outlook emails in cpp', 'save outlook email as draft in cpp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Create-Outlook-Emails-in-C.jpg" alt="Create Outlook Emails in C++">}}


Email Automation is quite popular these days for generating and sending emails automatically from within the web or desktop applications. It is being used for sending important notifications, documents, newsletters, and various kinds of other messages. In order to develop an automated email system, Aspose facilitates the developers with its email API - [Aspose.Email][1]. Today, I'm going to pick up the C++ variant of Aspose.Email and show you **how to create Outlook emails using C++**.

*   [C++ Email Library][2]
*   [Create an Outlook Email using C++][3]
*   [Create an Outlook Email with HTML Body using C++][4]
*   [Set Encoding for Outlook Email using C++][5]
*   [Save Outlook Message as Draft using C++][6]

## C++ Email Library to Create Outlook Emails {#C++-Email-Library}

[Aspose.Email for C++][7] is a native C++ library that lets you create and send emails of MS Outlook and other popular email formats. It also allows you to manipulate Outlook objects such as calendars, tasks, contacts, etc. and convert the existing email files to other formats. You can download the complete library package from [here][8] or install it within your C++ application using [NuGet][9].

## Create an Outlook Email using C++

First of all, let's check out how to create a simple email message and save it in an email format such as MSG, EML, and EMLX. The following are the steps to create an email message using Aspose.Email for C++.

*   Create an instance of [MailMessage][10] class.
*   Set the message’s properties such as To, From, and Body.
*   Save the email message using [MailMessage->Save()][11] method.

The following code sample shows how to create an Outlook message in a particular email format using C++.

{{< gist aspose-com-gists d72533ad16b377f605e3af93f410cb26 "create-outlook-email.cpp" >}}

## Create an Outlook Email with HTML Body using C++ {#Create-an-Email-with-HTML-Body-using-C++}

In the previous example, we have created an email with plain text. However, most of the emails these days contain an HTML body for a fine presentation of the email's content. In such a case, you can configure Aspose.Email and set the HTML-based body of the email. For this, just use [MailMessage->set\_HtmlBody(System::String)][12] and pass to it the HTML content. The following code sample shows how to create an email with an HTML body using C++.

{{< gist aspose-com-gists d72533ad16b377f605e3af93f410cb26 "create-outlook-email-HTML.cpp" >}}

## Set Encoding for Outlook Email using C++ {#Create-an-email-with-a-particular-encoding-using-C++}

Aspose.Email for C++ also lets you define the encoding standard to guide the browser about how to deal with characters in the email. For setting the particular encoding standard, you can use [MailMessage->set\_BodyEncoding(System::Text::Encoding)][13] method. The following code sample shows how to create an email with particular encoding using C++.

{{< gist aspose-com-gists d72533ad16b377f605e3af93f410cb26 "create-outlook-email-encoding.cpp" >}}

## Save Outlook Message as Draft using C++

You can also save the newly created Outlook email message as a draft. The following are the steps to perform this operation:

*   Create a new email or load an existing one using the [MailMessage][14] object.
*   Create a _MapiMessage_ object from the Outlook mail message.
*   Use [MapiMessage->SetMessageFlags(Aspose::Email::Mapi::MapiMessageFlags)][15] method to set email message as draft.
*   Save the Outlook email.

The following code sample shows how to create an email as a draft using C++.

{{< gist aspose-com-gists d72533ad16b377f605e3af93f410cb26 "create-outlook-email-draft.cpp" >}}

## Live Demos

*   [Email Editor][16]
*   [EML Editor][17]
*   [MSG Editor][18]

## Conclusion

In this article, I have shown you **how to create Outlook emails within C++ applications**. The C++ code samples demonstrated how to create MSG, EML or EMLX emails with text/HTML body or a particular encoding. You can [explore more][19] about how to deal with Outlook emails and other items using Aspose.Email for C++.

## See Also

*   [Create and send Outlook emails using C#][20]




[1]: https://products.aspose.com/email
[2]: #C++-Email-Library
[3]: #Create-Email-Messages-using-C++
[4]: #Create-an-Email-with-HTML-Body-using-C++
[5]: #Create-an-email-with-a-particular-encoding-using-C++
[6]: #Save-Outlook-Message-as-Draft-using-C++
[7]: https://products.aspose.com/email/cpp
[8]: https://downloads.aspose.com/email/cpp
[9]: https://www.nuget.org/packages/Aspose.email.cpp
[10]: https://apireference.aspose.com/email/cpp/class/aspose.email.mail_message
[11]: https://apireference.aspose.com/email/cpp/class/aspose.email.mail_message#a41d3ada3ca8b7ca8130629b616f0b91c
[12]: https://apireference.aspose.com/email/cpp/class/aspose.email.mail_message#a23c43a950d6fe4331e62dbb2824a5864
[13]: https://apireference.aspose.com/email/cpp/class/aspose.email.mail_message#a79c9d4b420c46995cb8311dcad05c300
[14]: https://apireference.aspose.com/email/cpp/class/aspose.email.mail_message
[15]: https://apireference.aspose.com/email/cpp/class/aspose.email.mapi.mapi_message_item_base#a4493e690628abea578a38b9c8a335eca
[16]: https://products.aspose.app/email/editor
[17]: https://products.aspose.app/email/editor/eml
[18]: https://products.aspose.app/email/editor/msg
[19]: https://docs.aspose.com/email/cpp/
[20]: https://blog.aspose.com/2020/01/23/create-send-outlook-email-eml-msg-csharp-net-core/





