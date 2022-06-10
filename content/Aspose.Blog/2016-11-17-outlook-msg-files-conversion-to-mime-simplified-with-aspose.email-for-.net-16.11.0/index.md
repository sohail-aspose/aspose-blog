---
title: 'Outlook MSG to MIME Conversion with Aspose.Email for .NET 16.11.0'
date: Thu, 17 Nov 2016 13:18:35 +0000
draft: false
url: /2016/11/17/outlook-msg-files-conversion-to-mime-simplified-with-aspose.email-for-.net-16.11.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Aspose.Email-for-.NET_.png" alt="Aspose.Email for .NET">}}


We are pleased to announce the release of [Aspose.Email for .NET 16.11.0][1]. This month’s release includes enhancements where the API functionality is improved by enriching the existing features of the API. It also improves the overall API functionality by fixing several bugs. For a complete list of what is new and fixed, please visit our documentation section for [release notes][2] of this version.

# Enhancements

**Conversion of MSG to EML without using Interpreter classes:** Aspose.Email API uses Interpreter classes for conversion of Microsoft Outlook (MSG) files to Multipurpose Internet Mail Extensions (MIME) messages. This month’s release enhances and simplifies this functionality using the MapiMessage class with its _[toMailMessage][3]_ method. This also provides the capability to specify additional saving options using the _MailConversionOptions_ class.

```
MapiMessage msg = new MapiMessage(
    "sender@test.com",
    "recipient1@test.com; recipient2@test.com",
    "Test Subject",
    "This is a body of message.");
var options = new MailConversionOptions();
options.ConvertAsTnef = true;
MailMessage mail = msg.ToMailMessage(options);

MemoryStream ms = new MemoryStream();
msg.Save(ms, SaveOptions.DefaultHtml);

string fileName = "savedMessage.eml";
msg.Save(fileName , SaveOptions.DefaultEml);
```

**Provision of the BCC field in Exchange Message Summary Information:** This month’s release also modifies the ExchangeMessageInfo summary object by incorporating the BCC field as property in it. This helps retrieve the information in case messages are listed from Drafts or Sent Items folder.

# Other Improvements

This month’s release also fixes several bugs reported with our previous version that further adds stability to the API functionality.

# API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   [Product Documentation][4] – Provides detailed examples of working with the API
*   [API Reference Guide][5] – Details all the namespaces and classes of the API
*   [GitHub Examples][6] – Provides ready to run API example
*   [Support Forum][7] – Write to us if you have any query or inquiry about the API




[1]: http://downloads.aspose.com/email/net
[2]: http://docs.aspose.com/display/emailnet/Aspose.Email+for+.NET+16.11.0+Release+Notes
[3]: http://docs.aspose.com/display/emailnet/Managing+Message+Files+with+Aspose.Email.Outlook#ManagingMessageFileswithAspose.Email.Outlook-ConvertingMSGtoMIMEmessage
[4]: https://docs.aspose.com/display/emailnet/Developer+Guide
[5]: https://apireference.aspose.com/net/email
[6]: https://github.com/aspose-email/Aspose.Email-for-.NET
[7]: https://forum.aspose.com/c/email




