---
title: 'Convert MSG and EML Emails to HTML using C++'
seoTitle: "Convert MSG and EML Emails to HTML using C++ | Use custom timezone"
description: "Convert emails to HTML or MHTML formats using C++. Convert MSG or EML files to HTML or MHTML format withing your C++ applications."
date: Wed, 17 Mar 2021 13:54:04 +0000
draft: false
url: /2021/03/17/convert-emails-to-html-using-cpp/
author: Muhammad Ahmad
summary: 'In this day and age, emails are among the most common means of communication over the internet. As software developers, you see a wide variety of user requirements and usage scenarios. One such requirement might be that you want to embed the email content in web pages. For such cases, you would need to convert the emails into [HTML][1] format. In this article, you will learn **how to convert [MSG][2] and [EML][3] emails to HTML or [MHTML][4]** **format programmatically using C++**.'
tags: ['convert email to html using c++', 'convert eml to html using c++', 'convert msg to html using c++']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Email-to-HTML.jpg" alt="Convert Email to HTML using C++">}}


In this day and age, emails are among the most common means of communication over the internet. As software developers, you see a wide variety of user requirements and usage scenarios. One such requirement might be that you want to embed the email content in web pages. For such cases, you would need to convert the emails into [HTML][5] format. In this article, you will learn **how to convert [MSG][6] and [EML][7] emails to HTML or [MHTML][8]** **format programmatically using [C++][9]**.

*   [C++ API for Converting Emails to HTML][10]
*   [Convert Email to HTML using C++][11]
*   [Converting Email to MHTML using C++][12]
*   [Export Email to HTML with Header][13]
*   [Emails to HTML Conversion with custom Timezone][14]
*   [Get a Free License][15]

## C++ API for Converting Emails to HTML {#CPP-API-for-Converting-Emails-to-HTML}

[Aspose.Email for C++][16] is a native C++ library for creating, manipulating, and sending emails without requiring Microsoft Outlook to be installed. The API also provides the ability to convert emails to different formats, including HTML. You can either install the API through [NuGet][17] or download it directly from the [Downloads][18] section.

```
PM> Install-Package Aspose.Email.Cpp
```

## Convert Email to HTML using C++ {#Convert-Email-to-HTML-using-CPP}

Converting email files to HTML is a breeze with Aspose.Email for C++ API. In just two lines of code, you can convert an email file to HTML format. The following are the steps to convert an email file to HTML format using C++.

*   Load the email file using the [MailMessage][19] class.
*   Save the file as HTML using the [MailMessage->Save (System::String fileName, System::SharedPtr<SaveOptions> options)][20] method.

The following is the sample code to convert email files to HTML format.

{{< gist aspose-com-gists a6d453aad8224a82727fc8c578fa3088 "Convert-Email-To-HTML.cpp" >}}

## Converting Email to MHTML using C++ {#Converting-Email-to-MHTML-using-CPP}

Similar to converting an email to HTML, you can convert an email file to MHTML format by passing [Aspose::Email::SaveOptions::get\_DefaultMhtml()][21] as the second parameter of the [MailMessage->Save (System::String fileName, System::SharedPtr<SaveOptions> options)][22] method. The following are the steps to convert an email file to MHTML format.

*   Load the email file using the [MailMessage][23] class.
*   Save the file as MHTML using the [MailMessage->Save (System::String fileName, System::SharedPtr<SaveOptions> options)][24] method.

The following is the sample code to convert email files to MHTML format.

{{< gist aspose-com-gists a6d453aad8224a82727fc8c578fa3088 "Convert-Email-To-MHTML.cpp" >}}

## Export Email to HTML with Header {#Export-Email-to-HTML-with-Header}

By default, the generated HTML does not include the email header information. To export the header information, you can use the [HtmlSaveOptions][25] class. The following are the steps to convert email files to HTML format with the header information included in the resulting HTML.

*   Load the email file using the [MailMessage][26] class.
*   Create an instance of the [HtmlSaveOptions][27] class.
*   Set the format option to show header information using [SaveOption->set\_HtmlFormatOptions (Aspose::Email::HtmlFormatOptions value)][28] method.
*   Finally, save the file as HTML using the [MailMessage->Save (System::String fileName, System::SharedPtr<SaveOptions> options)][29] method.

The following is the sample code to convert emails to HTML with header information.

{{< gist aspose-com-gists a6d453aad8224a82727fc8c578fa3088 "Convert-Email-To-HTML-With-Header.cpp" >}}

## Email to HTML Conversion with custom Timezone {#Email-to-HTML-Conversion-with-custom-Timezone}

Aspose.Email for C++ provides you the ability to convert emails by specifying a custom timezone. The resulting HTML file will show the time in the selected timezone. The following are the steps to convert email files to HTML format with a custom timezone.

*   Load the email file using the [MailMessage][30] class.
*   Set the custom timezone using [MailMessage->set\_TimeZoneOffset(System::TimeSpan _value_)][31] method.
*   Create an instance of the [HtmlSaveOptions][32] class.
*   Set the format option to show header information using [SaveOption->set\_HtmlFormatOptions (Aspose::Email::HtmlFormatOptions value)][33] method.
*   Finally, save the file as HTML using the [MailMessage->Save (System::String fileName, System::SharedPtr<SaveOptions> options)][34] method.

The following is the sample code to convert email files to HTML format with a custom timezone using C++.

{{< gist aspose-com-gists a6d453aad8224a82727fc8c578fa3088 "Convert-Email-To-HTML-With-Custom-Timezone.cpp" >}}

## Get a Free License {#Get-a-Free-License}

You can try the API without evaluation limitations by requesting [a free temporary license][35].

## Live Demo

*   [EML to HTML Converter][36]
*   [MSG to HTML Converter][37]

## Conclusion

In this article, you have learned how to convert MSG and EML files to HTML and MHTML format using C++. You have also seen how to include header information in the generated HTML output. Furthermore, you have learned how to customize the timezone of the email. Aspose.Email for C++ provides many more features for working with email files. You can explore the API in detail by visiting the [official documentation][38]. If you have any questions, please feel free to reach us on our [free support forum][39].

## See Also

*   [Convert Email Messages to PDF using C++][40]




[1]: https://docs.fileformat.com/web/html/
[2]: https://docs.fileformat.com/email/msg/
[3]: https://docs.fileformat.com/email/eml/
[4]: https://docs.fileformat.com/web/mhtml/
[5]: https://docs.fileformat.com/web/html/
[6]: https://docs.fileformat.com/email/msg/
[7]: https://docs.fileformat.com/email/eml/
[8]: https://docs.fileformat.com/web/mhtml/
[9]: https://docs.fileformat.com/programming/cpp/
[10]: #CPP-API-for-Converting-Emails-to-HTML
[11]: #Convert-Email-to-HTML-using-CPP
[12]: #Converting-Email-to-MHTML-using-CPP
[13]: #Export-Email-to-HTML-with-Header
[14]: #Email-to-HTML-Conversion-with-custom-Timezone
[15]: #Get-a-Free-License
[16]: https://products.aspose.com/email/cpp
[17]: https://www.nuget.org/packages/Aspose.Email.Cpp
[18]: https://downloads.aspose.com/email/cpp
[19]: https://apireference.aspose.com/email/cpp/class/aspose.email.mail_message
[20]: https://apireference.aspose.com/email/cpp/class/aspose.email.mail_message#a7e7c6b50c8db5a8bcc6934db02b4a786
[21]: https://apireference.aspose.com/email/cpp/class/aspose.email.save_options#a11b2d0dda5ad0473180039c978038872
[22]: https://apireference.aspose.com/email/cpp/class/aspose.email.mail_message#a7e7c6b50c8db5a8bcc6934db02b4a786
[23]: https://apireference.aspose.com/email/cpp/class/aspose.email.mail_message
[24]: https://apireference.aspose.com/email/cpp/class/aspose.email.mail_message#a7e7c6b50c8db5a8bcc6934db02b4a786
[25]: https://apireference.aspose.com/email/cpp/class/aspose.email.html_save_options
[26]: https://apireference.aspose.com/email/cpp/class/aspose.email.mail_message
[27]: https://apireference.aspose.com/email/cpp/class/aspose.email.html_save_options
[28]: https://apireference.aspose.com/email/cpp/class/aspose.email.html_save_options#add66b6aa58f38d0d7e8f801784b8c59a
[29]: https://apireference.aspose.com/email/cpp/class/aspose.email.mail_message#a7e7c6b50c8db5a8bcc6934db02b4a786
[30]: https://apireference.aspose.com/email/cpp/class/aspose.email.mail_message
[31]: https://apireference.aspose.com/email/cpp/class/aspose.email.mail_message#a1a0d21796c28395e01fa9456c1f03195
[32]: https://apireference.aspose.com/email/cpp/class/aspose.email.html_save_options
[33]: https://apireference.aspose.com/email/cpp/class/aspose.email.html_save_options#add66b6aa58f38d0d7e8f801784b8c59a
[34]: https://apireference.aspose.com/email/cpp/class/aspose.email.mail_message#a7e7c6b50c8db5a8bcc6934db02b4a786
[35]: https://purchase.aspose.com/temporary-license
[36]: https://products.aspose.app/email/conversion/eml-to-html
[37]: https://products.aspose.app/email/conversion/msg-to-html
[38]: https://docs.aspose.com/email/cpp/
[39]: https://forum.aspose.com/c/email/12
[40]: https://blog.aspose.com/2021/02/13/convert-email-messages-to-pdf-using-cpp/





