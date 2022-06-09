---
title: 'Convert HTML Files to Word Document in Java'
seoTitle: "Convert HTML to Word in Java | HTML to DOCX, DOC, DOT, DOCM etc."
description: "Use Java Word library to convert HTML files to Word processing format in Java. Convert HTML to DOCX, DOC, DOT, DOCM etc. programmatically."
date: Mon, 29 Nov 2021 06:48:08 +0000
draft: false
url: /2021/11/29/convert-html-to-word-in-java/
author: Usman Aziz
summary: 'In various cases, you may need to convert the HTML content to a Word document. For example, for generating the document from a WYSIWYG HTML editor or converting a web page to DOCX or DOC format. To perform this conversion programmatically, this article covers **how to convert HTML files to Word [DOCX][1], [DOC][2], [DOCM][3], or other formats in Java**.'
tags: ['Convert HTML to DOC in Java', 'Convert HTML to DOCM in Java', 'Convert HTML to DOCX in Java', 'Convert HTML to DOT in Java', 'Convert HTML to Word in Java']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Convert-HTML-to-Word.jpg" alt="Convert HTML Files to Word DOCX DOC in Java">}}


In various cases, you may need to convert the HTML content to a Word document. For example, for generating the document from a WYSIWYG HTML editor or converting a web page to DOCX or DOC format. To perform this conversion programmatically, this article covers **how to convert HTML files to Word [DOCX][4], [DOC][5], [DOCM][6], or other formats in Java**.

*   [Library to Convert HTML to Word][7]
*   [Convert an HTML File to DOCX/DOC/DOCM etc.][8]
*   [Convert a Web Page to Word using URL][9]
*   [HTML String to Word Conversion][10]

**Info**: If you ever need to get a Word document from a PowerPoint presentation, you can use Aspose [Presentation to Word Document][11] converter.

## Java Library to Convert HTML to Word {#Java-Library-to-Convert-HTML-to-Word}

To convert HTML to DOCX, DOC, DOT, DOCM, and other Word formats, we will use [Aspose.Words for Java][12]. It is a powerful library to create and manipulate Word documents programmatically. Moreover, it provides a built-in document converter that provides high fidelity conversion of/to Word processing documents. You can download the API's JAR from the [downloads section][13] or install it using the following Maven configurations in pom.xml.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-words</artifactId>
    <version>21.11</version>
    <type>pom</type>
</dependency>
```

## Convert HTML to DOCX/DOC/DOCM in Java {#Convert-an-HTML-File-to-DOCX-DOC-DOCM}

Using Aspose.Words for Java, the conversion of an HTML file to Word format can be done in a couple of steps, which are mentioned below.

*   Load the HTML file using [Document][14] class.
*   Save the HTML file as Word document using [Document.save(string, SaveFormat)][15] method.

The [SaveFormat][16]  enum in _Document.save()_ method specifies the format in which you want to convert the HTML file. The following code sample shows how to generate a Word document from HTML in Java.

{{< gist aspose-com-gists 6292eed8c4680f319ff8c909e6728582 "html-to-word.java" >}}

## Convert a Web Page to Word using URL in Java {#Convert-a-Web-Page-to-Word-using-URL}

You can also convert a web page to a Word document directly from its URL. The following are the steps to convert HTML to DOCX using URL in Java.

*   Create an instance of [URL][17] class and initialize it with desired URL.
*   Open URL into a [InputStream][18] object.
*   Create an instance of [HtmlLoadOptions][19] class.
*   Create an instance of [Document][20] class and initialize it with _InputStream_ and _HtmlLoadOptions_ objects.
*   Save the web page as Word document using [Document.save(string, SaveFormat)][21] method.

The following code sample shows how to convert a web page to a Word document using a URL.

{{< gist aspose-com-gists 6292eed8c4680f319ff8c909e6728582 "web-page-to-word.java" >}}

## Convert an HTML String to Word using Java {#HTML-String-to-Word-Conversion}

Aspose.Words for Java also allows you to generate a Word document from HTML string dynamically. The following are the steps to perform this operation.

*   Create an instance of [Document][22] class.
*   Create an instance of [DocumentBuilder][23] class and initialize it with _Document_ object.
*   Insert HTML into the document using [DocumentBuilder.InsertHtml(string)][24] method.
*   Save the Word document using [Document.save(string, SaveFormat)][25] method.

The following code sample shows how to convert an HTML string to a DOCX file using Java.

{{< gist aspose-com-gists 6292eed8c4680f319ff8c909e6728582 "HTML-string-to-word.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Words for Java without evaluation limitations by getting a free [temporary license][26].

## Conclusion

In this article, you have learned how to convert HTML files to Word DOCX, DOC, DOCM, or other formats programmatically using Java. Moreover, you have seen how to convert an HTML string or a web page from a URL to a Word document dynamically. You can simply install Aspose.Words for Java and use the provided code to build your HTML to Word converter. Besides, you can visit the [documentation][27] to explore more about Aspose.Words for Java. Furthermore, you can share your queries with us on our [forum][28].

## See Also

*   [Create Word Documents without MS Office using Java][29]
*   [Convert PDF to Word in Java][30]
*   [Convert Word to PDF in Java][31]




[1]: https://docs.fileformat.com/word-processing/docx/
[2]: https://docs.fileformat.com/word-processing/doc/
[3]: https://docs.fileformat.com/word-processing/docm/
[4]: https://docs.fileformat.com/word-processing/docx/
[5]: https://docs.fileformat.com/word-processing/doc/
[6]: https://docs.fileformat.com/word-processing/docm/
[7]: #Java-Library-to-Convert-HTML-to-Word
[8]: #Convert-an-HTML-File-to-DOCX-DOC-DOCM
[9]: #Convert-a-Web-Page-to-Word-using-URL
[10]: #HTML-String-to-Word-Conversion
[11]: https://products.aspose.app/slides/conversion/ppt-to-word
[12]: https://products.aspose.com/words/java/
[13]: https://downloads.aspose.com/words/java
[14]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[15]: https://apireference.aspose.com/words/java/com.aspose.words/Document#save(java.lang.String,int)
[16]: https://apireference.aspose.com/words/java/com.aspose.words/SaveFormat
[17]: https://docs.oracle.com/javase/7/docs/api/java/net/URL.html
[18]: https://docs.oracle.com/javase/7/docs/api/java/io/InputStream.html
[19]: https://apireference.aspose.com/words/java/com.aspose.words/HtmlLoadOptions
[20]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[21]: https://apireference.aspose.com/words/java/com.aspose.words/Document#save(java.lang.String,int)
[22]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[23]: https://apireference.aspose.com/words/java/com.aspose.words/DocumentBuilder
[24]: https://apireference.aspose.com/words/java/com.aspose.words/DocumentBuilder#insertHtml(java.lang.String)
[25]: https://apireference.aspose.com/words/java/com.aspose.words/Document#save(java.lang.String,int)
[26]: https://purchase.aspose.com/temporary-license
[27]: https://docs.aspose.com/words/java
[28]: https://forum.aspose.com/
[29]: https://blog.aspose.com/2020/03/11/create-rich-word-documents-programmatically-in-java-using-java-word-api/
[30]: https://blog.aspose.com/2020/01/17/convert-pdf-to-word-doc-docx-in-java/
[31]: https://blog.aspose.com/2020/02/20/convert-word-doc-docx-to-pdf-in-java-programmatically/




