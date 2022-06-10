---
title: 'Convert an MSG Message to TIFF with the MailPrinter Class'
date: Mon, 02 Jan 2012 17:06:26 +0000
draft: false
url: /2012/01/02/convert-message-to-tiff-with-mailprinter-class/
author: Babar Raza
summary: ''
tags: ['Convert .msg email messages to TIFF', 'Convert MSG to TIFF', 'Microsoft Outlook']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose.email-logo120.jpg" alt="Aspose.Email logo">}}


We are pleased to announce the release of Aspose.Email for .NET 1.3. We've added a number of new features, including auto-detecting message file format, extracting embedded objects data and support for EMLX format. A feature we want to draw your attention to is support for converting email messages to TIFF format using the Aspose.Email.Printing.MailPrinter class.

The Print() method takes an instance of the MailMessage class as an argument, so you can convert EML, MSG or MHT files. This sample code shows how to print an email:

```
// Initialize the MailPrinter class
var msgPrinter = new Aspose.Email.Printing.MailPrinter();
// Load an email message
MailMessage msg = MailMessage.Load("attached and embedded image.msg", MessageFormat.Msg);
// Call Print() method
msgPrinter.Print(msg, "test.tiff", Aspose.Email.Printing.PrintFormat.Tiff);
```

Aspose.Email for .NET 1.3 also contains other new features and bug fixes. For a complete list and the download, please visit [here][1].




[1]: https://downloads.aspose.com/




