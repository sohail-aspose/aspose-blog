---
title: 'Create and Send Outlook Emails using C# .NET or .NET Core'
seoTitle: "C# Send Outlook Emails | Create Outlook Email in ASP.NET | C# Email API"
description: "C# .NET Email Library. Send Outlook emails in C# using SMTP. Send emails asynchronously in ASP.NET C#. Create and send emails (MSG, EML) in C# .NET Core."
date: Thu, 23 Jan 2020 08:55:49 +0000
draft: false
url: /2020/01/23/create-send-outlook-email-eml-msg-csharp-net-core/
author: Usman Aziz
summary: "In this blog, you will learn how to **create Outlook email** messages (including MSG, EML, EMLX, or MHTML) and **send emails** **synchronously** or **asynchronously** using **C#** in **.NET** or **.NET Core**."
tags: ['C# .net email library', 'create and send outlook emails', 'create outlook msg in C# .net', 'send email in C# .net', 'send emails asynchronously']
categories: ['Aspose.Email Product Family']
---

In this blog, you will learn how to **create Outlook email** messages (including MSG, EML, EMLX, or MHTML) and **send emails** **synchronously** or **asynchronously** using **C#** in **.NET** or **.NET Core**.



{{< figure align=center src="images/Send-Email-in-C.png" alt="C# send outlook email ">}}


The **email** has become a primary source of exchanging messages and sharing content such as documents, images, or other types of files. The frequency of using emails is more within the online systems for sharing important notifications or documents with multiple entities. In such cases, preparing a template and sending emails to multiple stakeholders manually could be a time-consuming and hectic task.

Here comes the need for an **Email Automation Service** using which you can create and send emails seamlessly. So in this article, I am going to teach you how to create email messages of popular Outlook formats and automate the process of sending emails programmatically. After reading this article, you will be able to:

*   create and save an email message in C#,
*   create an email with HTML body in C#,
*   create an email with a particular encoding in C#,
*   send emails synchronously using SMTP in C#,
*   send emails asynchronously using SMTP in C#,
*   and send bulk emails in C#.

## C# API to Create and Send Outlook Emails

In order to automate the process of creating and sending email messages, we will use [Aspose.Email for .NET][1] which is a powerful email manipulation and processing API. It supports popular email formats including MS Outlook messages such as MSG, EML/EMLX, etc. You can directly download the API's [DLL][2] or install it via [NuGet Package Manager][3] or Package Manager Console in Visual Studio.

```
PM> Install-Package Aspose.Email
```

After you have created a C# (Console, ASP.NET, etc.) application and installed _Aspose.Email for .NET_, you can begin creating and sending the emails in C#.

## Create an Outlook Email in C#

In order to create or manipulate Outlook email messages, _Aspose.Email_ provides the [MailMessage][4] class. This class lets you set all the properties of an email message (_Subject_, _To_, _From_ and _Body_), add attachments, and save the message in different email formats such as EML, MSG, MHTML, etc. The following are the steps to create an email message:

*   Create an instance of _MailMessage_ class.
*   Set the message's properties.
*   Save the email message using _MailMessage.Save()_ method.

The following code sample shows how to create and save an email message in C#.

{{< gist aspose-com-gists 7126ba23a3ba099642e13dbfbfd94970 "create-email-message.cs" >}}

## Create an Outlook Email with HTML Body in C#

The HTML tags are used to make the body of the email more structured, presentable and enriched with different elements such as tables, images, lists, and so on. In case you want to create an email with having HTML body, you can use [MailMessage.HtmlBody][5] property. The following code sample shows how to create an Outlook email with HTML body in C#.

{{< gist aspose-com-gists 7126ba23a3ba099642e13dbfbfd94970 "create-email-html-body.cs" >}}

## Create an Outlook Email with a Particular Encoding in C#

You can also specify your desired encoding standard to tell the browser or email application about how to interpret the characters in the email's body. The [MailMessage.BodyEncoding][6] property is used for this purpose. The following code sample shows how to set body encoding when creating an Outlook email using C#.

{{< gist aspose-com-gists 7126ba23a3ba099642e13dbfbfd94970 "create-email-message-body-encoding.cs" >}}

## Send Outlook Emails Synchronously or Asynchronously in C#

Now, once you have created the email message, you can send it to its recipients synchronously or asynchronously. The [SmtpClient][7] class lets you send the Outlook email messages using SMTP (Simple Mail Transfer Protocol). The following are the steps to send an email in C# using _Aspose.Email for .NET_.

*   Create or load an email message using the _MailMessage_ class.
*   Create an instance of _SmtpClient_ class and set host, username, password and port number.
*   Send email synchronously or asynchronously using [SmtpClient.Send][8] or [SmtpClient.SendAsync][9] method respectively.

### Send an Outlook Email Synchronously in C#

{{< gist aspose-com-gists 7126ba23a3ba099642e13dbfbfd94970 "send-email-synchronously-using-smtp.cs" >}}

### Send an Outlook Email Asynchronously in C#

{{< gist aspose-com-gists 7126ba23a3ba099642e13dbfbfd94970 "send-email-asynchronously-using-smtp.cs" >}}

## Send Bulk Emails in C#

You can also create and send emails in bulk. The [MailMessageCollection][10] class is used to contain the collection of email messages you want to send. The following code sample shows how to send bulk emails in C#.

{{< gist aspose-com-gists 7126ba23a3ba099642e13dbfbfd94970 "send-bulk-emails-using-smtp.cs" >}}

## Live Demos

*   [Email Editor][11]
*   [EML Editor][12]
*   [MSG Editor][13]

## Conclusion

In this article, you have learned how to create Outlook emails in C#. Furthermore, you have seen how to send emails synchronously or asynchronously from within .NET applications. You can explore the [documentation][14] of _Aspose.Email for .NET_ to learn more about the API.

## See Also

*   [Send Word Document in Email Body using C#][15]




[1]: https://products.aspose.com/email
[2]: https://downloads.aspose.com/email/net
[3]: https://www.nuget.org/packages/aspose.email
[4]: https://apireference.aspose.com/net/email/aspose.email/mailmessage
[5]: https://apireference.aspose.com/net/email/aspose.email/mailmessage/properties/htmlbody
[6]: https://apireference.aspose.com/net/email/aspose.email/mailmessage/properties/bodyencoding
[7]: https://apireference.aspose.com/net/email/aspose.email.clients.smtp/smtpclient
[8]: https://apireference.aspose.com/net/email/aspose.email.clients.smtp.smtpclient/send/methods/5
[9]: https://apireference.aspose.com/email/net/aspose.email.clients.smtp.smtpclient/sendasync/methods/10
[10]: https://apireference.aspose.com/net/email/aspose.email/mailmessagecollection
[11]: https://products.aspose.app/email/editor
[12]: https://products.aspose.app/email/editor/eml
[13]: https://products.aspose.app/email/editor/msg
[14]: https://docs.aspose.com/display/emailnet/Developer+Guide
[15]: https://blog.aspose.com/2021/02/16/send-word-document-in-email-body-using-csharp/





