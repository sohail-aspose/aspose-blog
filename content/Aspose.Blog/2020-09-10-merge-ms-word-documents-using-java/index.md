---
title: 'Merge MS Word Documents using Java'
seoTitle: ""
description: ""
date: Thu, 10 Sep 2020 22:17:00 +0000
draft: false
url: /2020/09/10/merge-ms-word-documents-using-java/
author: Usman Aziz
summary: 'The merger of multiple MS Word documents could be needed in various scenarios. For example, reducing the number of documents, keeping similar kinds of content in a single file (i.e. invoices), and etc. Many online applications let you merge two or more MS Word documents, however, you may need to implement document merging features within your own web or desktop applications. For such a case, in this article, you will learn how to merge MS Word documents using Java.'
tags: ['merge doc docx using java', 'merge multiple word documents using java', 'merge two word documents using java', 'merge word documents using java']
categories: ['Aspose.Words Product Family']
---

The merger of multiple MS Word documents could be needed in various scenarios such as reducing the number of documents, keeping similar kinds of content in a single file (i.e. invoices), and etc. Many online applications let you merge two or more MS Word documents, however, you may need to implement document merging features within your own web or desktop applications. For such a case, in this article, you will learn **how to merge MS Word DOCX documents using Java**.

*   [Java API for Merging MS Word Documents][1]
*   [Merge MS Word DOCX Documents using Java][2]
*   [Additional Options to Merge MS Word Documents][3]

## Merge Word Documents with Java API {#Java-API-for-Merging-MS-Word-Documents}

[Aspose.Words for Java][4] is a popular word processing API that lets you create, manipulate, and play with MS Word document formats within Java applications. Along with a wide range of document generation features, the API allows you to merge MS Word documents quite easily. You can [download][5] the API or install it using the following Maven configurations.

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
    <version>20.8</version>
    <type>pom</type>
</dependency>
```

## Merge MS Word DOCX Documents using Java {#Merge-MS-Word-Documents-using-Java}

Merging MS Word documents using Aspose.Words for Java is as easy as pie. Just load the documents and merge them by calling a single method. Below are the two MS Word documents that you will merge in the following code samples.



{{< figure align=center src="images/Source-Word-Documents-1024x633.jpg" alt="Word Documents to Merge">}}


The following are the steps to merge two MS Word documents.

*   Load the destination Word document using the [Document][6] class.
*   Load the source Word document using the [Document][7] class.
*   Merge source Word document into destination document using [Document.appendDocument(Document, ImportFormatMode)][8] method.
*   Set [ImportFormatMode][9] in the _appendDocument_ method to specify the formatting of the source document.
*   Save the destination Word document using [Document.save(String, SaveFormat)][10] method.

The following code sample shows how to merge MS Word documents (DOCX) using Java.

{{< gist aspose-com-gists 0e5aba636419098aef07e054cbd08d77 "merge-word-documents.java" >}}

The following is the screenshot of the merged MS Word document.



{{< figure align=center src="images/Merged-Word-Document-1024x676.jpg" alt="Merged MS Word Documents">}}


## Merge MS Word DOCX with Additional Options {#Merge-MS-Word-Documents-with-Additional-Options}

Aspose.Words for Java also provides some additional options to customize the appearance of the source document after performing the merger. The [ImportFormatOptions][11] class provides the following customization options.

*   [setIgnoreHeaderFooter][12] (boolean value) – Specifies that source formatting of headers/footers content is ignored if [ImportFormatMode.KEEP\_SOURCE\_FORMATTING][13] mode is used.
*   [setIgnoreTextBoxes][14] (boolean value) – Specifies that source formatting of textboxes content is ignored if [ImportFormatMode.KEEP\_SOURCE\_FORMATTING][15] mode is used.
*   [setKeepSourceNumbering][16] (boolean value) – Specifies how to import numbering when it clashes in source and destination documents.
*   [setSmartStyleBehavior][17] (boolean value) – Specifies how to import styles when having similar names in source and destination documents.

The following are the steps to merge two MS Word documents with additional options.

*   Load the destination Word document using the [Document][18] class.
*   Load the source Word document using the [Document][19] class.
*   Create an instance of [ImportFormatOptions][20] class and set the desired options.
*   Merge source Word document into destination document using [Document.appendDocument(Document, ImportFormatMode, ImportFormatOptions)][21] method.
*   Save the destination Word document using [Document.save(String, SaveFormat)][22] method.

The following code sample shows how to merge two MS Word documents with additional options using Java.

{{< gist aspose-com-gists 0e5aba636419098aef07e054cbd08d77 "merge-word-documents-customized.java" >}}

## Conclusion

In this article, you have seen how to merge MS Word DOCX documents using Java. Furthermore, you have learned how to use the additional options to customize the document merging feature. You can explore more about Aspose.Words for Java using the [documentation][23].

## See Also

*   [Split MS Word Documents using C#][24]




[1]: #Java-API-for-Merging-MS-Word-Documents
[2]: #Merge-MS-Word-Documents-using-Java
[3]: #Merge-MS-Word-Documents-with-Additional-Options
[4]: https://products.aspose.com/words/java
[5]: https://downloads.aspose.com/words/java
[6]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[7]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[8]: https://apireference.aspose.com/words/java/com.aspose.words/document#appendDocument(com.aspose.words.Document,int)
[9]: https://apireference.aspose.com/words/java/com.aspose.words/ImportFormatmode
[10]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String,int)
[11]: https://apireference.aspose.com/words/java/com.aspose.words/ImportFormatOptions
[12]: https://apireference.aspose.com/words/java/com.aspose.words/importformatoptions#IgnoreHeaderFooter
[13]: https://apireference.aspose.com/words/java/com.aspose.words/ImportFormatMode#KEEP_SOURCE_FORMATTING
[14]: https://apireference.aspose.com/words/java/com.aspose.words/importformatoptions#IgnoreTextBoxes
[15]: https://apireference.aspose.com/words/java/com.aspose.words/ImportFormatMode#KEEP_SOURCE_FORMATTING
[16]: https://apireference.aspose.com/words/java/com.aspose.words/importformatoptions#KeepSourceNumbering
[17]: https://apireference.aspose.com/words/java/com.aspose.words/importformatoptions#SmartStyleBehavior
[18]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[19]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[20]: https://apireference.aspose.com/words/java/com.aspose.words/ImportFormatOptions
[21]: https://apireference.aspose.com/words/java/com.aspose.words/document#appendDocument(com.aspose.words.Document,int,com.aspose.words.ImportFormatOptions)
[22]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String,int)
[23]: https://docs.aspose.com/words/java/
[24]: https://blog.aspose.com/2020/08/26/split-ms-word-documents-using-csharp/





