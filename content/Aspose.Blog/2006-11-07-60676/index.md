---
title: 'Aspose.Network.Mail , System.Net.Mail and System.Web.Mail'
date: Tue, 07 Nov 2006 00:23:00 +0000
draft: false
url: /2006/11/07/60676/
author: Iret
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

In this article, we will talk about the differences among Aspose.Network.Mail, System.Net.Mail (New in .NET 2.0) and System.Web.Mail.

System.Web.Mail and System.Net.Mail are all the built-in library provided by Microsoft in .NET framework. System.Web.Mail supports .NET 1.1 and .NET 2.0 (for compatibility). System.Net.Mail is new for .NET 2.0.

System.Web.Mail is simply a wrapper around the two COM libraries: CDONTS.NewMail (found in the cdonts.dll) and CDO.Message (found in the cdosys.dll). You will also need them installed on your server. By default, cdonts.dll, and cdosys.dll will be installed in WindowsNT/2000/XP/2003.

What’s more, if you trace into the class, System.Web.Mail.SmtpMail, you can find some odd behaviors:

· It only supports Win32NT operation systems, for example, windows 2000, windows 2003, windows XP.

· When the SmtpMail class sends the MailMesage, the SmtMail class checks the OS version. If the version is <= 4, the CDONTS.Newmail object is used. For all OS’s greater than 4, the CDO.Message object is used.

Because of these conditions, your troubleshooting will become much more difficult, when moving the code to different OS’s. And your application may get unexpected results from different OS.

System.Net.Mail is a new SMTP protocol client implementation in .NET 2.0. It is also a pure managed code implementation used C#. However, System.Net.Mail only provides simple E-Mail sending function and not support .NET 1.1

Aspose.Networ.Mail is a pure C#, full managed code .NET component. It has Zero reliance on any COM libraries, including CDONTS.NewMail, or CDO.Message. Therefore, with the help of Aspose.Network.Mail, you can avoid invoking any unmanaged code in your applications, increasing reliability and free of boring COM debugging. Aspose.Network.Mail is features rich and provides much more services than those are provided by System.Web.Email architect. Aspose.Network.Mail supports not only .NET 1.1 but also supports .NET 2.0.

Here is the Matrix

**Aspose.Network**

**System.Web.Mail**

**System.Net.Mail**

**_Compatibility_**

Support .NET 1.1

√

√

×

Support .NET 2.0

√

√

√

**_Common features_**

CDO/CDONTS Dependency

×

√

×

Pure Managed Code

√

×

√

Authentications

√

√

√

Sender address

√

√

√

Recipients address

√

√

√

HTML Body

√

√

√

Text Body

√

√

√

Bcc/Cc

√

√

√

Send Attachment

√

√

√

Linked Image

√

√

√

Body Encoding (Unicode/ASCII)

√

√

√

Subject Encoding (Unicode/ASCII)

√

×

√

Synchronous programming model

√

×

√

Asynchronous programming model

√

×

√

**_Unique features_**

Customized Mail Header

√

×

×

Importance Header

√

×

×

Sensitivity Header

√

×

×

X-Mailer Header

√

×

×

Reply to

√

×

×

Send Date

√

×

×

Template-based Mail Merge

√

×

×

Mail Merge from DataSet

√

×

×

Mail Merge from DataTable

√

×

×

Mail Merge from DataReader

√

×

×

Bulk Send with Multi-threading

√

×

×

Send Calendar

√

×

×

Send Meeting request

√

×

×

**_Formatting / Loading_**

Load from Microsoft Msg format

√

×

×

Load from Microsoft Mht format

√

×

×

Save to Microsoft Mht format

√

×

×

Save to Eml format

√

×

×

Load from Eml format

√

×

×

Load from RFC 822 compliant file

√

×

×

**_Interoperation_**

Works with Aspose.Network.Pop3

√

×

×

Works with Aspose.Network.Imap

√

×

×

Works with Aspose.Network.Mime

√

×

×








