---
title: 'Split MS Word Documents using Java'
seoTitle: "Split MS Word DOCX DOC in Java | Split by Section, Page or Page Range"
description: "Use Java Word API to split MS Word documents using Java. Split a Word document by sections, pages, or a range of pages within Java applications."
date: Fri, 29 Jan 2021 09:25:55 +0000
draft: false
url: /2021/01/29/split-ms-word-documents-using-java/
author: Usman Aziz
summary: 'In various cases, you need to split an MS Word document into multiple documents. For example, you may need to create a separate document for each page, section, or a collection of pages in a Word document. In order to automate the document splitting, this article covers **how to split MS Word documents programmatically using Java**. The following sections provide a step by step tutorial and code samples of the above-mentioned splitting criteria.'
tags: ['Java Document Splitter', 'Split-Word-Document-by-Pages-in-Java', 'Split-Word-Document-by-Sections-in-Java', 'Split-Word-by-Page-Range-in-Java']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Split-Word-Documents.jpg" alt="Split Word Documents Java">}}


In various cases, you need to split an MS Word document into multiple documents. For example, you may need to create a separate document for each page, section, or collection of pages in a Word document. In order to automate the document splitting, this article covers **how to split MS Word DOCX programmatically using Java**. The following sections provide a step-by-step tutorial and code samples of the above-mentioned splitting criteria.

*   [Java API to Split Word Documents][1]
*   [Split a Word DOCX/DOC using Java][2]
*   [Use Page Range to Split Word Document][3]
*   [Split Word Document by Sections][4]
*   [Get Free API License][5]

## Java API to Split Word DOCX {#Java API to Split Word Documents}

[Aspose.Words for Java][6] is a powerful and feature-rich document manipulation API that lets you create and process MS Word documents. In addition to the basic as well as advanced Word automation features, the API also allows you to split a Word document into multiple documents. You can either [download][7] the API or install it within your Maven-based application using the following configurations.

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
    <version>21.1</version>
    <classifier>jdk17</classifier>
</dependency>
```

## Word Document Splitter - Helper Classes

Before you start splitting the documents, you would need to add the following helper classes to your project that implement a Java document splitter based on Aspose.Words for Java. Once you have added the classes, you can proceed to split the documents using the code samples provided in the sections below.

*   [DocumentPageSplitter][8]
*   [PageSplitter][9]

## Split a Word DOCX using Java {#Split-Word-Document-by-Pages}

First of all, let's have a look at how to split an MS Word document by page. In this case, each page of the source document will be converted into a separate Word document. The following are the steps to split pages of a Word document.

*   Load the Word document using [Document][10] class.
*   Create an object of [DocumentPageSplitter][11] and initialize it with the [Document][12] object.
*   Loop through the pages in the document.
*   Use [DocumentPageSplitter.getDocumentOfPage(Int pageIndex)][13] method to retrive each page into a [Document][14] object.
*   Save the document using the [Document.save(String)][15] method.

The following code sample shows how to split a Word document using Java.

{{< gist aspose-com-gists 163f03e6cd53fd757db6b4dc041e797c "split-word-document-by-page.java" >}}

## Use Page Range to Split Word DOCX in Java {#Use-Page-Range-to-Split-Word-Document}

You can also define a page range that you want to split from the source Word document. The following are the steps to perform this operation.

*   Load the Word document using [Document][16] class.
*   Create an object of [DocumentPageSplitter][17] and initialize it with the [Document][18] object.
*   Use [DocumentPageSplitter.getDocumentOfPageRange(Int, Int)][19] method to retrive collection of pages into a [Document][20] object.
*   Save the document using the [Document.save(String)][21] method.

The following code sample shows how to split a Word document by a page range using Java.

{{< gist aspose-com-gists 163f03e6cd53fd757db6b4dc041e797c "split-word-document-by-page-range.java" >}}

## Split a Word Document by Sections using Java {#Split-Word-Document-by-Sections}

Aspose.Words for Java also allows you to split a Word document by section breaks. The following are the steps to perform this operation.

*   Load the Word document using [Document][22] class.
*   Loop through each section of the document using [Document.getSections()][23] method.
*   Clone section into a [Section][24] object using [Document.getSections().get(index).deepClone()][25] method.
*   Create a new _Document_ and add cloned section to the document using [Document.getSections().add(Section)][26] method.
*   Save the document using [Document.save(String)][27] method.

The following code sample shows how to split a Word document by sections using Java.

{{< gist aspose-com-gists 163f03e6cd53fd757db6b4dc041e797c "split-word-document-by-section.java" >}}

## Get a Free API License {#Get-a-Free-License}

You can [get a free temporary license][28] in order to try the API without evaluation limitations.

## Conclusion

In this article, you have learned how to split MS Word DOCX/DOC using Java. The step by step guide and code samples have shown how to split a Word document by sections, pages, or a range of pages. You can explore more about the Java Word API using [documentation][29].

## See Also

*   [Mail Merge in MS Word Documents using Java][30]




[1]: #Java API to Split Word Documents
[2]: #Split-Word-Document-by-Pages
[3]: #Use-Page-Range-to-Split-Word-Document
[4]: #Split-Word-Document-by-Sections
[5]: #Get-a-Free-License
[6]: https://products.aspose.com/words/java
[7]: https://downloads.aspose.com/words/java
[8]: https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/src/main/java/com/aspose/words/examples/loading_saving/DocumentPageSplitter.java
[9]: https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/src/main/java/com/aspose/words/examples/loading_saving/PageSplitter.java
[10]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[11]: https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/src/main/java/com/aspose/words/examples/loading_saving/DocumentPageSplitter.java
[12]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[13]: https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/src/main/java/com/aspose/words/examples/loading_saving/DocumentPageSplitter.java#L36
[14]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[15]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String)
[16]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[17]: https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/src/main/java/com/aspose/words/examples/loading_saving/DocumentPageSplitter.java
[18]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[19]: https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/src/main/java/com/aspose/words/examples/loading_saving/DocumentPageSplitter.java#L52
[20]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[21]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String)
[22]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[23]: https://apireference.aspose.com/words/java/com.aspose.words/document#Sections
[24]: https://apireference.aspose.com/words/java/com.aspose.words/Section
[25]: https://apireference.aspose.com/words/java/com.aspose.words/section#deepClone()
[26]: https://apireference.aspose.com/words/java/com.aspose.words/sectioncollection#add(com.aspose.words.Node)
[27]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String)
[28]: https://purchase.aspose.com/temporary-license
[29]: https://docs.aspose.com/words/java/getting-started/
[30]: https://blog.aspose.com/2020/12/11/mail-merge-in-word-documents-using-java/





