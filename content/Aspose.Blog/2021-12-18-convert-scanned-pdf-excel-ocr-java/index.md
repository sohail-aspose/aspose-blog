---
title: 'Create Scanned PDF to Excel Converter with OCR in Java'
seoTitle: "Create Scanned PDF to Excel Converter with OCR in Java"
description: "You can create Scanned PDF to Excel file with OCR programmatically using Java. Convert scanned PDF to XLSX or XLS in Java."
date: Sat, 18 Dec 2021 09:58:00 +0000
draft: false
url: /2021/12/18/convert-scanned-pdf-excel-ocr-java/
author: Farhan Raza
summary: 'Scanned PDF files comprise data in image format because they are often created by scanners. In certain situations, you may require numerical information from a scanned PDF file. So you can perform OCR operations for creating an Excel file. This article covers how to **create a scanned PDF to Excel converter with OCR feature programmatically in Java.**'
tags: ['Convert Scanned PDF to Excel OCR Java', 'Java Scanned PDF to Excel OCR', 'Scanned PDF to Excel', 'Scanned PDF to Excel OCR', 'Scanned PDF to Excel in Java']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/Scanned-PDF-to-Excel-OCR-1.jpg" alt="Scanned PDF to Excel OCR Java">}}


Scanned [PDF][1] files comprise data in image format because they are often created by scanners. In certain situations, you may require numerical information from a scanned PDF file. So you can perform OCR operations for creating an Excel file. This article covers how to create a scanned PDF to Excel converter with OCR feature programmatically in Java.

*   [Create Scanned PDF to Excel Converter with OCR – Java API Installation][2]
*   [Convert Scanned PDF to Excel Programmatically in Java][3]

## Create Scanned PDF to Excel Converter with OCR – Java API Installation {#section1}

You can optically recognize the text in a PDF file with the OCR feature using [Aspose.OCR for Java][4] API. Simply install the API by downloading the JAR file from the [New Releases][5] section, or using the Maven specifications below:

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
    <version>21.12</version>
</dependency>
```

## Convert Scanned PDF to Excel Programmatically in Java {#section2}

You can convert a scanned PDF file to Excel with OCR by following the steps below:

1.  Create a [AsposeOcr][6] class object.
2.  Specify the settings with [DocumentRecognitionSettings][7] class.
3.  Recognize the scanned PDF file using [RecognizePdf][8] method.
4.  Save output OCR result as an Excel file.

The following code snippet elaborates how to convert a scanned PDF to an Excel file programmatically in Java:

{{< gist aspose-com-gists f0cfe4eef8e1f4dfee3b9a8c2b825218 "Scanned-PDF-to-Excel-Java.java" >}}

## Get Free Evaluation License

You can evaluate the API for creating scanned PDF to Excel converter by OCR operations without any limitations by requesting a [free temporary license][9].

## Conclusion

In this article, you have understood how to convert a scanned PDF file to an Excel file with the OCR feature programmatically in Java. Moreover, please take a look at other OCR-related features by visiting the [documentation][10]. Feel free to write to us at the [forum][11] in case of any concerns.

## See Also

[Convert Image to Searchable Word Document (DOC/DOCX) using Java][12]




[1]: https://docs.fileformat.com/pdf/
[2]: #section1
[3]: #section2
[4]: https://products.aspose.com/ocr/java
[5]: https://downloads.aspose.com/ocr/java
[6]: https://apireference.aspose.com/ocr/java/com.aspose.ocr/asposeocr
[7]: https://apireference.aspose.com/ocr/java/com.aspose.ocr/documentrecognitionsettings
[8]: https://apireference.aspose.com/ocr/java/com.aspose.ocr.pdf/AsposeOCRPdf#RecognizePdf-java.lang.String-com.aspose.ocr.DocumentRecognitionSettings-
[9]: https://purchase.aspose.com/temporary-license
[10]: https://docs.aspose.com/ocr/java/
[11]: https://forum.aspose.com/c/ocr/16
[12]: https://blog.aspose.com/2021/06/22/convert-image-searchable-word-docx-java/




