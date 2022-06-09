---
title: 'Convert OXPS or XPS to PDF Programmatically with Java'
seoTitle: "Java Convert OXPS XPS to PDF Programmatically | Export Render XPS"
description: "Convert XPS or OXPS to PDF Document Programmatically using Java language. Render or export XPS OXPS files with quick and easy examples."
date: Tue, 09 Feb 2021 15:18:41 +0000
draft: false
url: /2021/02/09/convert-oxps-xps-pdf-java/
author: Farhan Raza
summary: '[**XPS**][1] is a fixed-document format often used to organize information for printing purposes. Likewise, [**OXPS**][2] files are also based on XML paper Specifications. You can easily convert XPS or OXPS files to PDF documents programmatically using Java language.'
tags: ['Convert XPS to PDF', 'OXPS to PDF in Java', 'XPS to PDF in Java', 'convert oxps to pdf', 'oxps to pdf']
categories: ['Aspose.Page Product Family']
---



{{< figure align=center src="images/XPS-to-PDF-Conversion-1.png" alt="Convert XPS OXPS to PDF Java">}}


[XPS][3] is a fixed-document format often used to organize information for printing purposes. Likewise, [OXPS][4] files are also based on XML paper Specifications. You can easily convert XPS or OXPS files to PDF documents programmatically using Java language. Let us check out the following sections related to XPS and OXPS files conversion:

*   [XPS or OXPS to PDF Conversion – API Installation][5]
*   [Convert XPS to PDF Programmatically using Java][6]
*   [Convert OXPS to PDF Programmatically using Java][7]

## XPS or OXPS to PDF Conversion – API Installation {#section1}

[Aspose.Page for Java][8] API is designed to create, edit, manipulate and convert different fixed document formats including XPS, OXPS, [EPS][9], [PS][10], etc. You can quickly configure the API by downloading the JAR file from the [Downloads][11] section or adding the below configuration in the pom.xml file of your Maven project. This will configure the API hosted on [Aspose Artifactory][12]:

### Repository```
 <repositories>
     <repository>
         <id>snapshots</id>
         <name>repo</name>
         <url>http://repository.aspose.com/repo/</url>
     </repository>

</repositories>
```

### Dependency```
 <dependencies>
    <dependency>
        <groupId>com.aspose</groupId>
        <artifactId>aspose-page</artifactId>
        <version>20.1</version>
    </dependency>
</dependencies>
```

## Convert XPS to PDF Programmatically using Java {#section2}

You can convert XPS files to PDF documents with high fidelity among the input and output files. You need to follow the steps below for the conversion:

*   Load input XPS document
*   Initialize [PdfSaveOptions][13] object
*   Create [PdfDevice][14] for rendering
*   Save output PDF file

The following code snippet shows how to convert XPS to PDF programmatically using Java:

{{< gist aspose-com-gists 36014fe18885c184d472ae34c0c29750 "XPS-to-PDF.java" >}}

## Convert OXPS to PDF Programmatically in Java {#section3}

OXPS is a fixed layout format that can be used for creating letters, memos, and other official documents. Moreover, OXPS to PDF conversion is quite similar with above use case. So far we have learned how to convert all pages in the input file to PDF. Let us proceed another step further where we will be converting specific pages of OXPS file to PDF document. You can easily convert OXPS file to PDF in your Java applications. Below are the steps for converting OXPS to PDF document:

*   Load input OXPS document
*   Initialize [PdfSaveOptions][15] object with necessary parameters
*   Specify the page numbers with [setPageNumbers][16] method
*   Create rendering device for PDF format
*   Save output PDF file

The code below explains how to convert OXPS to PDF programmatically in Java:

{{< gist aspose-com-gists 36014fe18885c184d472ae34c0c29750 "OXPS-to-PDF.java" >}}

As we have discussed above, this code will convert specific pages to PDF. The output PDF file will comprise of first and third page from the input OXPS file.

## Conclusion

In this article, we have explored how to convert XPS or OXPS files to PDF documents. We have explored how to convert a whole document with all pages, as well as converting a few pages to PDF format files. Moreover, the API [supports several other file formats][17] that you can create, edit, or manipulate as per your requirements. We hope you must be interested to learn more, several other learning resources include [API documentation][18] as well as the [Examples project][19]. Furthermore, you can discuss any of your requirements or concerns via the [Free Support Forum][20]. We positively look forward to assisting you!

## See Also

[Convert XPS, OXPS to JPG or PNG Image using C# VB.NET][21]




[1]: https://docs.fileformat.com/page-description-language/xps/
[2]: https://en.wikipedia.org/wiki/Open_XML_Paper_Specification
[3]: https://docs.fileformat.com/page-description-language/xps/
[4]: https://en.wikipedia.org/wiki/Open_XML_Paper_Specification
[5]: #section1
[6]: #section2
[7]: #section3
[8]: https://products.aspose.com/page/java
[9]: https://docs.fileformat.com/page-description-language/eps/
[10]: https://docs.fileformat.com/page-description-language/ps/
[11]: https://downloads.aspose.com/page/java
[12]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/
[13]: https://apireference.aspose.com/page/java/com.aspose.eps.device/PdfSaveOptions
[14]: https://apireference.aspose.com/page/java/com.aspose.xps.rendering/PdfDevice
[15]: https://apireference.aspose.com/page/java/com.aspose.eps.device/PdfSaveOptions
[16]: https://apireference.aspose.com/page/java/com.aspose.xps.rendering/PdfSaveOptions#setPageNumbers-int:A-
[17]: https://docs.aspose.com/page/java/supported-file-formats/
[18]: https://docs.aspose.com/page/java/
[19]: https://github.com/aspose-page/Aspose.Page-for-Java
[20]: https://forum.aspose.com/c/page
[21]: https://blog.aspose.com/2020/11/02/convert-xps-to-jpg-png-image-csharp-vb-net/





