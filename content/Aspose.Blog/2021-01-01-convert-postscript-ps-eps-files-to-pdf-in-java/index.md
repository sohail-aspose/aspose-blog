---
title: 'Convert PostScript PS or EPS Files to PDF in Java'
seoTitle: "Convert PostScript EPS PS to PDF in Java | PS to PDF and EPS to PDF"
description: "Convert EPS or PS files to PDF using Java. Convert PS to PDF or EPS to PDF with high fidelity using Aspose.Page for Java API."
date: Fri, 01 Jan 2021 02:06:00 +0000
draft: false
url: /2021/01/01/convert-postscript-ps-eps-files-to-pdf-in-java/
author: Usman Aziz
summary: 'The PostScript (PS) file format is mainly used for printing purposes. A PS file is saved in page description language and can contain text, vector graphics, and raster images. On the other hand, the Encapsulated PostScript (EPS) format is used for images or drawings. In certain cases, you may need to convert a PS or EPS file to PDF format. Therefore, this article covers how to perform this conversion programmatically. Particularly, you will learn how to convert **PS/EPS files into PDF** **using Java**.'
tags: ['EPS to PDF java', 'PS to PDF in Java']
categories: ['Aspose.Page Product Family']
---



{{< figure align=center src="images/aspose_page-for-java.png" alt="eps or ps to pdf java">}}


The PostScript (PS) file format is mainly used for printing purposes. A PS file is saved in page description language and can contain text, vector graphics, and raster images. On the other hand, the Encapsulated PostScript (EPS) format is used for images or drawings. In certain cases, you may need to convert a PS or EPS file to PDF format. Therefore, this article covers how to perform this conversion programmatically. Particularly, you will learn how to convert **PS and EPS files to PDF** **using Java**.

*   [PS/EPS to PDF Converter API][1]
*   [Steps to Convert PS/EPS to PDF][2]
*   [Code Sample][3]

## Java PS or EPS to PDF Converter API {#Java-PS-EPS-to-PDF-Converter-API}

[Aspose.Page for Java][4] API is designed to work with PS and EPS files from within the Java applications. Along with other manipulation features, the API provides a high fidelity conversion of PS/EPS to PDF. You can either [download][5] the API's JAR or install it within your Maven-based application.

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
    <artifactId>aspose-page</artifactId>
    <version>20.12</version>
</dependency>
```

## Steps to Convert PS or EPS to PDF in Java {#Steps-to-Convert-PS-EPS-to-PDF-in-Java}

The following are the steps to convert a PS or EPS file to PDF using Aspose.Page.

*   Load the file using the [PsDocument][6] class.
*   Create an instance of [PdfSaveOptions][7] class and set PDF options if required.
*   Define an instance of [FileOutputStream][8] for output PDF file.
*   Create an instance of [PdfDevice][9] class and initialize it with output PDF's FileOutputStream object.
*   Save document as PDF using [PsDocument.save(PdfDevice, PdfSaveOptions)][10] method.

## Code Sample {#Code-Sample}

The following code sample shows how to convert an EPS or PS to PDF using Java.

{{< gist aspose-com-gists bcee4811da013bc7a78dd41af768a9d2 "Examples-src-main-java-com-aspose-page-conversion-PostScriptToPDF-PostScriptToPDF.java" >}}

## Conclusion

In this article, you have learned how to convert EPS or PS files to PDF using Java. You can explore more about the EPS or PS file manipulation API using the [documentation][11].

## See Also

*   [Convert XPS to BMP, JPEG, PNG, and TIFF using Java][12]




[1]: #Java-PS-EPS-to-PDF-Converter-API
[2]: #Steps-to-Convert-PS-EPS-to-PDF-in-Java
[3]: #Code-Sample
[4]: https://products.aspose.com/page/java
[5]: https://downloads.aspose.com/page/java
[6]: https://apireference.aspose.com/page/java/com.aspose.eps/PsDocument
[7]: https://apireference.aspose.com/page/java/com.aspose.eps.device/PdfSaveOptions
[8]: https://docs.oracle.com/javase/7/docs/api/java/io/FileOutputStream.html
[9]: https://apireference.aspose.com/page/java/com.aspose.eps.device/PdfDevice
[10]: https://apireference.aspose.com/page/java/com.aspose.eps/PsDocument#save-com.aspose.page.Device-com.aspose.page.SaveOptions-
[11]: https://docs.aspose.com/page/java/developer-guide/
[12]: https://blog.aspose.com/2020/12/18/convert-xps-to-bmp-jpeg-png-and-tiff-using-java/





