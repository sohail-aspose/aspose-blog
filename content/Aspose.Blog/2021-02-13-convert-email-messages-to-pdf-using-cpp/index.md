---
title: 'Convert Email Messages to PDF using C++'
seoTitle: "Convert Email Messages to PDF using C++ | MSG to PDF | EML to PDF"
description: "Convert Email messages to PDF using C++. Use Aspose.Email for C++ and Aspose.Words for C++ APIs to convert MSG and EML files to PDF format."
date: Sat, 13 Feb 2021 15:53:30 +0000
draft: false
url: /2021/02/13/convert-email-messages-to-pdf-using-cpp/
author: Muhammad Ahmad
summary: "Emails are the primary source of communication over the internet, especially in business environments. There might be cases such as discussing and finalizing the client's software requirements for product development. After completing the software requirements, you might need to generate a final set of documents containing the emails and other details to share with your team. In such scenarios, converting the email to [PDF][1] may prove to be helpful. In this article, you will learn **how to convert an email message to PDF format using C++**."
tags: ['Convert Email to PDF', 'Convert Email to PDF CPP', 'EML to PDF CPP', 'MSG to PDF CPP']
categories: ['Aspose.Words Product Family', 'Aspose.Email Product Family']
---



{{< figure align=center src="images/Convert-Email-to-PDF-1024x361.png" alt="Convert Email to PDF C++">}}


Emails are the primary source of communication over the internet, especially in business environments. There might be cases such as discussing and finalizing the client's software requirements for product development. After completing the software requirements, you might need to generate a final set of documents containing the emails and other details to share with your team. In such scenarios, converting the email to [PDF][2] may prove to be helpful. In this article, you will learn **how to convert an email message to PDF format using [C++][3]**.

*   [C++ Email to PDF Conversion API][4]
*   [Converting Email Messages to PDF using C++][5]
*   [Get a Free License][6]

## C++ Email to PDF Conversion API {#CPP-Email-to-PDF-Conversion-API}

To convert email to PDF, we will use [Aspose.Email for C++][7] and [Aspose.Words for C++][8] APIs. The former is a native C++ library for creating, manipulating, and converting Outlook files. Whereas, the latter allows you to generate, modify and convert Microsoft Word files. Furthermore, it also supports converting files to PDF format. We will use Aspose.Email for C++ for loading email files and Aspose.Words for C++ for their conversion to PDF format. You can either install the API through NuGet or download it directly from the [Downloads][9] section.

```
PM> Install-Package Aspose.Email.Cpp
PM> Install-Package Aspose.Words.Cpp
```

## Converting Email Messages to PDF using C++ {#Converting-Email-Messages-to-PDF-using-CPP}

The following are the steps to convert email files to PDF format using C++.

*   Load the email file using the [MailMessage][10] class.
*   Save the email message in the MemoryStream as [MHTML][11].
*   Create an instance of the [LoadOptions][12] class.
*   Set the load format as MHTML.
*   Load the file from the MemoryStream using the [](https://apireference.aspose.com/words/cpp/class/aspose.words.document#a1910ba5d8b5294351182b4d6dc6eea62)[Document(SharedPtr<Stream> stream, SharedPtr<LoadOptions> loadOptions)][13] constructor of the [Document][14] class.
*   Save the email as a PDF file using the [Document->Save(String fileName, SaveFormat saveFormat)][15] method.

The following code sample shows how to convert email messages to PDF format.

{{< gist aspose-com-gists 7496eada13a2a2eb4fff1d2e146dd91e "Convert-Email-to-PDF.cpp" >}}

## Get a Free License {#Get-a-Free-License}

You can try the API without evaluation limitations by requesting [a free temporary license][16].

## Live Demo

*   [EML to PDF Converter][17]
*   [MSG to PDF Converter][18]

## Conclusion

In this article, you have learned how to convert email messages to PDF format using C++. For this, we have used Aspose.Email for C++ for loading the email and Aspose.Words for C++ for converting it to PDF. Both of these APIs provide numerous features for working with email and MS Word files. To explore these APIs in detail, you can visit their official documentation.

*   [Aspose.Email for C++ Documentation][19]
*   [Aspose.Words for C++ Documentation][20]

## See Also

*   [Create Outlook Emails (MSG, EML, EMLX) using C++][21]
*   [Create MS Word Documents (DOC/DOCX) using C++][22]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: https://docs.fileformat.com/programming/cpp/
[4]: #CPP-Email-to-PDF-Conversion-API
[5]: #Converting-Email-Messages-to-PDF-using-CPP
[6]: #Get-a-Free-License
[7]: https://products.aspose.com/email/cpp
[8]: https://products.aspose.com/words/cpp
[9]: https://downloads.aspose.com/total
[10]: https://apireference.aspose.com/email/cpp/class/aspose.email.mail_message
[11]: https://docs.fileformat.com/web/mhtml/
[12]: https://apireference.aspose.com/words/cpp/class/aspose.words.loading.load_options
[13]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a1910ba5d8b5294351182b4d6dc6eea62
[14]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[15]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a1355bc15bd6da23c7bf65f3fcf0fb050
[16]: https://purchase.aspose.com/temporary-license
[17]: https://products.aspose.app/email/conversion/eml-to-pdf
[18]: https://products.aspose.app/email/conversion/msg-to-pdf
[19]: https://docs.aspose.com/email/cpp/
[20]: https://docs.aspose.com/words/cpp/
[21]: https://blog.aspose.com/2020/08/07/create-outlook-email-msg-eml-emlx-using-cpp/
[22]: https://blog.aspose.com/2020/08/25/create-ms-word-documents-using-cpp/





