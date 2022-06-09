---
title: 'Convert TXT Files to PDF in Java'
seoTitle: "Convert TXT to PDF in Java | Convert Notepad File to PDF in Java"
description: "Use Java Word library to convert Notepad's TXT files to PDF in Java. Java code sample to automate the conversion of TXT files to PDF."
date: Mon, 01 Nov 2021 14:56:00 +0000
draft: false
url: /2021/11/01/convert-txt-to-pdf-in-java/
author: Usman Aziz
summary: 'Notepad is the easiest tool to write down the important points and create quick notes in a [TXT][1] file. Since TXT files do not support advanced features, such as comments, etc., they are converted to [PDF][2] format. To perform this conversion programmatically, this article covers **how to convert TXT files to PDF format using Java**.'
tags: ['convert notepad files to pdf in java', 'convert txt to pdf in java', 'java txt to pdf converter library']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Convert-TXT-file-to-PDF.jpg" alt="Convert Notepad TXT file to PDF in Java">}}


Notepad is the easiest tool to write down the important points and create quick notes in a [TXT][3] file. Since TXT files do not support advanced features, such as comments, etc., they are converted to [PDF][4] format. To perform this conversion programmatically, this article covers **how to convert TXT files to PDF format using Java**.

*   [Java Library for TXT to PDF Conversion][5]
*   [Convert a TXT File to PDF][6]

## Java Library for TXT to PDF Conversion {#Library-for-TXT-to-PDF-Conversion}

In order to render TXT files as PDF, we will use [Aspose.Words for Java][7]. It is a popular library to create and manipulate word processing documents. Also, it provides high-quality conversion of Word documents and plain text files to other formats. You can [download][8] the API’s JAR or install it using the following Maven configuration.

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

## Convert a TXT File to PDF in Java {#Convert-a-TXT-File-to-PDF-in-Python}

The conversion of a TXT file to PDF format is extremely easy using Aspose.Words. Just load the TXT file and save it as a PDF document to your desired location. The following are the steps to convert a TXT file to PDF in Java.

*   Load TXT file using [Document][9] class.
*   Convert TXT file to PDF using [Document.save(string, SaveFormat)][10] method.

The following code sample shows how to convert a TXT file to PDF format.

{{< gist aspose-com-gists 98fced2b4280ef0b9f1373ba801c0746 "txt-to-pdf.java" >}}

The following screenshot shows the converted PDF file.



{{< figure align=center src="images/Convert-TXT-files-to-PDF.jpg" alt="Convert TXT files to PDF programmatically using Java" caption="Converted PDF File">}}


## Get a Free API License {#Get-a-Free-API-License}

You can get a [temporary license][11] to use Aspose.Words for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to convert TXT files to PDF format in Java. You can simply install Aspose.Words for Java and automate TXT to PDF conversion in your applications. You can explore more about Aspose.Words for Java using the [documentation][12]. Also, you can post your queries or questions to our [forum][13].

## See Also

*   [Create Word Documents without MS Office using Java][14]
*   [Convert PDF to Word in Java][15]
*   [Convert Word to PDF in Java][16]




[1]: https://docs.fileformat.com/word-processing/txt/
[2]: https://docs.fileformat.com/pdf/
[3]: https://docs.fileformat.com/word-processing/txt/
[4]: https://docs.fileformat.com/pdf/
[5]: #Library-for-TXT-to-PDF-Conversion
[6]: #Convert-a-TXT-File-to-PDF-in-Python
[7]: https://products.aspose.com/words/java/
[8]: https://downloads.aspose.com/words/java/
[9]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[10]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String,int)
[11]: https://purchase.aspose.com/temporary-license
[12]: https://docs.aspose.com/words/java/
[13]: https://forum.aspose.com/
[14]: https://blog.aspose.com/2020/03/11/create-rich-word-documents-programmatically-in-java-using-java-word-api/
[15]: https://blog.aspose.com/2020/01/17/convert-pdf-to-word-doc-docx-in-java/
[16]: https://blog.aspose.com/2020/02/20/convert-word-doc-docx-to-pdf-in-java-programmatically/




