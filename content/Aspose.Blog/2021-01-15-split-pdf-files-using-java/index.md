---
title: 'Split a PDF File using Java'
seoTitle: "Split PDF File into Multiple PDFs using Java | Java PDF Splitter Library"
description: "Split a PDF file into multiple files using Java. Split each page or a collection of pages in PDF to separate files using Java PDF splitter API."
date: Fri, 15 Jan 2021 11:34:00 +0000
draft: false
url: /2021/01/15/split-pdf-files-using-java/
author: Usman Aziz
summary: 'There could be various cases when you need to split a PDF into multiple PDF files. For example, you may have to split each page of the PDF containing invoices/receipts and save them as separate files. On the other hand, you may want to split a particular collection of pages from a PDF file. In order to deal with the above-mentioned scenarios, this article covers **how to split a PDF file into multiple PDFs programmatically using Java**.'
tags: ['Java-API-to-Split-PDF-Files', 'Split-a-PDF-File-by-Each-Page-using-Java', 'Split-a-PDF-File-by-Page-Collection-using-Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Split-PDF-Files.jpg" alt="Split PDF Files in Java">}}


There could be various cases when you need to split a [PDF][1] into multiple PDF files. For example, you may have to split each page of the PDF containing invoices/receipts and save them as separate files. On the other hand, you may want to split a particular collection of pages from a PDF file. In order to deal with the above-mentioned scenarios, this article covers **how to split a PDF file into multiple PDFs using [Java][2]**.

*   [Java API to Split PDF Files][3]
*   [Split a PDF File by Each Page using Java][4]
*   [Split a PDF File by Page Collection using Java][5]
*   [Get Free License][6]

## Java API to Split PDF Files – Free Download {#Java-API-to-Split-PDF-Free-Download}

In order to split the PDF files, we'll leverage the PDF manipulation capabilities of [Aspose.PDF for Java][7]. The API lets you perform a PDF splitting operation within a few steps. You can either [download][8] the API or install it within your Maven-based applications using the following configurations.

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
    <version>20.12</version>
    <classifier>jdk17</classifier>
</dependency>
```

## Split a PDF File using Java {#Split-a-PDF-File-by-Pages-using-Java}

The PDF splitting criteria may vary in different scenarios as per requirements. First, let's check out how to split a PDF file by pages and save each page as a separate PDF. The following are the steps to perform this operation.

*   Load the PDF document using [Document][9] class.
*   Loop through the pages using [Document.getPages()][10] method.
*   Access each page into a [Page][11] object.
*   In every iteration, create a new [Document][12], add the current page to the document and save it as a PDF file using [Document.save(String)][13] method.

The following code sample shows how to split a PDF file using Java.

{{< gist aspose-com-gists dbd370f2a932f1dc591bee6222550150 "split-pdf.java" >}}

## Split a PDF File by Page Collection using Java {#Select-Pages-to-Split-a-PDF-File-using-Java}

For the demonstration, let's have a look at another PDF splitting scenario. In this example, we will split a PDF based on even and odd page numbers. The following are the steps to perform this operation.

*   Load the PDF document using [Document][14] class.
*   Loop through the pages using [Document.getPages()][15] method.
*   Separate even and odd pages into _ArrayList<Page>_ objects.
*   Create a new [Document][16] object, add pages to the document and save it as a PDF file using [Document.save(String)][17] method.

The following code sample shows how to split even and odd pages in a PDF file using Java.

{{< gist aspose-com-gists dbd370f2a932f1dc591bee6222550150 "split-pdf-even-odd.java" >}}

## Get a Free License {#Get-Free-License}

You can [get a free temporary license][18] in order to try the API without evaluation limitations.

## Conclusion

In this article, you have learned how to split a PDF file using Java. Furthermore, you have seen how to customize the PDF splitting criteria as per requirements. You can explore more about the API using the [documentation][19].

## See Also

*   [Create PDF Files using Java – Java PDF API][20]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/programming/java/
[3]: #Java-API-to-Split-PDF-Free-Download
[4]: #Split-a-PDF-File-by-Pages-using-Java
[5]: #Select-Pages-to-Split-a-PDF-File-using-Java
[6]: #Get-Free-License
[7]: https://products.aspose.com/pdf/java
[8]: https://downloads.aspose.com/pdf/java
[9]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[10]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#getPages--
[11]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Page
[12]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[13]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[14]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[15]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#getPages--
[16]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[17]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/pdf/java/getting-started/
[20]: https://blog.aspose.com/2020/12/31/create-pdf-files-in-java/





