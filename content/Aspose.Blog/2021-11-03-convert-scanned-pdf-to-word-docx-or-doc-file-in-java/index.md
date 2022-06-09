---
title: 'Convert Scanned PDF to Word DOCX or DOC File in Java'
seoTitle: "Convert Scanned PDF to Word DOCX or DOC File in Java"
description: "Convert Scanned PDF to Word DOCX file programmatically in Java. Export scanned PDF document to Microsoft Word document using Java."
date: Wed, 03 Nov 2021 19:23:00 +0000
draft: false
url: /2021/11/03/convert-scanned-pdf-to-word-docx-or-doc-file-in-java/
author: Farhan Raza
summary: 'The PDF files created using a camera or scanner device contain scanned images. Such images cannot be processed for text selection or editing so you might need to convert scanned PDF to Word documents in DOCX or DOC format. This article covers how to **convert a scanned PDF file to a Word file programmatically using Java.**'
tags: ['PDF to Word OCR in Java', 'Scanned PDF to DOCX in Java', 'Scanned PDF to Word in Java']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/Scanned-PDF-to-Word-OCR.jpg" alt="Scanned PDF to Word Java OCR">}}


The [PDF][1] files created using a camera or scanner device contain scanned images. Such images cannot be processed for text selection or editing so you might need to convert scanned PDF to Word documents in [DOCX][2] or [DOC][3] format. This article covers how to convert a scanned PDF file to a Word file programmatically using Java.

*   [Java API to Convert Scanned PDF to Word File][4]
*   [Convert Scanned PDF to Word Document Programmatically using Java][5]

## Java API to Convert Scanned PDF to Word File {#section1}

You can manipulate scanned PDF documents with OCR operations using [Aspose.OCR for Java][6] API and then generate a Word file with [Aspose.Words for Java][7] API programmatically. Simply set up the APIs by downloading the JAR files from the [Downloads][8] section or using the following Maven specifications:

### Repository```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>
```

### Dependency```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-ocr</artifactId>
    <version>21.11</version>
    <artifactId>aspose-words</artifactId>
    <version>21.12</version>
</dependency>
```

## Convert Scanned PDF to Word Document Programmatically using Java {#section2}

You can convert a scanned PDF file to a Word document with optical character recognition technique. This is a two-step process where the scanned PDF is converted to text and then the text is converted to a Word document in DOC or DOCX format. You need to follow the steps below to convert scanned PDF to a Word document:

1.  Instantiate [AsposeOCRPdf][9] class object.
2.  Recognize images from PDF file using [DocumentRecognitionSettings][10] type object.
3.  Specify [String][11] class object and save the text.
4.  Initialize a new word document with the [Document][12] class.
5.  Set the fonts and paragraphs formatting.
6.  Finally, write the output Word document to disk as DOCX or DOC file.

The code snippet below demonstrates how to convert a scanned PDF file to a Word document as DOC or DOCX file programmatically using Java:

{{< gist aspose-com-gists 9d704265104be1331925e9461911734b "Convert-Scanned-PDF-to-Word.java" >}}

## Get Free Temporary License

You can evaluate the APIs without any limitations by requesting a [free temporary license][13].

**Info**: You may be interested in another Java API ([Aspose.Slides for Java][14] that allows you to convert presentations (into PDFs, [word documents][15], etc.) and [import images][16] or other documents into presentations.

## Conclusion

In this article, you have explored how to convert a scanned PDF file to a Word document as DOCX or DOC file programmatically using Java. Furthermore, you can take a look at other OCR-related features by visiting the [documentation][17]. In case of any concerns, please feel free to contact us at the [forum][18].

## See Also

[Convert Image to Searchable Word Document (DOC/DOCX) using Java][19]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/word-processing/docx/
[3]: https://docs.fileformat.com/word-processing/doc/
[4]: #section1
[5]: #section2
[6]: https://products.aspose.com/ocr/java
[7]: https://products.aspose.com/words/java
[8]: https://downloads.aspose.com/
[9]: https://apireference.aspose.com/ocr/java/com.aspose.ocr.pdf/AsposeOCRPdf
[10]: https://apireference.aspose.com/ocr/java/com.aspose.ocr/DocumentRecognitionSettings
[11]: https://docs.oracle.com/en/java/javase/11/docs/api/java.base/java/lang/String.html
[12]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[13]: https://purchase.aspose.com/temporary-license
[14]: https://products.aspose.com/slides/java/)
[15]: https://products.aspose.app/slides/conversion/ppt-to-word
[16]: https://products.aspose.app/slides/import/jpg-to-ppt
[17]: https://docs.aspose.com/ocr/java/
[18]: https://forum.aspose.com/c/ocr/16
[19]: https://blog.aspose.com/2021/06/22/convert-image-searchable-word-docx-java/




