---
title: 'Convert EML and MSG Emails to PDF using C#'
seoTitle: "Convert EML or MSG Emails to PDF in C# | C# MSG to PDF, EML to PDF"
description: "Convert Email messages to PDF using C#. Convert MSG and EML emails to PDF format with high fidelity within a few lines of C# code. Complete tutorial."
date: Thu, 07 Jan 2021 11:17:00 +0000
draft: false
url: /2021/01/07/convert-emails-to-pdf-using-csharp/
author: Usman Aziz
summary: 'There could be various scenarios when you need to embed the content of the emails within your web or desktop applications. In such cases, you can convert the email messages into a format that can easily be embedded and displayed. One of the possible solutions is email to PDF conversion. This article provides a step by step guide and code sample of **how to convert an email message to PDF using C#**.'
tags: ['convert email to pdf csharp', 'eml to pdf csharp', 'msg to pdf csharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Convert-Email-to-PDF-1024x361.png" alt="Convert Email to PDF">}}


There could be various scenarios when you need to embed the content of the emails within your web or desktop applications. In such cases, you can convert the email messages into a format that can easily be embedded and displayed. One of the possible solutions is email to [PDF][1] conversion. This article provides a step-by-step guide and code sample of **how to convert an EML or MSG email to PDF using [C#][2]**.

*   [C# Email to PDF Conversion API][3]
*   [Steps to Convert Emails to PDF using C#][4]
*   [C# Email to PDF Conversion - Complete Code][5]
*   [Get Free License][6]

## C# EML and MSG Emails to PDF Converter API {#CSharp-Email-to-PDF-Conversion-API}

[Aspose.Email for .NET][7] is a C# class library that is designed to create and manipulate popular email formats from within the .NET applications. In combination with [Aspose.Words for .NET][8], the API lets you convert the email messages to PDF format with high fidelity. You can either download the APIs' DLLs or install them within your .NET applications using NuGet.

```
PM> Install-Package Aspose.Words
PM> Install-Package Aspose.Email
```

*   [Download Aspose.Email for .NET][9]
*   [Download Aspose.Words for .NET][10]

## Steps to Convert EML or MSG to PDF using C# {#Steps-to-Convert-Emails-to-PDF-using-CSharp}

The following are the steps to convert email messages to PDF format in C#.

*   Load the email file using [MailMessage][11] class.

{{< gist aspose-com-gists 2b4338c1d2915a7cd5cd01db14c965ba "load-email.cs" >}}

*   Save the email message into a [MemoryStream][12] object as default MHTML format.

{{< gist aspose-com-gists 2b4338c1d2915a7cd5cd01db14c965ba "save-email-to-memorystream.cs" >}}

*   Create an instance of [Aspose.Words.LoadOptions][13] class and set the load format as MHTML.

{{< gist aspose-com-gists 2b4338c1d2915a7cd5cd01db14c965ba "create-loadoptions.cs" >}}

*   Instantiate [Aspose.Words.Document][14] class and pass [MemoryStream][15] and [LoadOptions][16] objects as parameters to its constructor.

{{< gist aspose-com-gists 2b4338c1d2915a7cd5cd01db14c965ba "load-document-from-memory-stream.cs" >}}

*   Create an instance of [Aspose.Words.Saving.PdfSaveOptions][17] class.

{{< gist aspose-com-gists 2b4338c1d2915a7cd5cd01db14c965ba "create-pdfsaveoptions.cs" >}}

*   Convert the email to PDF using [Document.Save("email-to-pdf.pdf", PdfSaveOptions)][18] method.

{{< gist aspose-com-gists 2b4338c1d2915a7cd5cd01db14c965ba "save-email-as-pdf.cs" >}}

## C# Email to PDF Conversion - Complete Code {#CSharp-Email-to-PDF-Conversion}

The following is the complete code to convert an email message to PDF using Aspose.Emails for .NET and Aspose.Words for .NET APIs.

{{< gist aspose-com-gists 2b4338c1d2915a7cd5cd01db14c965ba "convert-email-to-pdf.cs" >}}

## Get a Free License {#Get-Free-License}

You can [get a free temporary license][19] in order to try the APIs without evaluation limitations.

## Live Demo

*   [EML to PDF Converter][20]
*   [MSG to PDF Converter][21]

## Conclusion

Email to PDF conversion may come into practice when you need to embed the email messages within your web or desktop applications. Therefore, in this article, you have learned how to convert email messages to PDF using C# within your .NET applications. In order to explore more about the APIs being used, you can visit the following documentations.

*   [Aspose.Email for .NET][22]
*   [Aspose.Words for .NET][23]

## See Also

*   [Read Emails from MS Exchange Server using C#][24]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/programming/cs/
[3]: #CSharp-Email-to-PDF-Conversion-API
[4]: #Steps-to-Convert-Emails-to-PDF-using-CSharp
[5]: #CSharp-Email-to-PDF-Conversion
[6]: #Get-Free-License
[7]: https://products.aspose.com/email/net
[8]: https://products.aspose.com/words/net
[9]: https://downloads.aspose.com/email/net
[10]: https://downloads.aspose.com/words/net
[11]: https://apireference.aspose.com/email/net/aspose.email/mailmessage
[12]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream?view=net-5.0
[13]: https://apireference.aspose.com/words/net/aspose.words.loading/loadoptions
[14]: https://apireference.aspose.com/words/net/aspose.words/document
[15]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream?view=net-5.0
[16]: https://apireference.aspose.com/words/net/aspose.words.loading/loadoptions
[17]: https://apireference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions
[18]: https://apireference.aspose.com/words/net/aspose.words.document/save/methods/4
[19]: https://purchase.aspose.com/temporary-license
[20]: https://products.aspose.app/email/conversion/eml-to-pdf
[21]: https://products.aspose.app/email/conversion/msg-to-pdf
[22]: https://docs.aspose.com/email/net/developer-guide/
[23]: https://docs.aspose.com/words/net/developer-guide/
[24]: https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/





