---
title: 'Convert Word DOC/DOCX to PDF in Java'
seoTitle: "Convert Word to PDF in Java | DOC to PDF or DOCX to PDF in Java"
description: "Convert Word DOC/DOCX to PDF in Java. Convert DOC to PDF or DOCX to PDF in Java. Convert popular formats of Word to PDF. Code examples and tutorials."
date: Thu, 20 Feb 2020 02:39:33 +0000
draft: false
url: /2020/02/20/convert-word-doc-docx-to-pdf-in-java-programmatically/
author: Usman Aziz
summary: ''
tags: ['Convert DOC DOCX to PDF in Java', 'DOC to PDF in Java', 'DOCX to PDF in Java', 'Word to PDF in Java']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Word-to-PDF-Conversion-C.png" alt="Convert Word to PDF in Java">}}


**Word to PDF** conversion is commonly used before the documents are shared. Various **online Word to PDF converters** are available that allow you to convert single or a limited number of Word documents. However, with emerging MS Word automation and report generation solutions, automated Word to PDF conversion has become an essential part of the systems. Furthermore, the **batch conversion of DOC/DOCX to PDF** needs to be done automatically to minimize the time and effort. Keeping an eye on such scenarios, I'll show you how to automate the process of converting **Word DOC or DOCX documents to PDF programmatically in Java**.

**Info**: Aspose provides a free online web app that allows you to [view PDFs online][1], another that allows you to [convert PDFs to video][2], and one that allows you to [edit PDFs online][3].

## Java Word to PDF Conversion Scenarios

You'll learn about the following Word (DOC/DOCX) to PDF conversions in this article.

*   [Convert Word to PDF in Java][4]
*   [Convert selected pages of a Word DOC/DOCX to PDF in Java][5]
*   [Convert Word to PDF with a specific PDF Standard such as PDF 1.5, PDF/A-1a, etc.][6]
*   [Convert Word to PDF with image/text compression in Java][7]
*   [Convert Word to PDF with the customized JPEG quality for images in Java][8]

## Java Word to PDF Conversion API

For converting Word DOCX/DOC to PDF, we'll use [Aspose.Words for Java][9] which is a powerful Word automation API for working with popular word processing formats. You can either [download][10] _Aspose.Words for Java_ or install it in your Maven-based application using the following configurations.

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
    <version>20.1</version>
    <classifier>jdk17</classifier>
</dependency>
```

## Convert Word DOC/DOCX to PDF in Java {#Convert-Word-to-PDF-in-Java}

In order to convert a Word document to PDF, you simply need to load the Word document and save it with ".pdf" extension. The following are the steps to convert DOCX/DOC to PDF in Java.

*   Load the Word document using [Document][11] class.
*   Save the document as PDF using [Document.save()][12] method.

The following code sample shows how to convert a Word DOC to PDF in Java.

{{< gist aspose-com-gists e4fd3d0d9a5efcbf9a85647f8b0e1740 "convert-word-to-pdf.java" >}}

### Word Document



{{< figure align=center src="images/Word-to-PDF-Conversion.png" alt="DOC DOCX to PDF in Java">}}


### PDF Document



{{< figure align=center src="images/Word-to-PDF-Conversion2.png" alt="DOCX to PDF">}}


## Convert Selected Pages of Word DOC/DOCX to PDF in Java {#Convert-selected-pages-of-a-Word-DOC/DOCX-to-PDF-in-Java}

In case you want to convert only selective pages of Word to PDF, You can do it using the [PdfSaveOptions][13] class. You can either convert the first N pages or a range of pages by specifying the starting page's index.

The following are the steps to convert selected pages of a Word DOCX/DOC to PDF in Java.

*   Load the Word document using [Document][14] class.
*   Create an instance of [PdfSaveOptions][15] class.
*   Set starting page's index and the number of pages to convert.
*   Save the Word document as PDF using [Document.save()][16] method.

The following code sample shows how to convert selected pages of Word DOC/DOCX to PDF in Java.

{{< gist aspose-com-gists e4fd3d0d9a5efcbf9a85647f8b0e1740 "convert-selected-pages-of-word-to-pdf.java" >}}

## Convert Word DOC/DOCX to Particular PDF Standard in Java {#Convert-Word-to-PDF-with-a-specific-PDF-Standard}

There exist various PDF standards a PDF document may compliant with, such as PDF/A-1a, PDF 1.5, etc. In case you want to convert Word document to a specific PDF standard, you can specify it using [PdfCompliance][17].

The following code sample shows how to convert Word DOCX to PDF with a particular PDF standard in Java.

{{< gist aspose-com-gists e4fd3d0d9a5efcbf9a85647f8b0e1740 "convert-word-to-pdf-compliance.java" >}}

## Convert Word to PDF with Text or Image Compression in Java {#Convert-Word-to-PDF-with-image/text-compression-in-Java}

You can also reduce the size of the resultant PDF document by compressing the text or image in the Word document. You can apply the following compressions in Word to PDF conversion using _Aspose.Words for Java_.

### Text Compression Options

_Aspose.Words for Java_ provides [PdfTextCompression][18] class with the following text compression options:

*   _None_: No text compression.
*   _Flate_: Flate (ZIP) compression.

### Image Compression

The image compression options are available in the [PdfImageCompression][19] class.

*   _Auto_: The most appropriate compression for every image is selected automatically.
*   _Jpeg_: Images are converted to JPEG format (does not support transparency).

The following code sample shows how to convert Word DOCX to PDF by applying text and image compression in Java.

{{< gist aspose-com-gists e4fd3d0d9a5efcbf9a85647f8b0e1740 "convert-word-to-pdf-compression.java" >}}

## Convert Word to PDF with JPEG Quality in Java {#Convert-Word-to-PDF-with-the-customized-JPEG-quality}

You can also customize and control the JPEG quality in Word to PDF conversion. The [PdfSaveOptions.setJpegQuality][20] is used to set JPEG quality which can be from 0 (_worst quality with maximum compression_) to 100 (_best quality with minimum compression_).

The following code sample shows how to specify JPEG quality while converting Word DOCX to PDF in Java.

{{< gist aspose-com-gists e4fd3d0d9a5efcbf9a85647f8b0e1740 "convert-word-to-pdf-JPEG-quality.java" >}}

## Try Aspose.Words for Java for Free

You can get a [free temporary license][21] to try and use _Aspose.Words for Java_.

**Info**: You may be interested in another Java API, especially one that allows developers and applications to convert PowerPoint to PDF –[ Aspose.Slides for Python][22]. And you might also want to check out Aspose [PowerPoint to PDF Converter][23] because it is a live implementation of the PowerPoint document to PDF process.

## Conclusion

In this article, you have learned how to convert Word DOCX or DOC to PDF using Java. Furthermore, you have seen how to customize the Word to PDF conversion in different scenarios. You can explore more about Aspose.Words for Java using the [documentation][24].

## Related Articles

*   [Convert Word DOC/DOCX to PDF in C#][25]
*   [Convert PDF to Excel in C#][26]
*   [Convert PDF to MS Word Documents in Java][27]
*   [Convert Word to Markdown in Java][28]
*   [Word to EPUB Conversion in Java][29]
*   [HTML to Word Conversion in Java][30]
*   [Convert TXT Files to PDF in Java][31]




[1]: https://products.aspose.app/slides/viewer/pdf
[2]: https://products.aspose.app/slides/video/pdf
[3]: https://products.aspose.app/slides/editor/pdf
[4]: #Convert-Word-to-PDF-in-Java
[5]: #Convert-selected-pages-of-a-Word-DOC/DOCX-to-PDF-in-Java
[6]: #Convert-Word-to-PDF-with-a-specific-PDF-Standard
[7]: #Convert-Word-to-PDF-with-image/text-compression-in-Java
[8]: #Convert-Word-to-PDF-with-the-customized-JPEG-quality
[9]: https://products.aspose.com/words/java
[10]: https://downloads.aspose.com/words/java
[11]: https://apireference.aspose.com/java/words/com.aspose.words/document
[12]: https://apireference.aspose.com/java/words/com.aspose.words/document#save(java.lang.String)
[13]: https://apireference.aspose.com/java/words/com.aspose.words/PdfSaveOptions
[14]: https://apireference.aspose.com/java/words/com.aspose.words/document
[15]: https://apireference.aspose.com/java/words/com.aspose.words/PdfSaveOptions
[16]: https://apireference.aspose.com/java/words/com.aspose.words/document#save(java.lang.String)
[17]: https://apireference.aspose.com/java/words/com.aspose.words/PdfCompliance
[18]: https://apireference.aspose.com/java/words/com.aspose.words/PdfTextCompression
[19]: https://apireference.aspose.com/java/words/com.aspose.words/PdfImageCompression
[20]: https://apireference.aspose.com/java/words/com.aspose.words/pdfsaveoptions#JpegQuality
[21]: https://purchase.aspose.com/temporary-license
[22]: https://products.aspose.com/slides/java
[23]: https://products.aspose.app/slides/conversion
[24]: https://docs.aspose.com/words/java/
[25]: https://blog.aspose.com/2020/01/02/convert-word-doc-docx-to-pdf-in-csharp-net-core/
[26]: https://blog.aspose.com/2020/01/03/convert-pdf-to-excel-in-csharp-net-pdf-to-xls-pdf-to-xlsx/
[27]: https://blog.aspose.com/2020/01/17/convert-pdf-to-word-doc-docx-in-java/
[28]: https://blog.aspose.com/2021/11/01/convert-word-to-markdown-using-java/
[29]: https://blog.aspose.com/2021/11/01/convert-word-to-epub-in-java/
[30]: https://blog.aspose.com/2021/11/29/convert-html-to-word-in-java/
[31]: https://blog.aspose.com/2021/11/01/convert-txt-to-pdf-in-java/





