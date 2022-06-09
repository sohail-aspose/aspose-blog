---
title: 'Add or Update Table of Contents in Word using Java'
seoTitle: "Java: Add or Updated Table of Contents in Word DOCX DOC Documents"
description: "Use Java Word Processing API to add or update table of contents in Word documents using Java. Complete guide with sample source code."
date: Fri, 02 Jul 2021 15:31:04 +0000
draft: false
url: /2021/07/02/add-or-update-toc-in-word-using-java/
author: Usman Aziz
summary: '[Table of Contents][1] (TOC) in a Word document gives you an overview of the content of the document. Also, it allows you to navigate to a particular section of the document. In this article, you will learn how to work with the table of contents in Word documents programmatically. Particularly, the article covers **how to add or update a table of contents in Word documents using Java**.'
tags: ['Add Table of Contents in a Word Document', 'Java API to Work with TOC in Word Documents']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Table-to-Contents-in-Word.jpg" alt="Table of Contents in Word in Java">}}


[Table of Contents][2] (TOC) in a Word document gives you an overview of the content of the document. Also, it allows you to navigate to a particular section of the document. In this article, you will learn how to work with the table of contents in Word documents programmatically. Particularly, the article covers **how to add or update a table of contents in Word documents using Java**.

*   [Java API to Work with TOC in Word Documents][3]
*   [Add Table of Contents in a Word Document][4]
*   [Update Table of Contents in a Word Document][5]

## Java API to Work with TOC in Word Documents {#Java-API-to-Work-with-TOC-in-Word-Documents}

In order to work with the table of contents in Word documents, we will use [Aspose.Words for Java][6]. It is a powerful word processing API that lets you create, modify or convert Word documents. You can either [download][7] the API or install it using the following Maven configurations.

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
    <version>21.6</version>
    <type>pom</type>
</dependency>
```

## Add Table of Contents in a Word Document using Java {#Add-Table-of-Contents-in-a-Word-Document}

The following are the steps to add a table of contents to a Word document using Java.

*   Create an instance of the [Document][8] class (in case of loading an existing Word document, provide the file’s path in the constructor).
*   Create an instance of [DocumentBuilder][9] class and initialize it with the _Document_ object created earlier.
*   Insert table of contents using [DocumentBuilder.insertTableOfContents(“\\\\o \\”1-3\\” \\\\h \\\\z \\\\u”)][10] method.
*   Update the fields using [Document.updateFields()][11] method.
*   Save the Word document using [Document.save(String)][12] method.

The following code sample shows how to add a table of contents to a Word document.

{{< gist aspose-com-gists aa89da3b6a5f420a2953413006080c54 "add-toc.java" >}}

## Update TOC in a Word Document using Java {#Update-Table-of-Contents-in-a-Word-Document}

The following are the steps to update the table of contents in a Word document using Java.

*   Create an instance of the [Document][13] class to load the Word document.
*   Update the fields using [Document.updateFields()][14] method.
*   Save the Word document using [Document.save(String)][15] method.

The following code sample shows how to update the table of contents in a Word document.

{{< gist aspose-com-gists aa89da3b6a5f420a2953413006080c54 "update-toc.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [get a temporary license][16] in order to use the API without evaluation limitations.

## Conclusion

In this article, you have learned how to work with the table of contents in Word documents programmatically. The steps and code samples have shown how to add or update the table of contents in a Word document using Java. You can learn more about the Java word processing API using the [documentation][17]. In case you would have any questions, feel free to let us know via our [forum][18].

## See Also

*   [Create MS Word Documents using Java without MS Office][19]
*   [Split MS Word Documents using Java][20]
*   [Mail Merge in MS Word Documents using Java][21]




[1]: https://en.wikipedia.org/wiki/Table_of_contents
[2]: https://en.wikipedia.org/wiki/Table_of_contents
[3]: #Java-API-to-Work-with-TOC-in-Word-Documents
[4]: #Add-Table-of-Contents-in-a-Word-Document
[5]: #Update-Table-of-Contents-in-a-Word-Document
[6]: https://products.aspose.com/words/java
[7]: https://downloads.aspose.com/words/java
[8]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[9]: https://apireference.aspose.com/words/java/com.aspose.words/DocumentBuilder
[10]: https://apireference.aspose.com/words/java/com.aspose.words/documentbuilder#insertTableOfContents(java.lang.String)
[11]: https://apireference.aspose.com/words/java/com.aspose.words/document#updateFields()
[12]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String)
[13]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[14]: https://apireference.aspose.com/words/java/com.aspose.words/document#updateFields()
[15]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String)
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/words/java
[18]: https://forum.aspose.com/
[19]: https://blog.aspose.com/2020/03/11/create-rich-word-documents-programmatically-in-java-using-java-word-api/
[20]: https://blog.aspose.com/2021/01/29/split-ms-word-documents-using-java/
[21]: https://blog.aspose.com/2020/12/11/mail-merge-in-word-documents-using-java/





