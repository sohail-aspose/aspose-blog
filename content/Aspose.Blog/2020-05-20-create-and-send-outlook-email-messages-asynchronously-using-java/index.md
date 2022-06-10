---
title: 'Create and Send Outlook Email Messages using Java'
seoTitle: "Create and Send Outlook Emails using Java | Send Emails Asynchronously"
description: "Java Email Library to create and send Outlook emails in Java. Send emails synchronously or asynchronously via SMTP using Java. Create MSG, EML, MHT emails."
date: Wed, 20 May 2020 15:30:04 +0000
draft: false
url: /2020/05/20/create-and-send-outlook-email-messages-asynchronously-using-java/
author: Usman Aziz
summary: ''
tags: ['Create Outlook Emails using Java', 'Java Email Library', 'Send Outlook Emails using Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Create-and-Send-Outlook-Emails-Java.jpg" alt="Create and Send Outlook Emails Java">}}


[Aspose.Email for Java][1] is a powerful email processing API that provides all the basic as well as advanced features for email management. It allows you to create Outlook email messages, read existing emails, and convert MSG, EML, PST, OST, MBOX, and MHT messages to other formats from within your Java applications. In this article, I'll demonstrate some basic yet important features of how to create and send Outlook emails using Java.

I am going to cover the following features of creating and sending emails in this article:

*   [Create Outlook email message using Java][2]
*   [Set HTML body for email using Java][3]
*   [Create an email with a particular encoding using Java][4]
*   [Send Outlook emails using Java][5]
*   [Asynchronously send emails using Java][6]
*   [Send an email with a read receipt using Java][7]
*   [Send bulk emails using Java][8]

## Java Email API - Installation

Aspose.Email for Java can be downloaded from the [Downloads][9] section or installed using the following Maven configurations.

### Repository```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```

### Dependency```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-email</artifactId>
    <version>20.3</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Create Outlook Email Messages using Java {#Create-Outlook-email-message-using-Java}

Aspose.Email for Java lets you create email messages and save them in your desired email format including EML, EMLX, MSG, and MHTML. The following are the steps to create an email message and save it as a file.

*   Create an instance of [MailMessage][10] class.
*   Set the message's properties such as Subject, Body, To, CC, etc.
*   Add attachments if required.
*   Save the email message in your desired format using [MailMessage.save()][11] method.

The following code sample shows how to create an Outlook email message using Java.

{{< gist aspose-com-gists 2836280bbb0c0b9ea7df9fd3765751fa "create-outlook-email-message.java" >}}

## Create an Email with HTML Body using Java {#Create-an-email-with-HTML-body-using-Java}

In the previous example, we simply created a plain text email and saved it as an email file. However, most of the emails today are created with HTML body to well organize and present the email's content. In this case, HTML tags are used to specify the layout of the email. Let's see how to create an email with an HTML body using Aspose.Email for Java.

*   Use the [MailMessage][12] class to create a new email message.
*   Set Subject, To, CC, and other properties.
*   Set email's body using [MailMessage.setHtmlBody(string)][13] method.
*   Save the email message using [MailMessage.save()][14] method.

The following code sample shows how to create an email with an HTML body using Java.

{{< gist aspose-com-gists 2836280bbb0c0b9ea7df9fd3765751fa "create-outlook-message-html.java" >}}

## Create an Email with a Particular Encoding using Java {#Create-an-email-with-a-particular-encoding-using-Java}

Aspose.Email for Java also allows you to set the desired text encoding for the email messages. The encoding standard is used to tell the email application or browser about how to interpret the characters in the email’s body. The following are the steps to create an email with a particular encoding standard.

*   Create an object of the [MailMessage][15] class.
*   Set email's properties such as Subject, To, CC, etc.
*   Set encoding standard using [MailMessage.setBodyEncoding()][16] method.
*   Create and save the email using [MailMessage.save()][17] method.

The following code sample shows how to create an email with a particular encoding standard using Java.

{{< gist aspose-com-gists 2836280bbb0c0b9ea7df9fd3765751fa "create-outlook-message-encoding.java" >}}

## Send Outlook Emails using Java {#Send-emails-with-SMTP-client-using-Java}

Once you have created an email, you can send it to its recipients using Simple Mail Transfer Protocol (SMTP). The following are the steps to send an email message using Aspose.Email for Java.

*   Create a new email message or load an existing one using the [MailMessage][18] class.
*   Create an instance of the [SmtpClient][19] class and set its host, username, password, and port.
*   Send email using [SmtpClient.send()][20] method.

The following code sample shows how to send an email via SMTP client in Java.

{{< gist aspose-com-gists 2836280bbb0c0b9ea7df9fd3765751fa "send-outlook-emails.java" >}}

## Send Emails Asynchronously using Java {#Send-emails-asynchronously-using-Java}

Aspose.Email for Java also lets you send emails asynchronously. For this, you can use the [SmtpClient.beginSend()][21] method. The following code sample shows how to send emails asynchronously using Java.

{{< gist aspose-com-gists 2836280bbb0c0b9ea7df9fd3765751fa "send-outlook-emails-async.java" >}}

## Send Emails with a Read Receipt using Java {#Send-an-email-with-a-read-receipt-using-Java}

You can also add a request for a read receipt to the email messages. This feature allows you to receive a notification after the email has been received. The following are the steps to create and send an email message containing a request for read receipt.

*   Create a new email message using the [MailMessage][22] class.
*   Set the delivery notification option using [MailMessage.setDeliveryNotificationOptions()][23] method.
*   Add receipt information in the email headers.
*   Use the [SmtpClient][24] class to send the email.

The following code sample shows how to send an email containing a read receipt using Java.

{{< gist aspose-com-gists 2836280bbb0c0b9ea7df9fd3765751fa "send-email-read-receipt.java" >}}

## Send Bulk Emails using Java {#Send-bulk-emails-using-Java}

There might be the case when you need to send a bulk of different emails. In that case, you can simply add all the email messages to a [MailMessageCollection][25] object and pass it to SMTP client for sending. The following code sample shows how to send a bulk of emails using Java.

{{< gist aspose-com-gists 2836280bbb0c0b9ea7df9fd3765751fa "send-emails-bulk.java" >}}

## Live Demos

*   [Email Editor][26]
*   [EML Editor][27]
*   [MSG Editor][28]

## Conclusion

In this post, I have shown you how to create Outlook email messages and save them as EML, MSG, and MTH formats using Java. In addition, different ways of sending emails in Java using the STMP client are also discussed. You can learn more about Aspose's [Java Email Library][29] using the [documentation][30].

## See Also

*   [Create Outlook Messages and Send Emails using C#][31]




[1]: https://products.aspose.com/email/java
[2]: #Create-Outlook-email-message-using-Java
[3]: #Create-an-email-with-HTML-body-using-Java
[4]: #Create-an-email-with-a-particular-encoding-using-Java
[5]: #Send-emails-with-SMTP-client-using-Java
[6]: #Send-emails-asynchronously-using-Java
[7]: #Send-an-email-with-a-read-receipt-using-Java
[8]: #Send-bulk-emails-using-Java
[9]: https://downloads.aspose.com/email/java
[10]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage
[11]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage#save(java.lang.String,%20com.aspose.email.SaveOptions)
[12]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage
[13]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage#setHtmlBody(java.lang.String)
[14]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage#save(java.lang.String,%20com.aspose.email.SaveOptions)
[15]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage
[16]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage#setBodyEncoding(java.nio.charset.Charset)
[17]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage#save(java.lang.String,%20com.aspose.email.SaveOptions)
[18]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage
[19]: https://apireference.aspose.com/email/java/com.aspose.email/SmtpClient
[20]: https://apireference.aspose.com/email/java/com.aspose.email/SmtpClient#send(com.aspose.email.MailMessage)
[21]: https://apireference.aspose.com/email/java/com.aspose.email/SmtpClient#beginSend(com.aspose.email.MailMessage)
[22]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage
[23]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage#setDeliveryNotificationOptions(int)
[24]: https://apireference.aspose.com/email/java/com.aspose.email/SmtpClient
[25]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessageCollection
[26]: https://products.aspose.app/email/editor
[27]: https://products.aspose.app/email/editor/eml
[28]: https://products.aspose.app/email/editor/msg
[29]: https://products.aspose.com/email/java
[30]: https://docs.aspose.com/display/emailjava/Product+Overview
[31]: https://blog.aspose.com/2020/01/23/create-send-outlook-email-eml-msg-csharp-net-core/





