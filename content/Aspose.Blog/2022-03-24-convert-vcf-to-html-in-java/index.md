---
title: 'Convert VCF Files to HTML in Java'
seoTitle: "Convert VCF to HTML in Java | Java Email Library"
description: "Use Java email library to convert VCF files to HTML format programmatically in Java. Download the library for free and integrate VCF to HTML conversion."
date: Thu, 24 Mar 2022 07:01:39 +0000
draft: false
url: /2022/03/24/convert-vcf-to-html-in-java/
author: Usman Aziz
summary: '[VCF][1] is a commonly used format to store the contact information of single or multiple persons. Also, it can contain the contact information of the business. The fields of a VCF file include name, address, phone, email, etc. In certain cases, you may need to convert a VCF file to HTML, for example, to embed it into a web page. To accomplish that programmatically, this article shows **how to convert a VCF file to HTML in Java**.'
tags: ['Java Email Library', 'convert vcf files to html in java', 'vcf to html in java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/VCF-to-HTML.png" alt="Convert VCF Files to HTML in Java">}}


[VCF][2] is a commonly used format to store the contact information of single or multiple persons. Also, it can contain the contact information of the business. The fields of a VCF file include name, address, phone, email, etc. In certain cases, you may need to convert a VCF file to HTML, for example, to embed it into a web page. To accomplish that programmatically, this article shows **how to convert a VCF file to HTML in Java**.

*   [Java API for VCF to HTML Conversion][3]
*   [Convert a VCF File to HTML][4]

## Java API for VCF to HTML Conversion {#Java-API-for-VCF-to-HTML-Conversion}

To export VCF files as HTML, we will use [Aspose.Email for Java][5]. It is a popular and powerful library to implement email client applications in Java. Also, it allows you to manipulate and convert various email and contact formats. You can either [download][6] the JAR or use the following Maven configurations to install the library.

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
    <version>22.2</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Convert a VCF File to HTML in Java {#Convert-a-VCF-File-to-HTML-in-Java}

The following are the steps to convert a VCF file to HTML in Java.

*   Load VCF file using [MailMessage][7] class.
*   Save VCF as HTML using [MailMessage.save(String, SaveOptions.getDefaultHtml())][8] method.

The following code sample shows how to convert a VCF file to HTML format.

{{< gist aspose-com-gists e47a111651462d4924c32b7c2ebe79c8 "vcf-to-html.java" >}}

## Get a Free License {#Get-Free-License}

You can [get a free temporary license][9] in order to use Aspose.Email for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to convert VCF files to HTML format in Java. You can simply install Aspose.Email and integrate VCF to HTML conversion in your applications. In addition, you can explore the [documentation][10] of the API. Also, you can post your queries to our [forum][11].

## See Also

*   [Read Emails from MS Exchange Server using Java][12]
*   [Create and Send Outlook Email Messages using Java][13]




[1]: https://docs.fileformat.com/email/vcf/
[2]: https://docs.fileformat.com/email/vcf/
[3]: #Java-API-for-VCF-to-HTML-Conversion
[4]: #Convert-a-VCF-File-to-HTML-in-Java
[5]: https://products.aspose.com/email/java
[6]: https://downloads.aspose.com/email/java/
[7]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage
[8]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage#save(java.lang.String,%20com.aspose.email.SaveOptions)
[9]: https://purchase.aspose.com/temporary-license
[10]: https://docs.aspose.com/email/java
[11]: https://forum.aspose.com/
[12]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/
[13]: https://blog.aspose.com/2020/05/20/create-and-send-outlook-email-messages-asynchronously-using-java/




