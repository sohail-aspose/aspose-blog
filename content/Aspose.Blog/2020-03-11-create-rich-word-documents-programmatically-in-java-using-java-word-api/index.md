---
title: 'Create Rich Word Documents Programmatically in Java'
seoTitle: ""
description: ""
date: Wed, 11 Mar 2020 22:08:00 +0000
draft: false
url: /2020/03/11/create-rich-word-documents-programmatically-in-java-using-java-word-api/
author: Usman Aziz
summary: ''
tags: ['Create List in Word in Java', 'Create Rich Word Documents in Java', 'Create table in Word in Java', 'Java Word API']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Create-Rich-Word-Document-in-Java.png" alt="Create Rich Word Document in Java">}}


In recent years, the dynamic generation of Word documents has become a popular feature for composing reports, quotes, invoices, and other types of documents. Various manufacturing companies generate invoices based on the data stored in the databases. In such cases, document automation makes it possible to save time, efforts and resources required in the manual document creation process. This article aims to target the document automation process and lets you know how to **create Word documents programmatically in Java**.

*   [Java API to Create Word Documents][1]
*   [Create a Word Document using Java][2]
*   [Create a Word Document having Table][3]
*   [Insert a List in Word Document][4]
*   [Create Word Document having Image][5]

## Java API to Create Word Documents {#Java-API-to-Create-Word-Documents}

In this article, we'll use [Aspose.Words for Java][6] which is a feature-rich API to create, edit, or convert Word documents in Java-based applications. You can [download][7] the API's JAR or install it using the following Maven configurations:

### Repository```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```

### Dependency```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-words</artifactId>
    <version>20.2</version>
    <classifier>jdk17</classifier>
</dependency>
```

In the following sections, you'll learn how to create a Word document containing different elements such as text, paragraph, table, list, images, etc. programmatically using Java.

## Create a Word Document using Java {#Create-a-Word-Document-using-Java}

Most of the time, a considerable portion of the content in a Word document is based on the text. Therefore, we'll start our journey by creating a Word document with a heading and a paragraph. The following are the steps to create a Word document:

*   First, create an instance of [Document][8] class.
*   Create a [DocumentBuilder][9] object and initialize it with the _Document_ object.
*   Use the [Font][10] class and set font size, family, and etc.
*   Set paragraph's properties using [ParagraphFormat][11] class.
*   Write text to the document using [DocumentBuilder.write()][12] method.
*   Finally, call [Document.save()][13] method to create the document.

The following code sample shows how to create a Word document containing text in Java.

{{< gist aspose-com-gists ddbf6c72cf9448156c41a4efeb3067eb "create-Word-document-with-text.java" >}}

### Output



{{< figure align=center src="images/Create-Word-with-Text.png" alt="Generate Word Document in Java">}}


## Create a Word Document having Table using Java {#Create-a-Word-Document-having-Table-using-Java}

Tables in the Word documents are used to organize the content in the form of rows and columns. In this section, we'll create a simple table containing two rows and two columns. Creating a table includes four basic operations:

*   Starting the table
*   Inserting a cell
*   Ending the row
*   Ending the table

The following are the step to create a table in Word document using Java:

*   First, create the objects of [Document][14] and [DocumentBuilder][15] class.
*   Create a table using [Table][16] class.
*   Insert a cell using [DocumentBuilder.insertCell()][17] method.
*   Set table's properties as per your requirements.
*   Add text to the cell using [DocumentBuilder.write()][18] method.
*   End the row and table using [DocumentBuilder.endRow()][19] and [DocumentBuilder.endTable()][20] methods respectively.
*   Finally, save the document.

The following sample shows how to create a table in a Word document.

{{< gist aspose-com-gists ddbf6c72cf9448156c41a4efeb3067eb "create-Word-document-with-table.java" >}}

### Output



{{< figure align=center src="images/Create-Word-with-Table.png" alt="Java generate Word document with table">}}


## Create a List in Word Document using Java {#Insert-a-List-in-Word-Document-using-Java}

The following are the steps to add a list to the Word document.

*   First, create an object of [Document][21] class.
*   Add your desired type of list to the document using _Document.getLists().add()_ method.
*   Get the list from the document into a [List][22] object.
*   Populate the list using the [DocumentBuilder][23] object.
*   Finally, save the document.

The following code sample shows how to create a list in Word document using Java.

{{< gist aspose-com-gists ddbf6c72cf9448156c41a4efeb3067eb "create-Word-document-with-list.java" >}}

### Output



{{< figure align=center src="images/Create-Word-with-List.png" alt="Insert List in Word docx in Java">}}


## Insert Image in a Word Document using Java {#Create-Word-Document-having-Image-using-Java}

The insertion of an image into a Word document is as simple as pie. The following are some simple steps to perform this operation:

*   First, create an object of [Document][24] class.
*   Create an object of [DocumentBuilder][25] class and initialize it with the _Document_ object.
*   Insert image using [DocumentBuilder.insertImage()][26] method.
*   Finally, save the document.

The following code sample shows how to insert an image to the Word document using Java.

{{< gist aspose-com-gists ddbf6c72cf9448156c41a4efeb3067eb "create-Word-document-with-image.java" >}}

### Output



{{< figure align=center src="images/Create-Word-with-Image.png" alt="Insert Image in Word docx in Java">}}


## Conclusion

In this article, you have learned **how to create rich Word documents programmatically using Java**. Furthermore, the code samples have shown how to add text, tables, images, and lists to Word documents. You can [read more][27] about how to insert various elements into a Word document using Aspose.Words for Java.

## Try Aspose.Words for Java for Free

You can get a free [temporary license][28] to try and use Aspose.Words for Java without trial limitations.

## See Also

*   [Convert Word DOCX to PDF in Java][29]




[1]: #Java-API-to-Create-Word-Documents
[2]: #Create-a-Word-Document-using-Java
[3]: #Create-a-Word-Document-having-Table-using-Java
[4]: #Insert-a-List-in-Word-Document-using-Java
[5]: #Create-Word-Document-having-Image-using-Java
[6]: https://products.aspose.com/words/java
[7]: https://downloads.aspose.com/words/java
[8]: https://apireference.aspose.com/java/words/com.aspose.words/Document
[9]: https://apireference.aspose.com/java/words/com.aspose.words/DocumentBuilder
[10]: https://apireference.aspose.com/java/words/com.aspose.words/Font
[11]: https://apireference.aspose.com/java/words/com.aspose.words/ParagraphFormat
[12]: https://apireference.aspose.com/java/words/com.aspose.words/DocumentBuilder#write(java.lang.String)
[13]: https://apireference.aspose.com/java/words/com.aspose.words/document#save(java.lang.String)
[14]: https://apireference.aspose.com/java/words/com.aspose.words/Document
[15]: https://apireference.aspose.com/java/words/com.aspose.words/DocumentBuilder
[16]: https://apireference.aspose.com/java/words/com.aspose.words/Table
[17]: https://apireference.aspose.com/java/words/com.aspose.words/documentbuilder#insertCell()
[18]: https://apireference.aspose.com/java/words/com.aspose.words/DocumentBuilder#write(java.lang.String)
[19]: https://apireference.aspose.com/java/words/com.aspose.words/documentbuilder#endRow()
[20]: https://apireference.aspose.com/java/words/com.aspose.words/documentbuilder#endTable()
[21]: https://apireference.aspose.com/java/words/com.aspose.words/Document
[22]: https://apireference.aspose.com/java/words/com.aspose.words/List
[23]: https://apireference.aspose.com/java/words/com.aspose.words/DocumentBuilder
[24]: https://apireference.aspose.com/java/words/com.aspose.words/Document
[25]: https://apireference.aspose.com/java/words/com.aspose.words/DocumentBuilder
[26]: https://apireference.aspose.com/java/words/com.aspose.words/documentbuilder#insertImage(java.lang.String)
[27]: https://docs.aspose.com/display/wordsjava/Developer+Guide
[28]: https://purchase.aspose.com/temporary-license
[29]: https://blog.aspose.com/2020/02/20/convert-word-doc-docx-to-pdf-in-java-programmatically/





