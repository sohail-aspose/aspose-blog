---
title: 'Generate Thumbnails for PDF Files in Java'
date: Fri, 15 Apr 2022 16:14:00 +0000
draft: false
url: /2022/04/15/generate-thumbnails-for-pdf-files-in-java/
author: 'Usman Aziz'
summary: 'While embedding the [PDF][1] documents into a web application you may need to generate a thumbnail. In other scenarios, such as creating a PDF viewer, you may need to create a thumbnail for each page in the PDF. In this article, we will show you **how to generate thumbnails of a PDF file programmatically in Java**. We will explicitly cover how to create a thumbnail of a particular page or all the pages in a PDF file.'
tags: ['Generate Thumbnails of all Pages in PDF Java', 'Generate a Thumbnail of a PDF File Java', 'Java API to Generate Thumbnails of PDF', 'Java PDF Generator API']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Extract-Images-from-PDF.jpg" alt="Generate Thumbnails for PDF Files in C#">}}


While embedding the [PDF][2] documents into a web application you may need to generate a thumbnail. In other scenarios, such as creating a PDF viewer, you may need to create a thumbnail for each page in the PDF. In this article, we will show you **how to generate thumbnails of a PDF file programmatically in Java**. We will explicitly cover how to create a thumbnail of a particular page or all the pages in a PDF file.

*   [Java API to Generate Thumbnails of PDF][3]
*   [Generate a Thumbnail of a PDF File][4]
*   [Generate Thumbnails of all Pages in PDF][5]

## Java API to Generate Thumbnails of PDF {#API-to-Generate-Thumbnails-of-PDF}

To generate the thumbnails of PDF files, we will use [Aspose.PDF for Java][6]. It is a feature-rich library that lets you create and manipulate PDF documents. The API allows you to perform basic as well as advanced PDF automation operations seamlessly. You can [download][7] the API or install it using the following Maven configurations.

```
**Repository:**
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>

**Dependency:**
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-pdf</artifactId>
    <version>22.4</version>
</dependency>
```

## Generate a Thumbnail of a PDF File in Java {#Generate-a-Thumbnail-of-a-PDF-File}

Usually, you have to generate a single thumbnail image for a PDF document. The page for thumbnail could be the cover page or any other page of your choice. The following are the steps to generate a thumbnail of the desired page of a PDF in Java.

*   Load the PDF file using the [Document][8] class.
*   Get a reference of the desired page from the [Document.getPages()][9] collection.
*   Create a new [FileInputStream][10] for the image file.
*   Create an instance of the [Resolution][11] class to set the resolution of the thumbnail image.
*   Instantiate [JpegDevice][12] and set the height, width, resolution, and quality of the image.
*   Generate thumbnail using [JpegDevice.process(Page, FileInputStream)][13] method.
*   Close the file stream.

The following code sample shows how to generate a thumbnail of a PDF file in Java.

{{< gist aspose-com-gists b0f393d47f9178e9ab25e2168bed4a6e "generate-pdf-thumbnail.java" >}}

## Generate Thumbnails of all Pages in PDF in Java {#Generate-Thumbnails-of-all-Pages-in-PDF}

The following are the steps to generate thumbnails for all the pages in PDF in Java.

*   Load the PDF file using the [Document][14] class.
*   Loop through all the pages in PDF using [Document.getPages()][15] collection.
*   In each iteration, perform the following operations:
    *   Create a new [FileInputStream][16] for the image file.
    *   Create an instance of the [Resolution][17] class to set the resolution of the thumbnail image.
    *   Instantiate [JpegDevice][18] and set the height, width, resolution, and quality of the image.
    *   Generate thumbnail using [JpegDevice.process(Page, FileInputStream)][19] method.
    *   Close the file stream.

The following code sample shows how to generate thumbnails for all the pages in PDF.

{{< gist aspose-com-gists b0f393d47f9178e9ab25e2168bed4a6e "generate-pdf-thumbnail-all-pages.java" >}}

## Get a Free License {#Get-a-Free-License}

You can [get a free temporary license][20] in order to use Aspose.PDF for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to generate thumbnails for PDF files in Java. You have seen how to generate a thumbnail of a particular page or all the pages in a PDF file. Besides, you can explore more about the Java PDF API using the [documentation][21]. In case you would have any questions or queries, you can contact us via our [forum][22].

## See Also

*   [Creating PDF Files from Scratch using Java][23]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #API-to-Generate-Thumbnails-of-PDF
[4]: #Generate-a-Thumbnail-of-a-PDF-File
[5]: #Generate-Thumbnails-of-all-Pages-in-PDF
[6]: https://products.aspose.com/pdf/java/
[7]: https://downloads.aspose.com/pdf/java
[8]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[9]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#getPages--
[10]: https://docs.oracle.com/javase/7/docs/api/java/io/FileInputStream.html
[11]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.devices/Resolution
[12]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.devices/JpegDevice
[13]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.devices/JpegDevice#process-com.aspose.pdf.Page-java.io.OutputStream-
[14]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[15]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#getPages--
[16]: https://docs.oracle.com/javase/7/docs/api/java/io/FileInputStream.html
[17]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.devices/Resolution
[18]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.devices/JpegDevice
[19]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.devices/JpegDevice#process-com.aspose.pdf.Page-java.io.OutputStream-
[20]: https://purchase.aspose.com/temporary-license
[21]: https://docs.aspose.com/pdf/java/
[22]: https://forum.aspose.com/
[23]: https://blog.aspose.com/2020/12/31/create-pdf-files-in-java/




