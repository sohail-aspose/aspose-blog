---
title: 'Compare MS Word Documents using Java'
seoTitle: ""
description: ""
date: Mon, 05 Oct 2020 16:44:15 +0000
draft: false
url: /2020/10/05/compare-ms-word-documents-using-java/
author: Usman Aziz
summary: 'The comparison of MS Word documents is performed to know about the difference between two versions of a document. MS Word provides a built-in option to compare the content of two documents. However, with the increased number of documents, it becomes difficult to perform the document comparison manually. In order to automate this process, this article covers how to compare two MS Word (DOC/DOCX) documents using Java.'
tags: ['compare two word documents in java', 'compare word documents in java', 'diff checker for word documents in java']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose_words-for-java.png" alt="compare word documents in Java">}}


The comparison of MS Word documents is performed to know about the difference between two versions of a document. MS Word provides a built-in option to compare the content of two documents. However, with the increased number of documents, it becomes difficult to perform the document comparison manually. In order to automate this process, this article covers **how to compare two MS Word (DOC/DOCX) documents using Java**.

*   [MS Word Document Comparison API for Java][1]
*   [Compare MS Word Documents using Java][2]
*   [Ignore Formatting in MS Word Document Comparison][3]
*   [Set Target Document for Comparison Differences][4]
*   [Set Granularity to Compare MS Word Documents][5]

## Java API to Compare MS Word Documents {#MS-Word-Document-Comparison-Java-API}

[Aspose.Words for Java][6] is a powerful document manipulation API that lets you create, read, modify, and convert MS Word documents. In addition, it allows you to compare two Word documents along with considering or ignoring the formatting of the content. You can [download][7] the API or get it installed using Maven configurations.

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
    <version>20.9</version>
    <classifier>jdk17</classifier>
</dependency>
```

## Compare MS Word Documents using Java {#Compare-MS-Word-Documents-using-Java}

The following are the steps to perform a simple Word document comparison using Aspose.Words for Java API.

*   Load the documents to be compared using the [Document][8] class.
*   Call [Document.compare(Document, String, Date)][9] method to compare the document with the one passed as an argument.

The following code sample shows how to compare two MS Word documents using Java.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-CompareTwoWordDocuments-NormalComparisonCase.java" >}}

## Java Word Document Comparison - Ignore Formatting {#Ignore-Formatting-in-Word-Document-Comparison}

There might be the case when the documents have different formatting applied to the content. In such cases, you would prefer to compare the text only while ignoring the formatting, headers/footers, footnotes, tables, comments, etc. The following are the steps to ignore the document's formatting when comparing two MS Word documents.

*   Load the documents to be compared using the [Document][10] class.
*   Create an object of [CompareOptions][11] class.
*   Set [CompareOptions.setIgnoreFormatting(true)][12].
*   Compare the documents using [Document.compare(Document, String, Date, CompareOptions)][13] method.

The following code sample shows how to compare MS Word documents ignoring the content's formatting using Java.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-CompareTwoWordDocuments-WithCompareOptions.java" >}}

## Set Target Word Document for Comparison Differences {#Set-Target-Document-for-Comparison-Differences}

Aspose.Words for Java also allows you to specify the source Word document during the comparison. For this, you can use [CompareOptions.setTarget()][14] property which relates to MS Word's "Show changes in" option. The following code sample shows how to specify the target document in the comparison.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-CompareDocumentWithComparisonTarget-CompareDocumentWithComparisonTarget.java" >}}

## Set Granularity to Compare Word Files in Java {#Set-Granularity-to-Compare-Word-Documents}

You can also set the granularity of changes when comparing two MS Word documents. This can be done using [CompareOptions.setGranularity()][15] property. The following are the possible granularity options.

*   [CHAR\_LEVEL][16]
*   [WORD\_LEVEL][17]

The following code sample shows how to set granularity when comparing MS Word documents using Java.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-CompareTwoWordDocuments-SpecifyComparisonGranularity.java" >}}

## Conclusion

In this article, you have seen how to compare two MS Word documents in various scenarios using Java. You can explore more about Aspose.Words for Java using the [documentation][18].

## Try for Free

Aspose offers a [temporary license][19] for you to try its APIs for free. You can get yours to evaluate Aspose.Words for Java.

## See Also

*   [Merge MS Word Documents using Java][20]
*   [Create Rich Word Documents in Java][21]
*   [Convert MS Word DOC/DOCX to PDF in Java][22]




[1]: #MS-Word-Document-Comparison-Java-API
[2]: #Compare-MS-Word-Documents-using-Java
[3]: #Ignore-Formatting-in-Word-Document-Comparison
[4]: #Set-Target-Document-for-Comparison-Differences
[5]: #Set-Granularity-to-Compare-Word-Documents
[6]: https://products.aspose.com/words/java
[7]: https://downloads.aspose.com/words/java
[8]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[9]: https://apireference.aspose.com/words/java/com.aspose.words/document#compare(com.aspose.words.Document,java.lang.String,java.util.Date)
[10]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[11]: https://apireference.aspose.com/words/java/com.aspose.words/CompareOptions
[12]: https://apireference.aspose.com/words/java/com.aspose.words/compareoptions#IgnoreFormatting
[13]: https://apireference.aspose.com/words/java/com.aspose.words/document#compare(com.aspose.words.Document,java.lang.String,java.util.Date)
[14]: https://apireference.aspose.com/words/java/com.aspose.words/compareoptions#Target
[15]: https://apireference.aspose.com/words/java/com.aspose.words/compareoptions#Granularity
[16]: https://apireference.aspose.com/words/java/com.aspose.words/granularity#CHAR_LEVEL
[17]: https://apireference.aspose.com/words/java/com.aspose.words/granularity#WORD_LEVEL
[18]: https://docs.aspose.com/words/java/getting-started/
[19]: https://purchase.aspose.com/temporary-license
[20]: https://blog.aspose.com/2020/09/10/merge-ms-word-documents-using-java/
[21]: https://blog.aspose.com/2020/03/11/create-rich-word-documents-programmatically-in-java-using-java-word-api/
[22]: https://blog.aspose.com/2020/02/20/convert-word-doc-docx-to-pdf-in-java-programmatically/





