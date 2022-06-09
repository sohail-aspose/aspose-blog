---
title: 'Send a Word Document as Email in Java'
seoTitle: "Send Word Document as Email in Java | Import Word Doc in Email Body"
description: "Use Java APIs to send MS Word document as email body using Java. Import content from Word document into email body within Java applications."
date: Mon, 26 Apr 2021 20:02:51 +0000
draft: false
url: /2021/04/26/send-a-word-document-as-email-in-java/
author: Usman Aziz
summary: 'In most cases, emails are sent in a well-formatted layout following a particular template. However, various email editors do not provide the enhanced formatting options. In such cases, you can create a message in a Word document and use it as an email body. In this article, you will learn **how to send an MS Word document as an email body using Java**.'
tags: ['Java APIs to Import Word Document to Email', 'Java Email API', 'Java Word API', 'Send Word Document in Email Body in Java']
categories: ['Aspose.Words Product Family', 'Aspose.Total Product Family', 'Aspose.Email Product Family']
---



{{< figure align=center src="images/Send-Word-Document-in-Email.jpg" alt="send word document as email in java">}}


In most cases, emails are sent in a well-formatted layout following a particular template. However, various email editors do not provide the enhanced formatting options. In such cases, you can create a message in a Word document and use it as an email body. In this article, you will learn **how to send an MS Word document as an email body using [Java][1]**.

*   [Java APIs to Import Word Document in Email][2]
*   [Send a Word Document in Email Body][3]
*   [Get a Free API License][4]

## Java APIs to Import Word Document in Email {#Java-APIs-to-Import-Word-Document-to-Email}

In order to import and send a Word document in an email body, we'll leverage the capabilities of [Aspose.Words for Java][5] and [Aspose.Email for Java][6] APIs. The former will be used to save the Word document in [MHTML][7] format, whereas, the latter will be used to create and send the email. You can download the APIs from the following sections or install them using the Maven configurations.

*   [Aspose.Words for Java][8]
*   [Aspose.Email for Java][9]

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-words</artifactId>
    <version>21.4</version>
    <type>pom</type>
</dependency>
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-email</artifactId>
    <version>21.3</version>
    <classifier>jdk16</classifier>
</dependency> 
```

## Send a Word Document in Email Body using Java {#Steps-to-Send-Word-Document-in-Email-Body-in-Java}

The following are the steps to import and send a Word document in an email body.

*   Load the Word document using [com.aspose.words.Document][10] class.
*   Create an instance of [ByteArrayOutputStream][11] class.
*   Save the Word document as MHTML in _ByteArrayOutputStream_ object.
*   Load the MHTML in a [ByteArrayInputStream][12] object.
*   Create an instance of [com.aspose.email.MailMessage][13] class and load the MHTML saved in the _ByteArrayInputStream_ object.
*   Set email's fields such as To, From, Subject, etc.
*   Create an instance of [com.aspose.email.SmtpClient][14] class
*   Set the host and send the email using [SmtpClient.send(MailMessage)][15] method.

The following code sample shows how to send a Word document as an email body.

{{< gist aspose-com-gists 29940e46a37422a80882208f20218ee1 "send-word-doc-as-email.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try the APIs used in this article without evaluation limitations by [getting a free temporary license][16].

## Conclusion

In this article, you have learned how to import and send a Word document as an email body using Java. Furthermore, the code sample has shown how to send the email composed of a Word document using an SMTP client. You can explore more about the APIs being used in the article by visiting the following documentations.

*   [Aspose.Words for Java][17]
*   [Aspose.Email for Java][18]

## See Also

*   [Read Email Messages Programmatically using Java][19]




[1]: https://docs.fileformat.com/programming/java/
[2]: #Java-APIs-to-Import-Word-Document-to-Email
[3]: #Steps-to-Send-Word-Document-in-Email-Body-in-Java
[4]: #Get-a-Free-API-License
[5]: https://products.aspose.com/words/java
[6]: https://products.aspose.com/email/java
[7]: https://docs.fileformat.com/web/mhtml/
[8]: https://downloads.aspose.com/words/java
[9]: https://downloads.aspose.com/email/java
[10]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[11]: https://docs.oracle.com/javase/7/docs/api/java/io/ByteArrayOutputStream.html
[12]: https://docs.oracle.com/javase/7/docs/api/java/io/ByteArrayInputStream.html
[13]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage
[14]: https://apireference.aspose.com/email/java/com.aspose.email/SmtpClient
[15]: https://apireference.aspose.com/email/java/com.aspose.email/SmtpClient#send(com.aspose.email.MailMessage)
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/words/java
[18]: https://docs.aspose.com/email/java
[19]: https://blog.aspose.com/2021/04/12/read-email-messages-programmatically-using-java/





