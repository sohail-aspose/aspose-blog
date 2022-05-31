---
title: 'Convert OFT Files to HTML in Java'
date: Tue, 12 Apr 2022 07:10:00 +0000
draft: false
url: /2022/04/12/convert-oft-files-to-html-in-java/
author: ''Usman Aziz''
summary: 'MS Outlook uses [OFT][1] as a template format to create layouts for the emails. The template can be preformatted and populated with the content dynamically for creating custom messages. In some instances, you may get the OFT files and need to convert them to HTML format programmatically. To achieve that, this article shows **how to convert an OFT file to HTML in Java**.'
tags: ['Convert an OFT File to HTML in Java', 'Java API for OFT to HTML Conversion', 'Java Email API', 'Java Email Converter API']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/OFT-to-HTML.png" alt="Convert OFT Files to HTML in Java">}}


MS Outlook uses [OFT][2] as a template format to create layouts for the emails. The template can be preformatted and populated with the content dynamically for creating custom messages. In some instances, you may get the OFT files and need to convert them to HTML format programmatically. To achieve that, this article shows **how to convert an OFT file to HTML in Java**.

*   [API for OFT to HTML Conversion][3]
*   [Convert an OFT File to HTML][4]

## Java API for OFT to HTML Conversion {#API-for-OFT-to-HTML-Conversion}

To convert OFT files, we will use [Aspose.Email for Java][5]. It is a powerful library for creating and sending emails and implementing email client applications. Furthermore, it allows you to manipulate and convert various email formats. You can either [download][6] the API or install it using the following Maven configurations.

```
**Repository:**
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>

**Dependency:**
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-email</artifactId>
    <version>22.4</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Convert an OFT File to HTML {#Convert-a-OFT-to-HTML}

The following are the steps to convert an OFT file to HTML programmatically.

*   Load OFT file using [MailMessage][7] class.
*   Convert OFT to HTML using [MailMessage.save(String, SaveOptions)][8] method.

The following code sample shows how to convert an OFT file to HTML format.

{{< gist aspose-com-gists a9cfb703afea6ae99893be49a82b54ed "oft-to-html.java" >}}

## Get a Free License {#Get-Free-License}

You can [get a free temporary license][9] in order to use Aspose.Email for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to convert OFT files to HTML in Java. You can simply install Aspose.Email and integrate OFT to HTML conversion in your applications. In addition, you can explore other features of Aspose.Email using the [documentation][10]. Also, you can post your queries to our [forum][11].

## See Also

*   [Read Emails from MS Exchange Server using Java][12]
*   [Create and Send Outlook Email Messages using Java][13]




[1]: https://docs.fileformat.com/email/oft/
[2]: https://docs.fileformat.com/email/oft/
[3]: #API-for-OFT-to-HTML-Conversion
[4]: #Convert-a-OFT-to-HTML
[5]: https://products.aspose.com/email/java/
[6]: https://downloads.aspose.com/email/java/
[7]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage
[8]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage#save(java.lang.String,%20com.aspose.email.SaveOptions)
[9]: https://purchase.aspose.com/temporary-license
[10]: https://docs.aspose.com/email/java/
[11]: https://forum.aspose.com/
[12]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/
[13]: https://blog.aspose.com/2020/05/20/create-and-send-outlook-email-messages-asynchronously-using-java/




