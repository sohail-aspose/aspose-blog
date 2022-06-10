---
title: 'Print Email Message to XPS with Aspose.Email for .NET'
date: Mon, 05 Dec 2011 06:36:47 +0000
draft: false
url: /2011/12/05/print-email-message-to-xps/
author: Saqib Razzaq
summary: ''
tags: ['.NET', 'XPS', 'email', 'email programming', 'eml', 'msg', 'print message', 'print message to xps', 'product release']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose.email-logo120.jpg" alt="Aspose.Email logo">}}


We are pleased to announce the release of [Aspose.Email for .NET][1] 1.2. In this version, we have added support for printing email messages to XPS format using the MailPrinter class. The Print() method takes an instance of the MailMessage class as an argument, so you can print EML, MSG, or MHT files. This sample code shows how to print an email:

```
// Initialize the MailPrinter class
MailPrinter msgPrinter = new MailPrinter();
// Load an email message
MailMessage msg = MailMessage.Load("attached and embedded image.msg", MessageFormat.Msg);
// Call Print() method
msgPrinter.Print(msg, "test.xps", PrintFormat.XPS);
```

Aspose.Email for .NET 1.2 also contains some other new features and bug fixes. For a complete list and the download, please visit: [https://downloads.aspose.com/email/net][2]




[1]: https://products.aspose.com/email/net
[2]: https://downloads.aspose.com/email/net




