---
title: 'Convert PDF to SVG Format using Java'
seoTitle: ""
description: ""
date: Wed, 04 Nov 2020 22:24:49 +0000
draft: false
url: /2020/11/04/convert-pdf-to-svg-using-java/
author: Usman Aziz
summary: '[PDF][1] has been ruling the world of digital document formats for many years for printing, sharing, exchanging, and archiving the documents. However, PDF may not be suitable in certain situations such as displaying it on a web page. In such cases, [SVG][2] comes as an alternative. SVG files can easily be displayed on the web pages without disturbing the user experience across the diversity of screen sizes. Hence, PDF to SVG conversion takes place in such cases. In this article, you are going to learn **how to convert the PDF files to SVG format using Java**.'
tags: ['Convert PDF to SVG in Java', 'Java PDF to SVG Converter', 'PDF to SVG in Java']
categories: ['Aspose.PDF Product Family']
---

[PDF][3] has been ruling the world of digital document formats for many years for printing, sharing, exchanging, and archiving documents. However, PDF may not be suitable in certain situations such as displaying it on a web page as it requires browser support or additional plugins. In such cases, [SVG][4] comes as an alternative. SVG files can easily be displayed on the web pages without disturbing the user experience because of its screen resolution independence. Hence, PDF to SVG conversion takes place in such cases. In this article, you are going to learn **how to convert the PDF files to SVG format using [Java][5]**.

*   [Java PDF to SVG Converter API - Free Download][6]
*   [PDF to SVG Conversion][7]
*   [Convert PDF to SVG with Additional Options][8]

## Java PDF to SVG Converter API - Free Download {#PDF-to-SVG-Java-API-Free-Download}

[Aspose.PDF for Java][9] is a PDF manipulation API that has a built-in PDF converter. The API lets you convert the PDF documents into SVG format with high accuracy. You can either [download][10] the API or get it installed within your Java applications using the following Maven configurations.

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
    <artifactId>aspose-pdf</artifactId>
    <classifier>jdk17</classifier>
</dependency>
```

## PDF to SVG Java Conversion {#PDF-to-SVG-Java-Conversion}

The following are the steps to convert a PDF file to SVG format using Aspose.PDF for Java.

*   Load the PDF file using the [Document][11] class.
*   Create an object of the [SvgSaveOptions][12] class.
*   Save the PDF as SVG using [Document.save(String, SvgSaveOptions)][13] method.

The following code sample shows how to convert a PDF to SVG using Java.

{{< gist aspose-com-gists 0a483b70ef3cc1336638c35e482745d7 "pdf-to-svg.java" >}}

## Convert PDF to SVG with Additional Options {#Convert-PDF-to-SVG-with-Additional-Options}

Aspose.PDF also provides some additional options to customize the PDF to SVG conversion. The [SvgSaveOptions][14] class lets you accomplish this using the following options.

*   [CompressOutputToZipArchive][15]
*   [CustomStrategyOfEmbeddedImagesSaving][16]
*   [ScaleToPixels][17]
*   [TreatTargetFileNameAsDirectory][18]

The following are the steps to convert PDF to SVG with additional options.

*   Load the PDF file using the [Document][19] class.
*   Create an object of the [SvgSaveOptions][20] class.
*   Set the desired SVG option such as [CompressOutputToZipArchive][21].
*   Save the PDF as SVG using [Document.save(String, SvgSaveOptions)][22] method.

The following code sample shows how to perform a customized PDF to SVG conversion.

{{< gist aspose-com-gists 0a483b70ef3cc1336638c35e482745d7 "pdf-to-svg-custom.java" >}}

## Conclusion

In this article, you have seen how to convert PDF files to SVG using Java. The code samples have also demonstrated the customized conversion with additional options. You can explore more about the Java PDF API using the [documentation][23].

## See Also

*   [Convert PDF to DOCX in Java][24]




[1]: void(0)
[2]: https://docs.fileformat.com/page-description-language/svg/
[3]: https://docs.fileformat.com/pdf/
[4]: https://docs.fileformat.com/page-description-language/svg/
[5]: https://docs.fileformat.com/programming/java/
[6]: #PDF-to-SVG-Java-API-Free-Download
[7]: #PDF-to-SVG-Java-Conversion
[8]: #Convert-PDF-to-SVG-with-Additional-Options
[9]: https://products.aspose.com/pdf/java
[10]: https://downloads.aspose.com/pdf/java
[11]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/Document
[12]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/SvgSaveOptions
[13]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-com.aspose.pdf.SaveOptions-
[14]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/SvgSaveOptions
[15]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/SvgSaveOptions#CompressOutputToZipArchive
[16]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/SvgSaveOptions#CustomStrategyOfEmbeddedImagesSaving
[17]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/SvgSaveOptions#ScaleToPixels
[18]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/SvgSaveOptions#TreatTargetFileNameAsDirectory
[19]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/Document
[20]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/SvgSaveOptions
[21]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/SvgSaveOptions#CompressOutputToZipArchive
[22]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-com.aspose.pdf.SaveOptions-
[23]: https://docs.aspose.com/pdf/java/
[24]: https://blog.aspose.com/2020/01/17/convert-pdf-to-word-doc-docx-in-java/





