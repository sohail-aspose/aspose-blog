---
title: 'Aspose.Network for .NET v3.7.0.0'
date: Fri, 04 Jan 2008 02:46:00 +0000
draft: false
url: /2008/01/04/aspose-network-for-net-v3-7-0-0/
author: Iret
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

**Aspose.Network for .NET v3.7.0.0** has been released. Aspose.Network is a complete solution for network programming on .NET frameworks.

This version is a major release, containing SSL support for SMTP, bug fixes and many other improvements.

**New Features**

*   SSL SMTP Protocol: Aspose.Network.Mail supports sending email with SSL SMTP protocol.
*   Implicit / Explicit Security mode in SSL SMTP.

          \[C# Sample\]

         SmtpClient client = new SmtpClient("smtp.gmail.com",587,"from@gmail.com","password");

         client.SecurityMode = SmtpSslSecurityMode.Explicit;

         client.EnableSsl = true;

         client.Send("from@aspose.com","to@gmail.com", "Hello, Gmail.", "Hello, Gmail.");

*   VAS/VMS List item : Aspose.Network.Ftp supports parsing VAS/VMS format item list.
*   Pop3 Authentication : Aspose.Network.Pop3 supports 3 types of authentication methods.

**Bug Fixes**

*   4243 IMAP Invalid character in a Base-64 string when listing messages 
*   4244 Pop3Client.State property value is wrong when connecting to remote server.

**HowTo Download**

*   [http://www.aspose.com/Community/Files/54/aspose.network/default.aspx][1]




[1]: http://www.aspose.com/Community/Files/54/aspose.network/default.aspx




