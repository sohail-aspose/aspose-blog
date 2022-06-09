---
title: 'Convert Word Documents to Markdown using Java'
seoTitle: "Convert Word to Markdown (.md) in Java | DOCX, DOC to MD in Java"
description: "Use Java Word API to convert MS Word documents to Markdown (.md) format in Java. Customize DOCX/DOC to MD conversion dynamically."
date: Mon, 01 Nov 2021 07:14:00 +0000
draft: false
url: /2021/11/01/convert-word-to-markdown-using-java/
author: Usman Aziz
summary: 'Nowadays, [Markdown][1] ([MD][2] format is widely opted to write online articles, blogs, and documentation. However, its syntax becomes difficult to remember and write in the case of large-sized documents. To make things easier, you can write content in MS Word and then convert [DOCX][3] or [DOC][4] file to Markdown. To perform this conversion programmatically, this article covers **how to convert Word documents to Markdown (.md) files using Java**.'
tags: ['convert doc to markdown in java', 'convert docx to markdown in java', 'convert word documents to markdown in java']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Word-to-Markdown.jpg" alt="Convert Word to Markdown in C#">}}


Nowadays, [Markdown][5] ([MD][6] format is widely opted to write online articles, blogs, and documentation. However, its syntax becomes difficult to remember and write in the case of large-sized documents. To make things easier, you can write content in MS Word and then convert [DOCX][7] or [DOC][8] file to Markdown. To perform this conversion programmatically, this article covers **how to convert Word documents to Markdown (.md) files using Java**.

*   [Word to Markdown Converter Library][9]
*   [Convert a Word Document to Markdown][10]
*   [Customize Word to Markdown Conversion][11]

## Java Word to Markdown Converter Library {#Word-to-Markdown-Converter-Library}

To convert DOCX/DOC files to Markdown format, we will use [Aspose.Words for Java][12]. The said API allows you to create and manipulate Word documents from within Java applications. Also, it provides a high-quality document converter to convert MS Word documents to other formats. You can [download][13] the API’s JAR or install it using the following Maven configurations.

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

## Convert a Word Document to Markdown in Java {#Convert-a-Word-Document-to-Markdown}

The following are the steps to convert a Word DOCX file to Markdown format in Java.

*   Load the Word file using [Document][14] class.
*   Convert Word file to Markdown format using [Document.save(string)][15] method.

The following code sample shows how to convert a DOCX file to Markdown format using Java.

{{< gist aspose-com-gists d3fee2edd09e40fc8e40c8aee4beab65 "word-to-markdown.java" >}}

## Customize Word to Markdown Conversion {#Customize-Word-to-Markdown-Conversion}

You can also change the default behavior of the API for Word to Markdown conversion. For example, you can set the alignment of the content in the tables, specify a folder to keep images, and so on. The following are the steps to set different options in Word to Markdown conversion.

*   Load the Word document using [Document][16] class.
*   Create an object of [MarkdownSaveOptions][17] class.
*   Set desired options such as [MarkdownSaveOptions.setImagesFolder(string)][18].
*   Convert Word document to Markdown using [Document.save(string, MarkdownSaveOptions)][19] method.

The following code sample shows how to customize DOCX to Markdown conversion using Java.

{{< gist aspose-com-gists d3fee2edd09e40fc8e40c8aee4beab65 "word-to-markdown-custom.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Words for Java without evaluation limitations using a [temporary license][20].

## Conclusion

In this article, you have learned how to convert Word DOCX/DOC files to Markdown (.md) programmatically in Java. Moreover, you have seen how to modify Word to Markdown conversion using different options. You can also explore other features offered by Aspose.Words for Java using the [documentation][21]. In addition, you can feel free to ask your questions via our [forum][22].

## See Also

*   [Create Word Documents without MS Office using Java][23]
*   [Convert PDF to Word in Java][24]
*   [Convert Word to PDF in Java][25]




[1]: https://en.wikipedia.org/wiki/Markdown
[2]: https://docs.fileformat.com/word-processing/md/)
[3]: https://docs.fileformat.com/word-processing/docx/
[4]: https://docs.fileformat.com/word-processing/doc/
[5]: https://en.wikipedia.org/wiki/Markdown
[6]: https://docs.fileformat.com/word-processing/md/)
[7]: https://docs.fileformat.com/word-processing/docx/
[8]: https://docs.fileformat.com/word-processing/doc/
[9]: #Word-to-Markdown-Converter-Library
[10]: #Convert-a-Word-Document-to-Markdown
[11]: #Customize-Word-to-Markdown-Conversion
[12]: https://products.aspose.com/words/java/
[13]: https://downloads.aspose.com/words/java/
[14]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[15]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String)
[16]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[17]: https://apireference.aspose.com/words/java/com.aspose.words/MarkdownSaveOptions
[18]: https://apireference.aspose.com/words/java/com.aspose.words/markdownsaveoptions#ImagesFolder
[19]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String,com.aspose.words.SaveOptions)
[20]: https://purchase.aspose.com/temporary-license
[21]: https://docs.aspose.com/words/java/
[22]: https://forum.aspose.com/
[23]: https://blog.aspose.com/2020/03/11/create-rich-word-documents-programmatically-in-java-using-java-word-api/
[24]: https://blog.aspose.com/2020/01/17/convert-pdf-to-word-doc-docx-in-java/
[25]: https://blog.aspose.com/2020/02/20/convert-word-doc-docx-to-pdf-in-java-programmatically/




