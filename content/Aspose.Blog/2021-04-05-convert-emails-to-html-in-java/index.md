---
title: 'Convert Emails to HTML in Java'
seoTitle: "Convert Email to HTML in Java | Java EML to HTML or MSG to HTML"
description: "Convert email files to HTML programmatically using Java. Convert EML or EMLX files to HTML or MSG email messages to HTML using Java Email API."
date: Mon, 05 Apr 2021 11:10:00 +0000
draft: false
url: /2021/04/05/convert-emails-to-html-in-java/
author: Usman Aziz
summary: '[MSG][1] and [EML][2] are popular file formats to store email messages. However, you can not display the content of both of the email formats directly in your web applications. In order to embed MSG or EML emails within your web pages, you can convert them to HTML. In this article, you will learn **how to convert MSG and EML/EMLX emails to HTML in Java**.'
tags: ['Convert EML Emails to HTML in Java', 'Convert MSG Emails to HTML in Java', 'Java Email to HTML Conversion API']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Email-to-HTML.jpg" alt="email to HTML java">}}


[MSG][3] and [EML][4] are popular file formats to store email messages. However, you can not display the content of both of the email formats directly in your web applications. In order to embed MSG or EML emails within your web pages, you can convert them to [HTML][5]. In this article, you will learn **how to convert MSG and EML/EMLX emails to HTML in Java**.

*   [Java Email to HTML Conversion API][6]
*   [Convert EML Emails to HTML in Java][7]
*   [Convert MSG Emails to HTML in Java][8]
*   [Get a Free API License][9]

## Java Email to HTML Conversion API {#Java-Email-to-HTML-Conversion-API}

[Aspose.Email for Java][10] is an email manipulation API that lets you implement feature-rich email client applications. In addition, it allows you to convert EML and MSG email messages to other formats such as HTML. In order to use the API, you can either [download][11] its JAR or get it installed using the following Maven configurations.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-email</artifactId>
    <version>21.3</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Convert Emails to HTML in Java

Since EML and MSG are the most commonly used email formats, therefore, we'll demonstrate conversion of both formats.

### Convert EML to HTML in Java {#Convert-EML-Emails-to-HTML-in-Java}

The following are the steps to convert EML or EMLX files to HTML using Java.

*   Load the EML/EMLX email using [MailMessage][12] class.
*   Convert email to HTML using [MailMessage.save(String, SaveOptions.getDefaultHtml())][13] method.

The following code sample shows how to convert EML or EMLX emails to HTML using Java.

{{< gist aspose-com-gists cd40b60f91f72f0c65ab49f479e61884 "eml-to-html.java" >}}

### Convert MSG to HTML in Java {#Convert-MSG-Emails-to-HTML-in-Java}

The following are the steps to convert MSG emails to HTML using Java.

*   Load the MSG email using [MailMessage][14] class.
*   Convert MSG to HTML using [MailMessage.save(String, SaveOptions.getDefaultHtml())][15] method.

The following code sample shows how to convert MSG emails to HTML using Java.

{{< gist aspose-com-gists cd40b60f91f72f0c65ab49f479e61884 "msg-to-html.java" >}}

## Get a Free API Lincese {#Get-a-Free-API-License}

You can [request a free temporary license][16] in order to use the API without evaluation limitations.

## Conclusion

In this article, you have learned how to convert email files to HTML using Java. Particularly, the code samples have demonstrated how to convert MSG or EML/EMLX emails to HTML. You can explore other features of Aspose.Email for Java using [documentation][17]. In case you would have any queries, feel free to let us know via our [forum][18].

## Live Demo

*   [EML to HTML Converter][19]
*   [MBOX to HTML Converter][20]

## See Also

*   [Read Emails from MS Exchange Server using Java][21]




[1]: https://docs.fileformat.com/email/msg/
[2]: https://docs.fileformat.com/email/eml
[3]: https://docs.fileformat.com/email/msg/
[4]: https://docs.fileformat.com/email/eml
[5]: https://docs.fileformat.com/web/html/
[6]: #Java-Email-to-HTML-Conversion-API
[7]: #Convert-EML-Emails-to-HTML-in-Java
[8]: #Convert-MSG-Emails-to-HTML-in-Java
[9]: #Get-a-Free-API-License
[10]: https://products.aspose.com/email/java
[11]: https://downloads.aspose.com/email/java
[12]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage
[13]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage#save(java.lang.String,%20com.aspose.email.SaveOptions)
[14]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage
[15]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage#save(java.lang.String,%20com.aspose.email.SaveOptions)
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/email/java/
[18]: https://forum.aspose.com/
[19]: https://products.aspose.app/email/conversion/eml-to-html
[20]: https://products.aspose.app/email/conversion/mbox-to-html
[21]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/





