---
title: 'Aspose.Network for .NET v3.9.0.0 Released'
date: Mon, 02 Jun 2008 20:16:00 +0000
draft: false
url: /2008/06/02/aspose-network-for-net-v3-9-0-0-released/
author: Iret
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

Aspose.Network for .NET v3.9.0.0 has released.

In this major release, we supported S/MIME protocol features. Now you can add a digital signature to your email message.

Here is the sample code:

       // load the certificate and associated private key from a file   
       X509Certificate2 certificate = X509Certificate2.LoadPfx("mycer.pfx", "password");

       // create an instance of MailMessage   
       MailMessage message = new MailMessage();

        // set its properties to desired values   
        message.From = "[sender@domain.com][1]";  
        message.To = [recipient][2][@domain.com][3];  
        message.Subject = "This is a signed message";  
        message.TextBody = "Hello, world!";  
        // attach a digital signature   
        message.AttachSignature(certificate);  
        SmtpClient.Send(message);

Download Link:

[http://www.aspose.com/community/files/54/utility-components/aspose.network/default.aspx][4]




[1]: mailto:sender@domain.com
[2]: mailto:recipient@domain.com
[3]: mailto:recipient@example.com
[4]: http://www.aspose.com/community/files/54/utility-components/aspose.network/default.aspx




