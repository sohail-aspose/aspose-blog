---
title: 'Convert Image to Excel with OCR in Java'
seoTitle: "Convert Image to Excel with OCR Programmatically in Java"
description: "Convert Image to Excel XLSX or XLS file programmatically in Java. Export JPG, PNG, TIFF, or BMP to Excel with OCR using Java."
date: Sun, 26 Dec 2021 10:18:00 +0000
draft: false
url: /2021/12/26/image-to-excel-ocr-java/
author: Farhan Raza
summary: 'You can **convert an image to an Excel file with optical character recognition programmatically in Java**. You can load the input image from the disk or URI address and then recognize text to create XLSX or XLS file.'
tags: ['Convert Image to Excel', 'Image to Excel', 'Image to Excel in Java', 'Image to XLSX', 'JPG to Excel', 'Java PNG to Excel', 'PNG to Excel', 'Picture to Excel']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/Image-to-Excel-OCR.jpg" alt="Image to Excel OCR Java">}}


You can convert an image to an Excel file with optical character recognition programmatically in Java. You can load the input image from the disk or URI address and then recognize text to create XLSX or XLS file.

*   [Image to Excel Converter – Java API Installation][1]
*   [Convert Image to Excel with OCR using Java][2]
*   [Convert Online Image using URI to Excel with OCR in Java][3]

## Image to Excel Converter – Java API Installation {#section1}

You can convert images to Excel using [Aspose.OCR for Java][4] API. Load an input file as JPG, PNG, BMP, or other formats and recognize the text for saving the output Excel file. Please download the JAR file from [New Releases][5] or use the below configurations in the pom.xml file of your Maven-based project:

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

## Convert Image to Excel with OCR using Java {#section2}

You can convert an image to an Excel file with the following steps:

1.  Initialize an instance of [AsposeOcr][6] class.
2.  Create an instance of [RecognitionSettings][7] class object.
3.  Recognize the input image with [RecognizePage][8] method.
4.  Finally, save the output as an Excel file.

The following code demonstrates how to convert an image to an Excel file using Java:

{{< gist aspose-com-gists 55d48e68f63e416b1c7882a7c832758e "OCRImagetoExceljava.java" >}}

## Convert Online Image using URI to Excel with OCR in Java {#section3}

You can convert an online image to an Excel file with the OCR feature by following the steps below:

1.  Firstly, create an object of [AsposeOcr][9] class.
2.  Initialize an instance of [RecognitionSettings][10] class.
3.  Recognize image with OCR using the [RecognizePage][11] method.
4.  Save the output file in XLSX or XLS format.

The following code snippet explains how to convert an online image with OCR in Java:

{{< gist aspose-com-gists 55d48e68f63e416b1c7882a7c832758e "OCRuriToExcelJava.java" >}}

## Get Free API License

You can evaluate the API features in full capacity by requesting a [free temporary license][12].

## Conclusion

In this article, you have learned how to convert an image from a local file or from an online URI to an Excel file with OCR programmatically in Java. You can automate this process for recognizing multiple images from a folder as well as using parallel processing as per your requirements. Please visit the [documentation][13] to explore other features. Moreover, please feel free to get in touch with us at the [forum][14].

## See Also

[Convert Scanned PDF to Searchable PDF with OCR in Java][15]




[1]: #section1
[2]: #section2
[3]: #section3
[4]: https://products.aspose.com/ocr/java
[5]: https://downloads.aspose.com/ocr/java
[6]: https://apireference.aspose.com/ocr/java/com.aspose.ocr/AsposeOCR
[7]: https://apireference.aspose.com/ocr/java/com.aspose.ocr/RecognitionSettings
[8]: https://apireference.aspose.com/ocr/java/com.aspose.ocr/AsposeOCR#RecognizePage-java.lang.String-
[9]: https://apireference.aspose.com/ocr/java/com.aspose.ocr/AsposeOCR
[10]: https://apireference.aspose.com/ocr/java/com.aspose.ocr/RecognitionSettings
[11]: https://apireference.aspose.com/ocr/java/com.aspose.ocr/AsposeOCR#RecognizePage-java.lang.String-
[12]: https://purchase.aspose.com/temporary-license
[13]: https://docs.aspose.com/ocr/java/
[14]: https://forum.aspose.com/c/ocr
[15]: https://blog.aspose.com/2021/12/13/convert-scanned-pdf-searchable-ocr-java/




