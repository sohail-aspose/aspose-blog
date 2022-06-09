---
title: 'Generate PDF File from Images using Java'
seoTitle: "Generate PDF File from Images in Java | Image to PDF in Java"
description: "Use Java PDF Generator API to generate PDF files from multiple images in Java. Perform image to PDF conversion programmatically."
date: Mon, 01 Mar 2021 10:56:00 +0000
draft: false
url: /2021/03/01/generate-pdf-file-from-images-using-java/
author: Usman Aziz
summary: 'In various cases, you may need to convert a collection of images to a PDF file. For example, you may want to insert all images from an album into a single PDF file. On the other hand, you may need to generate PDF from the images of a scanned document. In order to deal with such cases, this article covers **how to generate a PDF from multiple images using Java**.'
tags: ['Add images to pdf using java', 'generate PDF files from images java', 'image to pdf in java', 'java pdf generator']
categories: ['Aspose.PDF Product Family']
---

In various cases, you may need to convert a collection of images to a [PDF][1] file. For example, you may want to insert all images from an album into a single PDF file. On the other hand, you may need to generate PDF from the images of a scanned document. In order to perform image to PDF conversion, this article covers **how to generate a PDF from multiple images using [Java][2]**.

*   [Java API for Image to PDF Conversion][3]
*   [Steps to Generate a PDF File from Images][4]
*   [Generate PDF from Images using Java][5]
*   [Get a Free API License][6]

## Java API for Image to PDF Conversion {#Java-API-to-Generate-PDF-from-Images}

[Aspose.PDF for Java][7] is a powerful API that provides basic as well as advanced PDF manipulation features. It lets you generate new PDF files and modify the existing ones quite easily. You can [download][8] the API's JAR or install it using the following Maven configurations.

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
    <version>21.2</version>
</dependency>
```

## Steps to Generate PDF from Images {#Steps-to-Generate-a-PDF-File-from-Image}

The following are the steps that we will follow to generate a PDF file from images in this article.

*   First, create a new PDF document.
*   Get the list of the images' file names in an array.
*   For each image file in the list, do the following:
    *   Add a new page to the PDF document and set its properties.
    *   Load each image file in a file stream from the list.
    *   Add image to the paragraph collection of the page.
*   Finally, save the PDF document.

## Generate PDF from Images using Java {#Generate-PDF-from-Images-using-Java}

Let's now check out how to implement each of the above-mentioned steps using Aspose.PDF for Java.

*   Create an instance of [Document][9] class.
*   Get the list of the images' file names in an array using the [java.io.File][10] class.
*   For each image file in the list, do the following:
    
    *   Add a new [Page][11] to the PDF document using [Document.getPages().add()][12] method and set page's properties.
    *   Load the image file into a [FileInputStream][13] object.
    *   Add a new [Image][14] to the page using [Page.getParagraphs().add(Image)][15] method.
    
    *   Set image's stream using [Image.setImageStream(FileInputStream)][16] method.
*   Finally, save the PDF document using [Document.save(String)][17] method.

The following code sample shows how to generate PDF file from images in Java.

{{< gist aspose-com-gists 8cc0eeecadf75ea93d5d8d6237c8a940 "generate-pdf-from-images.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

In case you want to try the API without evaluation limitations, you can [get a free temporary license][18].

## Conclusion

In this article, you have learned how to generate a PDF file based on multiple images using Java. The step-by-step guide and code sample demonstrated how to fetch images from a folder and insert them into the PDF. You can explore more about the Java PDF API using [documentation][19].

## See Also

*   [Split a PDF File Programmatically using Java][20]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/programming/java/
[3]: #Java-API-to-Generate-PDF-from-Images
[4]: #Steps-to-Generate-a-PDF-File-from-Image
[5]: #Generate-PDF-from-Images-using-Java
[6]: #Get-a-Free-API-License
[7]: https://products.aspose.com/pdf/java
[8]: https://downloads.aspose.com/pdf/java
[9]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[10]: https://docs.oracle.com/javase/7/docs/api/java/io/File.html
[11]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Page
[12]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/PageCollection#add-com.aspose.pdf.Page-
[13]: https://docs.oracle.com/javase/7/docs/api/java/io/FileInputStream.html
[14]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Image
[15]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Paragraphs#add-com.aspose.pdf.BaseParagraph-
[16]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Image#setImageStream-java.io.InputStream-
[17]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/pdf/java
[20]: https://blog.aspose.com/2021/01/15/Split-PDF-Files-using-Java/





