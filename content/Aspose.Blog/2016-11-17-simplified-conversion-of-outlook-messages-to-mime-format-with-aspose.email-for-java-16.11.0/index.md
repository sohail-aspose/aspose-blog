---
title: 'Simplified Conversion of Outlook Messages to MIME Format with Aspose.Email for Java 16.11.0'
date: Thu, 17 Nov 2016 14:13:41 +0000
draft: false
url: /2016/11/17/simplified-conversion-of-outlook-messages-to-mime-format-with-aspose.email-for-java-16.11.0/
author: Kashif Iqbal
summary: ''
tags: ['Convert Outlook Message to MIME', 'Convert Outlook Message to MIME in Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="Convert Outlook to MIME Format">}}


[Aspose.Email for Java 16.11.0][1] has been released. Ported from its equivalent [.NET version][2], this month’s release includes the same features, enhancements and bug fixes that were part of the .NET version of the API. Specifically, it enhances the functionality of Outlook MSG conversion to MIME message. For a detailed note on what is new and fixed, please visit our documentation section for [release notes][3] of this month’s version.

## Convert Outlook Message to MIME Format in Java

**Outlook MSG conversion to MIME:** This month’s release simplifies the conversion process [of Outlook messages (MSG) to MIME][4]. Instead of using the MailMessageInterpreter class, the API provides overloads of MapiMesasge class’s save method to save MSG file to EML. In addition, the MapiMessage class now exposes toMailMessage method that converts MSG files to EML with additional options. The following code sample shows the usage of this API functionality.

```
MapiMessage msg = new MapiMessage(
"sender@test.com", 
"recipient1@test.com; recipient2@test.com", 
"Test Subject", 
"This is a body of message.");
MailConversionOptions options = new MailConversionOptions();
options.setConvertAsTnef(true);
MailMessage mail = msg.toMailMessage(options);

ByteArrayOutputStream ms = new ByteArrayOutputStream();
msg.save(ms, SaveOptions.getDefaultHtml());

String fileName = "savedMessage.eml";
msg.save(fileName, SaveOptions.getDefaultEml()); 
```

**Provision of BCC field in Exhcnage Message Summary Information:** This month’s release also enhances the ExchangeMessageInfo class for retrieving BCC information from email messages. This is helpful in retrieving the information for email messages from mailbox’s Draft as well as Sent Items folder.

## Other Improvements

This month’s release also fixes several bugs that further adds to the overall functional improvement of the API.

## API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   [Product Documentation][5] – Provides detailed examples of working with the API
*   [API Reference Guide][6] – Details all the packages and classes of the API
*   [GitHub Examples][7] – Provides ready to run API examples
*   [Aspose.Email Forum][8] – Feel free to contact us on Aspose.Email forum for your queries




[1]: https://downloads.aspose.com/email/java
[2]: https://blog.aspose.com/2016/11/17/outlook-msg-files-conversion-to-mime-simplified-with-aspose.email-for-.net-16.11.0/
[3]: https://docs.aspose.com/display/emailjava/Home
[4]: https://docs.aspose.com/display/emailjava/Creating+and+Saving+MSG+files
[5]: https://docs.aspose.com/display/emailjava/Home
[6]: https://apireference.aspose.com/java/email
[7]: https://github.com/aspose-email/Aspose.Email-for-Java
[8]: https://forum.aspose.com/c/email




