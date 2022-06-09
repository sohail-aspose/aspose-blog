---
title: 'Read Email Messages Programmatically using Java'
seoTitle: "Read Emails using Java | Extract Content from EML or MSG Emails"
description: "Use .NET Email API to read emails using Java. Extract content of the email messages such as to, from, subject, body and header information."
date: Mon, 12 Apr 2021 11:13:00 +0000
draft: false
url: /2021/04/12/read-email-messages-programmatically-using-java/
author: Usman Aziz
summary: "In certain cases, you may need to read and parse EML or MSG email messages from within your applications. In order to do it programmatically, this article shows **how to extract information from the email messages in Java**. Particularly, you will learn **how to read email's subject, to, from, body, and header information**."
tags: ['extract content from emails in java', 'read email header in java', 'read emails in java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Create-and-Send-Outlook-Emails-Java.jpg" alt="Read Emails in Java">}}


In certain cases, you may need to read and parse EML or MSG email messages from within your applications. In order to do it programmatically, this article shows **how to extract information from the email messages in Java**. Particularly, you will learn **how to read email's subject, to, from, body, and header information**.

*   [Java API to Read Emails][1]
*   [Read an Email Message using Java][2]
*   [Extract Email Body as Plain Text][3]
*   [Extract Header Information from Email][4]
*   [Decode Email Header's Value][5]
*   [Get a Free API License][6]

## Java API to Read Emails {#Java-API-to-Read-Emails}

In order to read the email messages, we'll use [Aspose.Email for Java][7]. It is a powerful API that lets you create feature-rich email clients in Java. You can either [download][8] the API's JAR or install it using the following Maven configurations.

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

## Read an Email Message using Java {#Read-an-Email-Message-using-Java}

The following are the steps to read an email message in Java.

*   Load the email file using [MailMessage][9] class.
*   Read the content of the email using [MailMessage][10] object, such as, To, From, Subject, Body, etc.

The following code sample shows how to read an email message using Java.

{{< gist aspose-com-gists dd95dfc64f21f075fd5c5e202451ae5d "read-email.java" >}}

## Extract Email Body as Plain Text in Java {#Extract-Email-Body-as-Plain-Text}

You can also read an email and extract its body as plain text instead of HTML. The following are the steps to perform this operation.

*   Load the email file using [MailMessage][11] class.
*   Extract email's body using [MailMessage.getHtmlBodyText(boolean)][12] method.

The following code sample shows how to extract email body as plain text in Java.

{{< gist aspose-com-gists dd95dfc64f21f075fd5c5e202451ae5d "read-email-plaintext.java" >}}

## Extract Header Information from an Email in Java {#Extract-Header-Information-from-Email}

Aspose.Email for Java also allows you to read header information of an email message. The following are the steps to perform this operation.

*   Load the email file using [MailMessage][13] class.
*   Loop through header collection of the email using [MailMessage.getHeaders()][14] method.

The following code sample shows how to read header of the email message using Java.

{{< gist aspose-com-gists dd95dfc64f21f075fd5c5e202451ae5d "extract-email-header.java" >}}

## Decode Email Headers in Java {#Decode-Email-Header-Value}

You can also decode the email headers using the following steps.

*   Load the email file using [MailMessage][15] class.
*   Get decoded email header's value using [MailMessage.getHeaders().getDecodedValue(String name)][16] method.

The following code sample shows how to decode an email header value in Java.

{{< gist aspose-com-gists dd95dfc64f21f075fd5c5e202451ae5d "decode-email-header.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [request a free temporary license][17] in order to use the API without evaluation limitations.

## Live Demo

*   [Email Viewer][18]

## Conclusion

In this article, you have learned how to read email messages using Java. Furthermore, you have seen how to extract header information from an email message. You can explore more about the Java email API using [documentation][19]. In addition, you can contact us via our [forum][20] in case of any queries.

## See Also

*   [Create and Send Outlook Email Messages using Java][21]




[1]: #Java-API-to-Read-Emails
[2]: #Read-an-Email-Message-using-Java
[3]: #Extract-Email-Body-as-Plain-Text
[4]: #Extract-Header-Information-from-Email
[5]: #Decode-Email-Header-Value
[6]: #Get-a-Free-API-License
[7]: https://products.aspose.com/email/java
[8]: https://downloads.aspose.com/email/java
[9]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage
[10]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage
[11]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage
[12]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage#getHtmlBodyText(boolean)
[13]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage
[14]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage#getHeaders()
[15]: https://apireference.aspose.com/email/java/com.aspose.email/MailMessage
[16]: https://apireference.aspose.com/email/java/com.aspose.email/HeaderCollection#getDecodedValue(java.lang.String)
[17]: https://purchase.aspose.com/temporary-license
[18]: http://products.aspose.app/email/viewer
[19]: https://docs.aspose.com/email/java/developer-guide/
[20]: https://forum.aspose.com/
[21]: https://blog.aspose.com/2020/05/20/create-and-send-outlook-email-messages-asynchronously-using-java/





