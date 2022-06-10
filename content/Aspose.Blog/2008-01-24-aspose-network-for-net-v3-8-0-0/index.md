---
title: 'Aspose.Network for .NET v3.8.0.0'
date: Thu, 24 Jan 2008 16:55:00 +0000
draft: false
url: /2008/01/24/aspose-network-for-net-v3-8-0-0/
author: Iret
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

**Aspose.Network for .NET v3.8.0.0** has been released. Aspose.Network is a complete solution for network programming on .NET frameworks.

This version is a major release, including SSL support for IMAP and POP3, bug fixes and many other improvements.

**New Features**

*   **SSL** on POP3 Protocol.
*   **Implicit / Explicit** security mode for SSL POP3
*   **SSL** on IMAP Protocol
*   **Implicit / Explicit** security mode for SSL IMAP
*   Updated Help document and code samples.

          Aspose.Network now supports using Secure Sockets Layer (SSL) to encrypt the connection (POP3/IMAP). With a few lines of code you can easily access your gmail account with Aspose.Network. Following is the sample to connect to your gmail account in C# using Aspose.Network.ImapClient.

          \[C# Sample\]

        //create imap client with specified server, username and password.  
        ImapClient client = new ImapClient("imap.gmail.com", 993, "[youraccount@google.com][1]", "password");  
        client.EnableSsl = true;  
        client.SecurityMode = ImapSslSecurityMode.Implicit;  
        //connect and login to the imap server  
        client.Connect(true);  
        //select the inbox as the current working folder  
        client.SelectFolder("inbox");  
        //save the message  
        client.SaveMessage(1, "file.eml");  
 **Bug Fixes**

*   NETWORK-4331 MailMessage.Save will throw exceptions for some outlook message files.
*   NETWORK-4332 MailMessage.Load will crash for invalid email address contained in the Outlook message files, like ';'.
*   NETWORK-4333 EmailVerify cannot reuse socket.
*   NETWORK-4334 SmtpClient need to use DNS lookup to identify the host name. 
*   NETWORK-4335 EmailVerify need to cache the MX records properly for performance.

**HowTo Download**

*   [http://www.aspose.com/Community/Files/54/aspose.network/default.aspx][2]




[1]: mailto:youraccount@google.com
[2]: http://www.aspose.com/Community/Files/54/aspose.network/default.aspx




