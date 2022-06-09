---
title: 'Create Multi-Column PDF Documents using Java'
seoTitle: "Create Multi-Column PDF using Java | Java PDF API | Source Code"
description: "Use Java PDF API to create multi-column PDF files from scratch using Java. Generate complex PDF files from within Java applications."
date: Mon, 06 Sep 2021 13:48:00 +0000
draft: false
url: /2021/09/06/create-multi-column-pdf-using-java/
author: Usman Aziz
summary: 'Various types of publications such as magazines, newspapers, research articles, etc. use multi-column page layouts. While generating such documents programmatically, you may need to create multi-column PDFs. For such cases, this article covers **how to create multi-column PDF files using Java**.'
tags: ['Java PDF API', 'create multi column pdf in java', 'create two column pdf in java', 'generate multi column pdf in java']
categories: ['Aspose.PDF Product Family']
---

Various types of publications such as magazines, newspapers, research articles, etc. use multi-column page layouts. While generating such documents programmatically, you may need to create multi-column PDFs. For such cases, this article covers **how to create multi-column PDF files using Java**.

*   [Java API to Create Multi-Column PDFs][1]
*   [Create a Multi-Column PDF File][2]

## Java API to Create Multi-Column PDFs {#API-to-Create-Multi-column-PDFs}

[Aspose.PDF for Java][3] is a feature-rich PDF manipulation API that lets you create simple as well as complex PDF files from scratch. We will use this API to create multiple-column PDF files using Java. You can either [download][4] the API's JAR or install it within your Java application using the following [Maven][5] configurations.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-pdf</artifactId>
    <version>21.9</version>
</dependency>
```

## Create a Multi-Column PDF using Java {#Create-a-Multi-column-PDF}

Aspose.PDF for Java makes it quite easier for you to create a multi-column PDF file. The following are the steps to achieve this.

*   First, create a new [Document][6] object.
*   Then, set the page margins using [Document.getPageInfo().getMargin().setLeft()][7] and [Document.getPageInfo().getMargin().setRight()][8] methods.
*   Add a new page in the PDF using [Document.getPages().add()][9] method and get its reference into a [Page][10] object.
*   Create a new [Graph][11] object and add it to the paragraph collection using [Page.getParagraphs().add()][12] method.
*   Create a new [Line][13] and add it to the [Graph.getShapes()][14] collection.
*   Add heading text to the page using [Page.getParagraphs().add()][15] method.
*   Create a new [FloatingBox][16] and specify the number of columns, column spacing, and column width.
*   Create another [Graph][17] object.
*   Add a new [Line][18] to the [Graph.getShapes()][19] collection.
*   Add Graph to the [FloatingBox.getParagraphs()][20] collection.
*   Create a new [TextFragment][21] and add it to [FloatingBox.getParagraphs()][22] collection.
*   Add [FloatingBox][23] to the page using [Page.getParagraphs().add()][24] method.
*   Finally, save the PDF file using [Document.save(string)][25] method.

The following code sample shows how to create a two-column PDF using Java.

{{< gist aspose-com-gists 6bdeaa06a31c5d5a2532c34e9c23d110 "create-multicolumn-pdf.java" >}}

The following is the screenshot of the multi-column PDF generated by Aspose.PDF for Java.



{{< figure align=center src="images/Create-Multi-Column-PDF.jpg" alt="Create multi-column PDF Java">}}


## Get a Free License {#Get-a-Free-License}

You can use Aspose.PDF for Java without evaluation limitations using a [temporary license][26].

## Conclusion

Multi-column layout in PDF documents is used for various types of publications. In this post, you have learned how to create multi-column PDF files from scratch using Java. Besides, you can learn more about the Java PDF API using the [documentation][27]. In case you would have any questions, feel free to ask via our [forum][28].

## See Also

*   [Create PDF Files Programmatically using Java][29]




[1]: #API-to-Create-Multi-column-PDFs
[2]: #Create-a-Multi-column-PDF
[3]: https://products.aspose.com/pdf/java
[4]: https://downloads.aspose.com/pdf/java
[5]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-pdf
[6]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[7]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/MarginInfo#setLeft-double-
[8]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/MarginInfo#setRight-double-
[9]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/PageCollection#add--
[10]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Page
[11]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph
[12]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Paragraphs#add-com.aspose.pdf.BaseParagraph-
[13]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Line
[14]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph#getShapes--
[15]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Paragraphs#add-com.aspose.pdf.BaseParagraph-
[16]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/FloatingBox
[17]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph
[18]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Line
[19]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph#getShapes--
[20]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/FloatingBox#getParagraphs--
[21]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragment
[22]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/FloatingBox#getParagraphs--
[23]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/FloatingBox
[24]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Paragraphs#add-com.aspose.pdf.BaseParagraph-
[25]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[26]: https://purchase.aspose.com/temporary-license
[27]: https://docs.aspose.com/pdf/java
[28]: https://forum.aspose.com/
[29]: https://blog.aspose.com/2020/12/31/create-pdf-files-in-java/



