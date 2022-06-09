---
title: 'Copy Content from a Word Document to Another in Java'
seoTitle: "Java: Copy Content from a Word Document to Another | Java DOCX Lib"
description: "Use Java Word library to copy the content of a Word document to another in Java. Create a copy of a Word document and save it as a new document."
date: Fri, 01 Oct 2021 14:42:00 +0000
draft: false
url: /2021/10/01/copy-content-from-a-word-document-to-another-in-java/
author: Usman Aziz
summary: 'While working with MS Word documents, you may need to copy the content from one document to another. Moreover, the clones of Word documents are also required in certain cases. To automate these operations, this article covers **how to copy the content from one Word document to another in Java**. Also, you will learn how to create a copy of a Word document programmatically.'
tags: ['clone ms word documents in java', 'copy content from one doc to other in java', 'copy content from one docx to other in java', 'copy content from one word document to other in java', 'create copy of a word document in java']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Copy-Word-Documents.jpg" alt="Copy content from one word document to another in Java">}}


While working with MS Word documents, you may need to copy the content from one document to another. Moreover, the clones of Word documents are also required in certain cases. To automate these operations, this article covers **how to copy the content from one Word document to another in Java**. Also, you will learn how to create a copy of a Word document programmatically.

*   [Java Library to Copy Content of Word Documents][1]
*   [Copy Content from One Word Document to Another][2]
*   [Create Copy of a Word Document][3]

## Java Library to Copy Content of Word Documents {#Library-to-Copy-Content-from-Word-Documents}

To copy the content from one document to another, we will use [Aspose.Words for Java][4]. It is a feature-rich library to create and manipulate Word documents from within the Java applications. You can download the API’s JAR from the [downloads section][5] or install it using the following Maven configurations in pom.xml.

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

## Copy Content from a Word Document to Another in Java {#Copy-Content-from-One-Word-Document-to-Another}

The following are the steps to copy the content of a Word document to another using Java.

*   Load the source Word document using [Document][6] class.
*   Similarly, load the destination document using [Document][7] class.
*   Copy the content of source Word document into destination document using [Document.appendDocument(Document, ImportFormatMode)][8] method.
*   Save the destination document using [Document.save(string)][9] method.

The following code sample shows how to copy the content of a Word document to another.

{{< gist aspose-com-gists 1c06147b9bd1212e71bfc8b6ec0ef4b8 "copy-content.java" >}}

## Create Copy of a Word Document in Java {#Create-Copy-of-a-Word-Document}

You can also copy the content of a Word document into a new document. In other words, you can create a clone of a document. The following are the steps to create a copy of the Word document using Java.

*   Load the Word document using [Document][10] class.
*   Create a clone using [Document.deepClone()][11] method.
*   Save the cloned document using [Document.save(string)][12] method.

The following code sample shows how to create a copy of a Word DOCX file in Java.

{{< gist aspose-com-gists 1c06147b9bd1212e71bfc8b6ec0ef4b8 "clone-document.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [get a temporary license][13] in order to use Aspose.Words for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to copy the content from a Word document to another in Java. Moreover, you have seen how to clone a Word document programmatically. Aspose.Words for Java provides a wide range of other features that you can explore using the [documentation][14]. Also, you can ask your queries via our [forum][15].

## See Also

*   [Create Word Documents without MS Office using Java][16]
*   [Convert PDF to Word in Java][17]
*   [Convert Word to PDF in Java][18]




[1]: #Library-to-Copy-Content-from-Word-Documents
[2]: #Copy-Content-from-One-Word-Document-to-Another
[3]: #Create-Copy-of-a-Word-Document
[4]: https://products.aspose.com/words/java/
[5]: https://downloads.aspose.com/words/java/
[6]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[7]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[8]: https://apireference.aspose.com/words/java/com.aspose.words/document#appendDocument(com.aspose.words.Document,int)
[9]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String)
[10]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[11]: https://apireference.aspose.com/words/java/com.aspose.words/document#deepClone()
[12]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String)
[13]: https://purchase.aspose.com/temporary-license
[14]: https://docs.aspose.com/words/java/
[15]: https://forum.aspose.com/
[16]: https://blog.aspose.com/2020/03/11/create-rich-word-documents-programmatically-in-java-using-java-word-api/
[17]: https://blog.aspose.com/2020/01/17/convert-pdf-to-word-doc-docx-in-java/
[18]: https://blog.aspose.com/2020/02/20/convert-word-doc-docx-to-pdf-in-java-programmatically/




