---
title: 'Convert EML and MSG Emails to PDF in Java'
seoTitle: "Convert EML or MSG to PDF in Java | Java Email to PDF Converter API"
description: "Convert EML and MSG emails to PDF format in Java. Embed email to PDF conversion features into your Java applications. Download source code."
date: Tue, 22 Mar 2022 14:28:32 +0000
draft: false
url: /2022/03/22/convert-eml-msg-emails-to-pdf-in-java/
author: Usman Aziz
summary: '[EML][1] and [MSG][2] are popular email formats used by MS Outlook to store emails. There could be the cases when you need to share the content of EML or MSG files from within your web or desktop applications. One of the most suitable solutions is the conversion of email files to PDF format. In this article, you will learn **how to convert an EML or MSG email to PDF programmatically in Java.**'
tags: ['EML to PDF in Java', 'Java APIs for Email to PDF Conversion', 'MSG to PDF in java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Convert-Email-to-PDF-1024x361.png" alt="Convert EML and MSG Emails to PDF in Java">}}


[EML][3] and [MSG][4] are popular email formats used by MS Outlook to store emails. There could be the cases when you need to share the content of EML or MSG files from within your web or desktop applications. One of the most suitable solutions is the conversion of email files to PDF format. In this article, you will learn **how to convert an EML or MSG email to PDF programmatically in Java.**

*   [Java APIs for Email to PDF Conversion][5]
*   [Convert EML to PDF using Java][6]
*   [Get Free License][7]

## Java EML and MSG to PDF Converter APIs {#Java-Email-to-PDF-Conversion-API}

To convert email files to PDF, we will use the combination of [Aspose.Email for Java][8] and [Aspose.Words for Java][9]. The former is an email API that provides a bunch of features to create email client applications. Whereas, the latter one is a word processing API for creating and manipulating Word documents. You can use the following Maven configurations to install the API in your Java applications.

```
**Repository:**
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>

**Dependencies:**
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-email</artifactId>
    <version>22.2</version>
    <classifier>jdk16</classifier>
</dependency>
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-words</artifactId>
    <version>22.3</version>
    <type>pom</type>
</dependency>
```

Also, you can download the JARs of the APIs from the following links.

*   [Aspose.Email for Java][10]
*   [Aspose.Words for Java][11]

## Convert an EML or MSG File to PDF in Java {#Steps-to-Convert-Emails-to-PDF}

The following are the steps to convert an EML or MSG email to PDF format in Java.

*   Load the email file using [MailMessage][12] class.
*   Save the email message into a [ByteArrayOutputStream][13] object as default MHTML format.
*   Create an instance of [LoadOptions][14] class and set the load format as MHTML.
*   Instantiate [Document][15] class and pass **ByteArrayOutputStream** and **LoadOptions** objects as parameters to its constructor.
*   Convert the email to PDF using [Document.save(String, SaveFormat.PDF)][16] method.

The following is the complete code to convert an email message to PDF in Java.

{{< gist aspose-com-gists 2674b8e024882ef9d55818b35bda2e7e "email-to-pdf.java" >}}

## Get a Free License {#Get-Free-License}

You can [get a free temporary license][17] in order to try the APIs without evaluation limitations.

## Live Demo

*   [EML to PDF Converter][18]
*   [MSG to PDF Converter][19]

## Conclusion

In this article, you have learned how to convert EML or MSG email messages to PDF in Java. We have demonstrated how to use the combination of Aspose.Email and Aspose.Words to implement email to PDF conversion from within Java applications. You can also explore the below-mentioned documentations of both of the APIs. Also, you can post your queries to our [forum][20].

*   [Aspose.Email for Java][21]
*   [Aspose.Words for Java][22]

## See Also

*   [Read Emails from MS Exchange Server using Java][23]
*   [Create and Send Outlook Email Messages using Java][24]




[1]: https://docs.fileformat.com/email/eml/
[2]: https://docs.fileformat.com/email/msg/
[3]: https://docs.fileformat.com/email/eml/
[4]: https://docs.fileformat.com/email/msg/
[5]: #Java-Email-to-PDF-Conversion-API
[6]: #Steps-to-Convert-Emails-to-PDF
[7]: #Get-Free-License
[8]: https://products.aspose.com/email/java
[9]: https://products.aspose.com/words/java
[10]: https://downloads.aspose.com/email/java
[11]: https://downloads.aspose.com/words/java
[12]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage
[13]: https://docs.oracle.com/javase/7/docs/api/java/io/ByteArrayOutputStream.html
[14]: https://apireference.aspose.com/words/java/com.aspose.words/LoadOptions
[15]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[16]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String,int)
[17]: https://purchase.aspose.com/temporary-license
[18]: https://products.aspose.app/email/conversion/eml-to-pdf
[19]: https://products.aspose.app/email/conversion/msg-to-pdf
[20]: https://forum.aspose.com/
[21]: https://docs.aspose.com/email/java
[22]: https://docs.aspose.com/words/java
[23]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/
[24]: https://blog.aspose.com/2020/05/20/create-and-send-outlook-email-messages-asynchronously-using-java/




