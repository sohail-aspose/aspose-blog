---
title: 'Send Word Document in Email Body using C#'
seoTitle: "Send Word Document as Email using C# | Import Word Doc in Email Body"
description: "Use .NET APIs to send MS Word document as email using C#. Import content from Word document into email body within .NET applications."
date: Tue, 16 Feb 2021 02:06:00 +0000
draft: false
url: /2021/02/16/send-word-document-in-email-body-using-csharp/
author: Usman Aziz
summary: "The presentation of the emails' body is one of the important factors to engage the readers. Therefore, emails are well formatted using headings, subheadings, tables, images, and etc. However, most of the built-in email editors do not provide advanced formatting options. In order to tackle this limitation, this article covers **how to compose your emails using Word documents as email body in C#**."
tags: ['Import Word Doc in Email Body csharp', 'Send Word Document as Email using Csharp']
categories: ['Aspose.Words Product Family', 'Aspose.Total Product Family', 'Aspose.Email Product Family']
---



{{< figure align=center src="images/Send-Word-Document-in-Email.jpg" alt="Send word document in email c#">}}


The presentation of the emails' body is one of the important factors to engage the readers. Therefore, emails are well formatted using headings, subheadings, tables, images, and etc. However, most of the built-in email editors do not provide advanced formatting options. In order to tackle this limitation, this article covers **how to compose your emails using Word documents as email body in [C#][1]**.

*   [C# APIs to Import Word Document to Email][2]
*   [Steps to Send Word Document in Email Body in C#][3]
*   [Complete Source Code][4]
*   [Get a Free API License][5]

## C# APIs to Import Word Document to Email {#APIs-to-Import-Word-Document-to-Email}

In order to import the content from a Word document, we'll use [Aspose.Words for .NET][6] API. Whereas, to compose and send the email, we'll leverage the capabilities of [Aspose.Email for .NET][7]. Both of the above-mentioned APIs can either be downloaded as DLL or installed via NuGet.

### Download DLLs

*   [Aspose.Words for .NET][8]
*   [Aspose.Email for .NET][9]

### Install via NuGet```
PM> Install-Package Aspose.Words
PM> Install-Package Aspose.Email
```

## Send Word Document in Email Body using C# {#Steps-to-Send-Word-Document-in-Email-Body-in-csharp}

**1.** Load the Word document using the [Aspose.Words.Document][10] class and save it as MHTML into a [MemoryStream][11] object.

{{< gist aspose-com-gists 3837cf82825bad3a302f30f13a6b9c32 "load-word-document.cs" >}}

**2.** Load the MHTML from the _MemoryStream_ object to [Aspose.Email.MailMessage][12] object and set _subject_, _to_ and _from_ fields of the email.

{{< gist aspose-com-gists 3837cf82825bad3a302f30f13a6b9c32 "create-email-from-word-doc.cs" >}}

**3.** Set up SMTP client using [Aspose.Email.Clients.Smtp.SmtpClient][13] class and send the email.

{{< gist aspose-com-gists 3837cf82825bad3a302f30f13a6b9c32 "send-email.cs" >}}

## Source Code {#Complete-Source-Code}

The following is the complete source code of importing MS Word document as an email body using C#.

{{< gist aspose-com-gists 3837cf82825bad3a302f30f13a6b9c32 "send-word-doc-as-email.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try the API without evaluation limitations for free. [Get a free temporary license][14] now.

## Conclusion

In this article, you have learned how to import a Word document as an email body using C#. Furthermore, the code sample has shown how to send the composed email message using an SMTP client. You can explore more about the APIs being used in the article by visiting the following documentations.

*   [Aspose.Words for .NET][15]
*   [Aspose.Email for .NET][16]

## See Also

*   [Convert Email Messages to PDF using C#][17]




[1]: https://docs.fileformat.com/programming/cs/
[2]: #APIs-to-Import-Word-Document-to-Email
[3]: #Steps-to-Send-Word-Document-in-Email-Body-in-csharp
[4]: #Complete-Source-Code
[5]: #Get-a-Free-API-License
[6]: https://products.aspose.com/words/net
[7]: https://products.aspose.com/email/net
[8]: https://downloads.aspose.com/words/net
[9]: https://downloads.aspose.com/email/net
[10]: https://apireference.aspose.com/words/net/aspose.words/document
[11]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream
[12]: https://apireference.aspose.com/email/net/aspose.email/mailmessage
[13]: https://apireference.aspose.com/email/net/aspose.email.clients.smtp/smtpclient
[14]: https://purchase.aspose.com/temporary-license
[15]: https://docs.aspose.com/words/net
[16]: https://docs.aspose.com/email/net
[17]: https://blog.aspose.com/2021/01/07/convert-emails-to-pdf-using-csharp/





