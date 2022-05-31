---
title: 'Send Excel Data in Email Body using C# .NET'
date: Wed, 11 May 2022 16:59:50 +0000
draft: false
url: /2022/05/11/send-excel-data-in-email-body-using-csharp-net/
author: 'Usman Aziz'
summary: "Excel files are widely used to keep and share data in the form of rows and columns. In addition, you can perform various operations on the Excel data and visually analyze it. In some instances, you have to embed and send the data from an Excel sheet in the email message. To accomplish that, this article covers **how to send Excel data in an email's body programmatically in C# .NET**."
tags: ['DotNeT APIs to Send Excel Data in Email Body', 'DotNet Email API', 'Embed and Send Excel Data in Email Body in Csharp']
categories: ['Aspose.Cells Product Family', 'Aspose.Email Product Family']
---



{{< figure align=center src="images/Send-Excel-Data-in-Email-Body.png" alt="Send Excel Data in Email Body using C# .NET">}}


Excel files are widely used to keep and share data in the form of rows and columns. In addition, you can perform various operations on the Excel data and visually analyze it. In some instances, you have to embed and send the data from an Excel sheet in the email message. To accomplish that, this article covers **how to send Excel data in an email's body programmatically in C# .NET**.

*   [.NET APIs to Send Excel Data in Email Body](#APIs-to-Send-Excel-Data-in-Email-Body)
*   [Embed and Send Excel Data in Email Body](#Embed-and-Send-Excel-Data-in-Email-Body)

## C# .NET APIs to Send Excel Data in Email Body {#APIs-to-Send-Excel-Data-in-Email-Body}

To send the Excel data in email messages, we will use [Aspose.Email for .NET](https://products.aspose.com/email/net/). It is a popular and feature-rich API that lets you create and send emails from within your .NET applications. In addition, we will use [Aspose.Cells for .NET](https://products.aspose.com/cells/net/) to convert the Excel sheets into HTML content. You can either [download](https://downloads.aspose.com/) the APIs' DLLs or install them from NuGet using the following commands.

```
PM> Install-Package Aspose.Email
PM> Install-Package Aspose.Cells
```

## Send Excel Data in Email's Body in C# {#Embed-and-Send-Excel-Data-in-Email-Body}

First, we will use Aspose.Cells for .NET to convert the Excel data into HTML so that it can be embedded into the email's body. After that, we will use Aspose.Email for .NET to compose the email, insert Excel data into the email's body, and send email. The following are the steps to send Excel data in an email's body in C#.

*   Load Excel workbook using Aspose.Cells’ [Workbook](https://apireference.aspose.com/cells/net/aspose.cells/workbook) class.
*   Save the workbook to [MemoryStream](https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream) in HTML format.
*   Read the HTML from the stream into a string object.
*   Create a new [MailMessage](https://apireference.aspose.com/email/net/aspose.email/mailmessage) object and set its _HtmlBody_ to the HTML content.
*   Create and configure the instance of [SmtpClient](https://apireference.aspose.com/email/net/aspose.email.clients.smtp/smtpclient) class.
*   Send the email using [SmtpClient.Send(MailMessage)](https://apireference.aspose.com/email/net/aspose.email.clients.smtp.smtpclient/send/methods/5) method.

The following code sample shows how to send Excel data in an email's body in C#.

{{< gist aspose-com-gists e60b900feab31255be239912e7f54b4f "send-excel-data-in-email.cs" >}}

## Get a Free API License

You can use Aspose.Email for .NET without evaluation limitations using a [free temporary license](https://products.aspose.com/email).

## Conclusion

In this article, you have learned how to embed and send Excel data in an email's body using C# .NET. You can simply install the mentioned APIs and integrate the provided code into your .NET applications. Besides, you can explore more about the APIs using their documentation given below.

*   [Aspose.Cells for .NET](https://docs.aspose.com/cells/net)
*   [Aspose.Email for .NET](https://docs.aspose.com/email/net)

In case you would have any questions, you can post to our [forum](https://forum.aspose.com/).

## See Also

*   [Create and Send Emails using C#](https://blog.aspose.com/2020/01/23/create-send-outlook-email-eml-msg-csharp-net-core/)
*   [Read Emails from MS Exchange Server using C#](https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/)




