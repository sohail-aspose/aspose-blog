---
title: 'Send Excel Data in Email Body using C# .NET'
seoTitle: "Send Excel Data in Email Body using C# .NET | .NET Email API"
description: "Use .NET email API to send Excel data in email's body programmatically in C#. Import data from Excel workbook into email's body from within .NET applications."
date: Wed, 11 May 2022 16:59:50 +0000
draft: false
url: /2022/05/11/send-excel-data-in-email-body-using-csharp-net/
author: Usman Aziz
summary: "Excel files are widely used to keep and share data in the form of rows and columns. In addition, you can perform various operations on the Excel data and visually analyze it. In some instances, you have to embed and send the data from an Excel sheet in the email message. To accomplish that, this article covers **how to send Excel data in an email's body programmatically in C# .NET**."
tags: ['DotNeT APIs to Send Excel Data in Email Body', 'DotNet Email API', 'Embed and Send Excel Data in Email Body in Csharp']
categories: ['Aspose.Cells Product Family', 'Aspose.Email Product Family']
---



{{< figure align=center src="images/Send-Excel-Data-in-Email-Body.png" alt="Send Excel Data in Email Body using C# .NET">}}


Excel files are widely used to keep and share data in the form of rows and columns. In addition, you can perform various operations on the Excel data and visually analyze it. In some instances, you have to embed and send the data from an Excel sheet in the email message. To accomplish that, this article covers **how to send Excel data in an email's body programmatically in C# .NET**.

*   [.NET APIs to Send Excel Data in Email Body][1]
*   [Embed and Send Excel Data in Email Body][2]

## C# .NET APIs to Send Excel Data in Email Body {#APIs-to-Send-Excel-Data-in-Email-Body}

To send the Excel data in email messages, we will use [Aspose.Email for .NET][3]. It is a popular and feature-rich API that lets you create and send emails from within your .NET applications. In addition, we will use [Aspose.Cells for .NET][4] to convert the Excel sheets into HTML content. You can either [download][5] the APIs' DLLs or install them from NuGet using the following commands.

```
PM> Install-Package Aspose.Email
PM> Install-Package Aspose.Cells
```

## Send Excel Data in Email's Body in C# {#Embed-and-Send-Excel-Data-in-Email-Body}

First, we will use Aspose.Cells for .NET to convert the Excel data into HTML so that it can be embedded into the email's body. After that, we will use Aspose.Email for .NET to compose the email, insert Excel data into the email's body, and send email. The following are the steps to send Excel data in an email's body in C#.

*   Load Excel workbook using Aspose.Cells’ [Workbook][6] class.
*   Save the workbook to [MemoryStream][7] in HTML format.
*   Read the HTML from the stream into a string object.
*   Create a new [MailMessage][8] object and set its _HtmlBody_ to the HTML content.
*   Create and configure the instance of [SmtpClient][9] class.
*   Send the email using [SmtpClient.Send(MailMessage)][10] method.

The following code sample shows how to send Excel data in an email's body in C#.

{{< gist aspose-com-gists e60b900feab31255be239912e7f54b4f "send-excel-data-in-email.cs" >}}

## Get a Free API License

You can use Aspose.Email for .NET without evaluation limitations using a [free temporary license][11].

## Conclusion

In this article, you have learned how to embed and send Excel data in an email's body using C# .NET. You can simply install the mentioned APIs and integrate the provided code into your .NET applications. Besides, you can explore more about the APIs using their documentation given below.

*   [Aspose.Cells for .NET][12]
*   [Aspose.Email for .NET][13]

In case you would have any questions, you can post to our [forum][14].

## See Also

*   [Create and Send Emails using C#][15]
*   [Read Emails from MS Exchange Server using C#][16]




[1]: #APIs-to-Send-Excel-Data-in-Email-Body
[2]: #Embed-and-Send-Excel-Data-in-Email-Body
[3]: https://products.aspose.com/email/net/
[4]: https://products.aspose.com/cells/net/
[5]: https://downloads.aspose.com/
[6]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[7]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream
[8]: https://apireference.aspose.com/email/net/aspose.email/mailmessage
[9]: https://apireference.aspose.com/email/net/aspose.email.clients.smtp/smtpclient
[10]: https://apireference.aspose.com/email/net/aspose.email.clients.smtp.smtpclient/send/methods/5
[11]: https://products.aspose.com/email
[12]: https://docs.aspose.com/cells/net
[13]: https://docs.aspose.com/email/net
[14]: https://forum.aspose.com/
[15]: https://blog.aspose.com/2020/01/23/create-send-outlook-email-eml-msg-csharp-net-core/
[16]: https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/




