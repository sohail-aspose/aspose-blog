---
title: 'Send Word Document in Email Body using C++'
seoTitle: "Send Word Document in Email Body using C++ | Send DOCX as Email"
description: "Send Word documents as the body of an email using C++. Import the content from Word documents and send it via email within your C++ applications."
date: Fri, 04 Jun 2021 18:42:48 +0000
draft: false
url: /2021/06/04/send-word-document-in-email-body-using-cpp/
author: Muhammad Ahmad
summary: 'Emails are the primary source of communication over the internet, and in the majority of cases, the layout and formatting of the emails is important. However, the majority of the email clients do not provide the enhanced formatting options required for designing high-quality email content. In such cases, a well-formatted Word document can be used in the body of the email. In this article, you will learn **how to send a Word document as the body of the email using C++**.'
tags: ['Send Word Document as Email using C++', 'Send Word Document in Email Body using C++']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Send-Word-Document-in-Email.jpg" alt="Send Word Document in Email Body using C++">}}


Emails are the primary source of communication over the internet and in the majority of cases, the layout and formatting of the email is important. However, most of the email clients do not provide the enhanced formatting options required for designing high-quality email content. In such cases, a well-formatted Word document can be used as the body of the email. In this article, you will learn **how to send a Word document as the body of the email using C++**.

*   [C++ APIs for Sending Word Documents In Email Body][1]
*   [Sending a Word Document in an Email Body using C++][2]

## C++ APIs for Sending Word Documents In Email Body {#CPP-APIs-for-Sending-Word-Documents-In-Email-Body}

In order to send a Word document in an email body, we will use the [Aspose.Words for C++][3] and [Aspose.Email for C++][4] APIs. The former allows you to generate, modify and convert Microsoft Word files. Whereas the latter allows you to create, manipulate, and convert Outlook files. We will use Aspose.Words for C++ API to convert the Word document to [MHTML][5] format and Aspose.Email for C++ API to generate and send the email. You can either install the APIs through NuGet or download them directly from the [Downloads][6] section.

```
PM> Install-Package Aspose.Words.Cpp
PM> Install-Package Aspose.Email.Cpp
```

## Sending a Word Document in an Email Body using C++ {#Sending-a-Word-Document-in-an-Email-Body-using-Cpp}

The following are the steps to send a Word document in an email body:

*   Load the Word document using the [Aspose::Words::Document][7] class.
*   Create an instance of the [MemoryStream][8] class.
*   Save the Word document to the [MemoryStream][9] in MHTML format.
*   Create an instance of the [Aspose::Email::MailMessage][10] class using the MHTML saved in the [MemoryStream][11].
*   Set To, From, and Subject of the email.
*   Create an instance of the [Aspose::Email::Clients::Smtp::SmtpClient][12] class.
*   Set the Host, Username, Password, Port, and Security Options.
*   Send the email message using the [SmtpClient->Send(System::SharedPtr<MailMessage> message)][13] method.

The following sample code shows how to send a Word document as the body of an email using C++.

{{< gist aspose-com-gists 2d7aa51be98b9bffef2c2cf0a4333e5a "Send-Word-Document-In-Email-Body.cpp" >}}

## Get a Free License

You can try the API without evaluation limitations by requesting [a free temporary license][14].

## Conclusion

In this article, you have learned how to send a Word document in an email body using C++. To summarize, you learned how to convert a Word document to MHTML format using Aspose.Words for C++ API and how to send MHTML as an email using Aspose.Email for C++ API. Both of these APIs provide numerous features for working with MS Word and email files. You can explore these APIs in detail by visiting their official documentation. In case of any questions, please feel free to reach us on our [free support forum][15].

*   [Aspose.Words for C++ Documentation][16]
*   [Aspose.Email for C++ Documentation][17]

## See Also

*   [Convert Email Messages to PDF using C++][18]
*   [Convert RTF Documents to PDF using C++][19]




[1]: #CPP-APIs-for-Sending-Word-Documents-In-Email-Body
[2]: #Sending-a-Word-Document-in-an-Email-Body-using-Cpp
[3]: https://products.aspose.com/words/cpp
[4]: https://products.aspose.com/email/cpp
[5]: https://docs.fileformat.com/web/mhtml/
[6]: https://downloads.aspose.com/total
[7]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[8]: https://apireference.codeporting.com/native/cs2cpp/class/system.i_o.memory_stream
[9]: https://apireference.codeporting.com/native/cs2cpp/class/system.i_o.memory_stream
[10]: https://apireference.aspose.com/email/cpp/class/aspose.email.mail_message
[11]: https://apireference.codeporting.com/native/cs2cpp/class/system.i_o.memory_stream
[12]: https://apireference.aspose.com/email/cpp/class/aspose.email.clients.smtp.smtp_client
[13]: https://apireference.aspose.com/email/cpp/class/aspose.email.clients.smtp.smtp_client#a8d28444f2c1c35fe0e4c1f6ec6b6c086
[14]: https://purchase.aspose.com/temporary-license
[15]: https://forum.aspose.com/
[16]: https://docs.aspose.com/words/cpp/
[17]: https://docs.aspose.com/email/cpp/
[18]: https://blog.aspose.com/2021/02/13/convert-email-messages-to-pdf-using-cpp/
[19]: https://blog.aspose.com/2021/02/17/convert-rtf-documents-to-pdf-using-cpp/





