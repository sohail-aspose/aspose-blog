---
title: 'Convert MSG and EML Emails to HTML using C#'
seoTitle: "Convert Email to HTML in C# | MSG or EML to HTML and MHTML"
description: "Use .NET email API to convert emails to HTML or MHTML formats using C#. Convert MSG or EML emails to HTML or MHTML within a couple of steps in C#."
date: Mon, 15 Feb 2021 10:47:00 +0000
draft: false
url: /2021/02/15/msg-and-eml-emails-to-html-using-csharp/
author: Usman Aziz
summary: 'In order to embed the content of the emails into the web pages, you would need to convert them into HTML format. For such cases, this article covers how to automate email to HTML conversion in .NET applications. Particularly, you will learn **how to convert [MSG][1] and [EML][2] email files to [HTML][3] or [MHTML][4] format using C#**.'
tags: ['email to html csharp', 'eml to html csharp', 'eml to mhtml csharp', 'msg to html csharp', 'msg to mhtml csharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Email-to-HTML.jpg" alt="C# Email to HTML ">}}


In order to embed the content of the emails into the web pages, you would need to convert them into [HTML][5] format. For such cases, this article covers how to automate an email to HTML conversion in .NET applications. Particularly, you will learn **how to convert [MSG][6] and [EML][7] emails to [HTML][8] or [MHTML][9] format using [C#][10]**.

*   [C# Email to HTML Converter API][11]
*   [Convert MSG/EML to HTML using C#][12]
*   [Convert MSG/EML to MHTML using C#][13]
*   [Get a Free API License][14]

## C# Email to HTML Converter API {#CSharp-Email-to-HTML-Converter-API}

For email to HTML conversion, we'll use [Aspose.Email for .NET][15]. The said API is designed to create, manipulate, convert, and send emails without installing MS Outlook or any other software. You can either [download][16] the API's DLL or install it within your .NET application using [NuGet][17].

```
PM> Install-Package Aspose.Email
```

## Convert Emails to HTML in C# {#Convert-MSG-EML-to-HTML-using-CSharp}

The following sections demonstrate how to convert emails to HTML or MHTML formats.

### Convert MSG or EML to HTML using C# {#Convert-MSG-EML-to-HTML-using-CSharp}

The following are the steps to convert an MSG or EML email file to HTML using Aspose.Email for .NET.

*   Load the EML or MSG email file using [MailMessage][18] class.
*   Convert email to HTML using [MailMessage.Save(String, SaveOptions.DefaultHtml)][19] method.

The following code sample shows how to convert an MSG/EML email to HTML using C#.

{{< gist aspose-com-gists 3588603072eedc144ef45b28741db2df "email-to-html.cs" >}}

### Convert MSG or EML to MHTML using C# {#Convert-MSG-EML-to-MHTML-using-CSharp}

MHTML is a web page archive format that is used to encapsulate the HTML content along with the external resources. In order to perform an email to MHTML conversion, you only need to provide [SaveOptions.DefaultMhtml][20] as a second parameter to _MailMessage.Save()_ method. The following are the steps to perform this operation.

*   Load the EML or MSG email file using [MailMessage][21] class.
*   Convert email to MHTML using [MailMessage.Save(String, SaveOptions.DefaultMhtml)][22] method.

The following code sample shows how to convert an MSG or EML file to MHTML using C#.

{{< gist aspose-com-gists 3588603072eedc144ef45b28741db2df "email-to-mhtml.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try Aspose.Email for .NET without evaluation limitations for free. [Get a free temporary license][23] now.

## Live Demo

*   [EML to HTML Converter][24]
*   [MSG to HTML Converter][25]

## Conclusion

In this article, you have learned how to convert emails to HTML or MHTML formats using C#. The steps along with API references and code samples have shown how to perform MSG/EML to HTML/MHTML conversion. You can explore more about the C# email API using [documentation][26].

## See Also

*   [Create Outlook Messages and Send Emails using C#][27]




[1]: https://docs.fileformat.com/email/msg/
[2]: https://docs.fileformat.com/email/eml/
[3]: https://docs.fileformat.com/web/html/
[4]: https://docs.fileformat.com/web/mhtml/
[5]: https://docs.fileformat.com/web/html/
[6]: https://docs.fileformat.com/email/msg/
[7]: https://docs.fileformat.com/email/eml/
[8]: https://docs.fileformat.com/web/html/
[9]: https://docs.fileformat.com/web/mhtml/
[10]: https://docs.fileformat.com/programming/cs/
[11]: #CSharp-Email-to-HTML-Converter-API
[12]: #Convert-MSG-EML-to-HTML-using-CSharp
[13]: #Convert-MSG-EML-to-MHTML-using-CSharp
[14]: #Get-a-Free-API-License
[15]: https://products.aspose.com/email/net
[16]: https://downloads.aspose.com/email/net
[17]: http://nuget.org/packages/Aspose.Email
[18]: https://apireference.aspose.com/email/net/aspose.email/mailmessage
[19]: https://apireference.aspose.com/email/net/aspose.email.mailmessage/save/methods/3
[20]: https://apireference.aspose.com/email/net/aspose.email/saveoptions/properties/defaultmhtml
[21]: https://apireference.aspose.com/email/net/aspose.email/mailmessage
[22]: https://apireference.aspose.com/email/net/aspose.email.mailmessage/save/methods/3
[23]: https://purchase.aspose.com/temporary-license
[24]: https://products.aspose.app/email/conversion/eml-to-html
[25]: https://products.aspose.app/email/conversion/msg-to-html
[26]: https://docs.aspose.com/email/net/developer-guide/
[27]: https://blog.aspose.com/2020/01/23/create-send-outlook-email-eml-msg-csharp-net-core/





