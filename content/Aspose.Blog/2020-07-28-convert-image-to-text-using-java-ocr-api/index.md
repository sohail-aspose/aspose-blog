---
title: 'Convert Image to Text using Java OCR API'
seoTitle: ""
description: ""
date: Tue, 28 Jul 2020 22:19:00 +0000
draft: false
url: /2020/07/28/convert-image-to-text-using-java-ocr-api/
author: Usman Aziz
summary: ''
tags: ['Java OCR API', 'convert image to text in java', 'perform ocr on image using java', 'perform ocr on png jpg bmp gif using java']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/Perform-OCR-using-C.jpg" alt="Perform OCR using Java">}}


The [Optical Character Recognition][1] (OCR) technology has made it possible to recognize and read the text within the scanned documents and images. OCR lets you convert the read-only text into an editable form. The converted text can further be processed for operations such as text analysis. In this article, I'll show you how to perform OCR on images ([PNG][2], [JPG][3], [BMP][4], and [GIF][5] and convert images to text using Java OCR API - [Aspose.OCR for Java][6].

*   [Java OCR API - Installation][7]
*   [Convert Image to Text using Java][8]
*   [Convert Images having Single Line of Text using Java][9]

**TIP**: You may be interested in a free [Text to GIF Converter][10] that allows you to generate animations from texts.

## Java OCR API - Installation {#Java-OCR-API-Installation}

Aspose.OCR for Java can be downloaded as a [JAR][11] or installed within a Maven-based application using the following configurations.

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
    <version>20.5</version>
</dependency>
```

## Convert Image to Text using Java {#Convert-Image-to-Text-using-Java}

Most often, the images for OCR are the pages of scanned documents, invoices, receipts, bills and etc. where the text is composed of multiple lines. In such scenarios, you need to retrieve the whole text from the image. The following are the steps to perform OCR on the image having multiple lines of text using Aspose.OCR for Java.

*   Create an instance of the [AsposeOcr][12] class.
*   Convert image to text using [AsposeOcr.recognizePage(String fullPath)][13] method by passing the image’s path.
*   Get the converted text into a string object.

The following code sample shows how to perform OCR on image and convert image to text using Java.

{{< gist aspose-com-gists 3830491066e58e54903b3025d04e5b0c "Examples-src-main-java-com-aspose-ocr-examples-OcrFeatures-PerformOCROnPage-1.java" >}}

## Convert Images having Single Line of Text {#Convert-Images-having-Single-Line-of-Text-using-Java}

In the previous example, we have performed OCR on an image having multiple lines of text. However, there could be a case when the image contains a single line of text. For such a case, you can configure the API accordingly. The following are the steps to convert an image having a single line of text.

*   Create an object of the [AsposeOcr][14] class.
*   Convert image to text using [AsposeOcr.recognizeLine(String fullPath)][15] method.
*   Get the result into a string object.

The following code sample shows how to perform OCR on an image having a single line of text using Java.

{{< gist aspose-com-gists 3830491066e58e54903b3025d04e5b0c "Examples-src-main-java-com-aspose-ocr-examples-OcrFeatures-RecognizeLine-1.java" >}}

## Conclusion

In this article, you have seen how to convert PNG, JPG, BMP, and GIF images to text using Java OCR API. The code samples show how to perform OCR on images having single or multiple lines of text within Java applications. You can learn more about Aspose's Java OCR API using [documentation][16].

## See Also

*   [Convert Image to Text using C#][17]
*   [Convert Image to Text using C++][18]




[1]: https://en.wikipedia.org/wiki/Optical_character_recognition
[2]: https://docs.fileformat.com/image/png/
[3]: https://docs.fileformat.com/image/jpeg/
[4]: https://docs.fileformat.com/image/bmp/
[5]: https://docs.fileformat.com/image/gif/)
[6]: https://products.aspose.com/ocr/java
[7]: #Java-OCR-API-Installation
[8]: #Convert-Image-to-Text-using-Java
[9]: #Convert-Images-having-Single-Line-of-Text-using-Java
[10]: https://products.aspose.app/slides/text-to-gif
[11]: https://downloads.aspose.com/ocr/java
[12]: https://apireference.aspose.com/ocr/java/com.aspose.ocr/AsposeOCR
[13]: https://apireference.aspose.com/ocr/java/com.aspose.ocr/AsposeOCR#RecognizePage-java.lang.String-
[14]: https://apireference.aspose.com/ocr/java/com.aspose.ocr/AsposeOCR
[15]: https://apireference.aspose.com/ocr/java/com.aspose.ocr/AsposeOCR#RecognizeLine-java.lang.String-
[16]: https://docs.aspose.com/display/OCRJAVA/Product+Overview
[17]: https://blog.aspose.com/2020/05/28/perform-ocr-on-images-and-scanned-documents-using-csharp-vb.net/
[18]: https://blog.aspose.com/2020/06/23/convert-image-to-text-using-cpp-ocr-library/





