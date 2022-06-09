---
title: 'Extract Data from Tables in PDF using Java'
seoTitle: "Java: Extract Data from Tables in PDF | PDF Data Extractor API"
description: "Use Java PDF API to extract data from the PDF table using Java. Extract tables from all pages or a specific region of a page in PDF."
date: Mon, 11 Oct 2021 15:25:24 +0000
draft: false
url: /2021/10/11/extract-data-from-tables-in-pdf-using-java/
author: Usman Aziz
summary: '[PDF][1] is one of the ruling document formats these days. It supports text, graphics, tables, annotations, and a range of other elements. In certain cases, you may need to extract data from the tables in PDF documents such as invoices. To achieve this programmatically, the article covers **how to extract data from tables in PDF using Java**.'
tags: ['Extract Data from Tables in PDF using Java', 'Extract Table from a Specific Area of PDF Java', 'Java API to Extract Data from Tables in PDF', 'Java Text Extractor API for PDF']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Extract-Tables-in-PDF.jpg" alt="Extract Data from Table in PDF Java">}}


[PDF][2] is one of the ruling document formats these days. It supports text, graphics, tables, annotations, and a range of other elements. In certain cases, you may need to extract data from the tables in PDF documents such as invoices. To achieve this programmatically, the article covers **how to extract data from tables in PDF using Java**.

*   [Java API to Extract Data from Tables in PDF][3]
*   [Extract Data from Tables in PDF][4]
*   [Extract Table from a Specific Area of Page][5]

## Java API to Extract Data from Tables in PDF {#API-to-Extract-Table-from-PDF}

[Aspose.PDF for Java][6] is a feature-rich API for creating and manipulating PDF documents. We will use this API to extract the data from tables in PDF documents. You can either [download][7] the API’s JAR or install it within your Java application using the following [Maven][8] configurations.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-pdf</artifactId>
    <version>21.9</version>
</dependency>
```

## Extract Data from Tables in PDF using Java {#Extract-Data-from-PDF-Table}

The following are the steps to extract data from tables in a PDF using Java.

*   First, load the PDF document using the [Document][9] class.
*   Loop through the pages in PDF using [Document.getPages()][10] collection.
*   In each iteration, initialize the [TableAbsorber][11] object and visit the selected page using [TableAbsorber.visit(Page)][12] method.
*   In a nested loop, iterate through the list of the tables in [TableAbsorber.getTableList()][13] collection.
*   For each [AbsorbedTable][14] in the collection, iterate through the collection of rows from [AbsorbedTable.getRowList()][15].
*   For each [AbsorbedRow][16] in the collection, iterate through the collection of cells from [AbsorbedRow.getCellList()][17].
*   Finally, loop through the [TextFragment][18] collection of each [AbsorbedCell][19] and print the text.

The following code sample shows how to extract text from tables in PDF using Java.

{{< gist aspose-com-gists 97a90eacc17f509deafc22fd5721a59a "extract-text-from-pdf-table.java" >}}

## Extract Table from a Specific Area of PDF Page {#Extract-Table-from-a-Specific-Area-of-Page}

The following are the steps to extract table from a specific part of the page in a PDF using Java.

*   First, load the PDF document using the [Document][20] class.
*   Then, select the desired [Page][21] from [Document.getPages()][22] collection.
*   Extract the Square annotation of the page.
*   In each iteration, initialize the [TableAbsorber][23] object and visit the selected page using [TableAbsorber.visit(Page)][24] method.
*   In a nested loop, iterate through the list of the tables in [TableAbsorber.getTableList()][25] collection.
*   Check if the absorbed table is in the desired page region.
*   For each [AbsorbedTable][26] in the collection, iterate through the collection of rows using [AbsorbedTable.getRowList()][27].
*   For each [AbsorbedRow][28] in the collection, iterate through the collection of cells using [AbsorbedRow.getCellList()][29].
*   Finally, loop through the [TextFragment][30] collection of each [AbsorbedCell][31] and print the text.

The following code sample shows how to extract tables from a specific region of the PDF page.

{{< gist aspose-com-gists 97a90eacc17f509deafc22fd5721a59a "extract-text-from-pdf-table-specific-area.java" >}}

## Get a Free License {#Get-a-Free-License}

You can use Aspose.PDF for Java without evaluation limitations using a [temporary license][32].

## Conclusion

In this article, you have learned how to extract data from tables in a PDF using Java. Furthermore, the article covered how to extract tables from a specific region of the page in PDF. Besides, you can learn more about Aspose.PDF for Java using the [documentation][33]. In addition, you can ask your questions via our [forum][34].

## See Also

*   [Creating PDF Files from Scratch using Java][35]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #API-to-Extract-Table-from-PDF
[4]: #Extract-Data-from-PDF-Table
[5]: #Extract-Table-from-a-Specific-Area-of-Page
[6]: https://products.aspose.com/pdf/java
[7]: https://downloads.aspose.com/pdf/java
[8]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-pdf
[9]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[10]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#getPages--
[11]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TableAbsorber
[12]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TableAbsorber#visit-com.aspose.pdf.Page-
[13]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TableAbsorber#getTableList--
[14]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/AbsorbedTable
[15]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/AbsorbedTable#getRowList--
[16]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/AbsorbedRow
[17]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/AbsorbedRow#getCellList--
[18]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragment
[19]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/AbsorbedCell
[20]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[21]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Page
[22]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#getPages--
[23]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TableAbsorber
[24]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TableAbsorber#visit-com.aspose.pdf.Page-
[25]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TableAbsorber#getTableList--
[26]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/AbsorbedTable
[27]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/AbsorbedTable#getRowList--
[28]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/AbsorbedRow
[29]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/AbsorbedRow#getCellList--
[30]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragment
[31]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/AbsorbedCell
[32]: https://purchase.aspose.com/temporary-license
[33]: https://docs.aspose.com/pdf/java
[34]: https://forum.aspose.com/
[35]: https://blog.aspose.com/2020/12/31/create-pdf-files-in-java/




