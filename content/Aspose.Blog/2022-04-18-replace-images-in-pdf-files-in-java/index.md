---
title: 'Replace Images in PDF Files in Java'
date: Mon, 18 Apr 2022 05:14:00 +0000
draft: false
url: /2022/04/18/replace-images-in-pdf-files-in-java/
author: 'Usman Aziz'
summary: 'Various industries use [PDF](https://docs.fileformat.com/pdf/) format to automatically generate their documents such as invoices, reports, technical articles, etc. Along with text, these documents may also contain images and other graphical objects. In some instances, you have to replace the confidential images in the PDF documents before sharing. To accomplish that programmatically, this article covers **how to replace images in PDF documents in Java**.'
tags: ['Java API to Replace Images in PDF Files', 'Java PDF Generator API', 'Replace Images in a PDF File in Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Extract-Images-from-PDF.jpg" alt="Replace Images in PDF Files in Java">}}


Various industries use [PDF](https://docs.fileformat.com/pdf/) format to automatically generate their documents such as invoices, reports, technical articles, etc. Along with text, these documents may also contain images and other graphical objects. In some instances, you have to replace the confidential images in the PDF documents before sharing. To accomplish that programmatically, this article covers **how to replace images in PDF documents in Java**.

*   [API to Replace Images in PDF Files](#API-to-Replace-Images-in-PDF-Files)
*   [Replace Images in a PDF File](#Replace-Images-in-a-PDF-File)

## Java API to Replace Images in PDF Files {#API-to-Replace-Images-in-PDF-Files}

To replace images in PDF files, we will use [Aspose.PDF for Java](https://products.aspose.com/pdf/java/). It is a powerful library that provides basic as well as advanced PDF generation and manipulation features. You can either [download](https://downloads.aspose.com/pdf/java) the API or install it using the following Maven configurations.

```
**Repository:** <repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>

**Dependency:** <dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-pdf</artifactId>
    <version>22.4</version>
</dependency>
```

## Replace Images in a PDF File in Java {#Replace-Images-in-a-PDF-File}

In PDF documents, the images are kept in an image collection of each page. Thus, you can access any of the images from the collection using its index and manipulate it. The following are the steps to replace a particular image in a PDF in Java.

*   Load the PDF file using the [Document](https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document) class.
*   Get reference of the desired page of the PDF from collection using [Document.getPages()](https://apireference.aspose.com/pdf/java/com.aspose.pdf/PageCollection) method.
*   Replace the image in the collection using [Pages\[index\].getResources().getImages().replace(imageIndex, new FileInputStream("lovely.jpg"))](https://apireference.aspose.com/pdf/java/com.aspose.pdf/XImageCollection#replace-int-java.io.InputStream-) method.
*   Save the updated document using [Document.save(string)](https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-) method.

The following code sample shows how to replace an image in a PDF using Java.

{{< gist aspose-com-gists 52282e9ca33265d0884b6d658f30b212 "replace-image-in-pdf.java" >}}

## Get a Free License {#Get-a-Free-License}

You can [get a free temporary license](https://purchase.aspose.com/temporary-license) in order to use Aspose.PDF for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to replace images in PDF files using Java. You can simply integrate the provided code sample and replace PDF images from within your applications. Besides, you can explore more about the Java PDF API using the [documentation](https://docs.aspose.com/pdf/java/). In case you would have any questions or queries, you can contact us via our [forum](https://forum.aspose.com/).

## See Also

*   [Creating PDF Files from Scratch using Java](https://blog.aspose.com/2020/12/31/create-pdf-files-in-java/)




