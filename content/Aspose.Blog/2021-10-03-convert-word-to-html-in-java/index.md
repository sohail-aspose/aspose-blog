---
title: 'Convert Word Documents to HTML using Java'
seoTitle: "Convert Word to HTML in Java | DOCX to HTML | DOC to HTML | Java API"
description: "Use Java Word API to convert Word document to HTML using Java. Control DOCX or DOC to HTML conversion with additional options dynamically."
date: Sun, 03 Oct 2021 15:33:00 +0000
draft: false
url: /2021/10/03/convert-word-to-html-in-java/
author: Usman Aziz
summary: "In order to embed the content of Word documents into your applications, you might need to perform the conversion. The most widely opted conversions in such cases are Word to [HTML][1] or Word to image. In accordance with that, this article covers **how to convert Word [DOCX][2] or [DOC][3] files to HTML using Java**. Also, we'll discuss how to keep resource files in a separate folder."
tags: ['DOC to HTML Java', 'DOCX to HTML Java', 'Java Word to HTML Converter', 'Word to HTML Java']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Word-to-HTML.jpg" alt="Word to HTML Java">}}


In order to embed the content of Word documents into your applications, you might need to perform the conversion. The most widely opted conversions in such cases are Word to [HTML][4] or Word to image. In accordance with that, this article covers **how to convert Word [DOCX][5] or [DOC][6] files to HTML using Java**. Also, we'll discuss how to keep resource files in a separate folder.

*   [Java API for Word to HTML Conversion][7]
*   [Convert a Word Document to HTML][8]
*   [Specify Resource Folder in Word to HTML Conversion][9]

## Java API for Word to HTML Conversion {#API-for-Word-to-HTML-Conversion}

For DOCX/DOC to HTML conversion, we will use [Aspose.Words for Java][10]. It is a powerful API to implement word processing features from within the Java applications. Furthermore, the API provides high-fidelity conversion of Word documents to HTML and [other formats][11]. You can either [download][12] the API or install it from [Maven][13].

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-words</artifactId>
    <version>21.10</version>
    <type>pom</type>
</dependency>
```

## Convert a Word Document to HTML in Java {#Convert-a-Word-Document-to-HTML}

To convert a Word document to HTML, you only need to load the document and save it as an HTML file. The following are the steps to convert a Word DOCX file to HTML using Java.

*   Load the Word document using [Document][14] class.
*   Convert Word document to HTML using [Document.save(string, SaveFormat)][15] method.

The following code sample shows how to convert a Word document to HTML using Java.

{{< gist aspose-com-gists ab4b54ad510e46d63b36a7bbbd0f1088 "word-to-html.java" >}}

## Specify Resource Folder in Word to HTML Conversion {#Specify-Resource-Folder-in-Word-to-HTML-Conversion}

You can also configure the API to save the resource files in a separate folder. Moreover, you can keep fonts and images separately in different folders. The following are the steps to specify the resource folder.

*   Load the Word document using [Document][16] class.
*   Create an object of [HtmlSaveOptions][17] class.
*   Set resource folder using [HtmlSaveOptions.setResourceFolder][18] method.
*   Convert Word document to HTML using [Document.save(string, HtmlSaveOptions)][19] method.

The following code sample keeps resource files in a separate folder in Word to HTML conversion.

{{< gist aspose-com-gists ab4b54ad510e46d63b36a7bbbd0f1088 "word-to-html-resources.java" >}}

You can [read more][20] about working with resource folders in Word to HTML conversion.

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Words for Java without evaluation limitations by getting a free [temporary license][21].

## Conclusion

In this article, you have learned how to convert Word DOCX or DOC files to HTML programmatically using Java. In addition to this, you have seen how to store resource files separately in Word to HTML conversion. Besides, you can read more about Aspose.Words for Java using the [documentation][22]. Furthermore, you can share your queries with us on our [forum][23].

## See Also

*   [Create Word Documents without MS Office using Java][24]




[1]: https://docs.fileformat.com/web/html/
[2]: https://docs.fileformat.com/word-processing/docx/
[3]: https://docs.fileformat.com/word-processing/doc/
[4]: https://docs.fileformat.com/web/html/
[5]: https://docs.fileformat.com/word-processing/docx/
[6]: https://docs.fileformat.com/word-processing/doc/
[7]: #API-for-Word-to-HTML-Conversion
[8]: #Convert-a-Word-Document-to-HTML
[9]: #Specify-Resource-Folder-in-Word-to-HTML-Conversion
[10]: https://products.aspose.com/words/java
[11]: https://docs.aspose.com/words/java/convert-a-document/
[12]: https://downloads.aspose.com/words/java
[13]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[14]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[15]: https://apireference.aspose.com/words/java/com.aspose.words/Document#save(java.lang.String,int)
[16]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[17]: https://apireference.aspose.com/words/java/com.aspose.words/HtmlSaveOptions
[18]: https://apireference.aspose.com/words/java/com.aspose.words/htmlsaveoptions#ResourceFolder
[19]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String,com.aspose.words.SaveOptions)
[20]: https://docs.aspose.com/words/java/convert-a-document-to-html-mhtml-or-epub/#specify-a-folder-for-saving-resources
[21]: https://purchase.aspose.com/temporary-license
[22]: https://docs.aspose.com/words/java
[23]: https://forum.aspose.com/
[24]: https://blog.aspose.com/2020/03/11/create-rich-word-documents-programmatically-in-java-using-java-word-api/




