---
title: 'Create Table in PDF Files in Java'
seoTitle: "Create Table in PDF Files in Java | Java PDF Generator API"
description: "Use Java PDF generator API to create table in PDF files using Java. Set margins, borders, and column adjustment of tables programmatically."
date: Fri, 22 Apr 2022 18:54:00 +0000
draft: false
url: /2022/04/22/create-table-in-pdf-files-in-java/
author: Usman Aziz
summary: 'A table lets the readers go through the data quickly without reading a lot of text. Therefore, tables are considered an integral part of the documents. While working on [PDF][1] automation and generating the PDF files programmatically, you may come across the need to create tables very often. To accomplish that, this article covers **how to create tables in PDF files using Java**.'
tags: ['Apply Column Adjustment to PDF Tables Java', 'Create a Table in a PDF File in Java', 'Java API to Create Tables in PDF', 'Java PDF Generator API', 'Set Borders and Margins in PDF Tables in Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Create-Tables-in-PDF.jpg" alt="Create Table in PDF Files in Java">}}


A table lets the readers go through the data quickly without reading a lot of text. Therefore, tables are considered an integral part of the documents. While working on [PDF][2] automation and generating the PDF files programmatically, you may come across the need to create tables very often. To accomplish that, this article covers **how to create tables in PDF files using Java**.

*   [Java API to Create Tables in PDF][3]
*   [Create a Table in a PDF File][4]
*   [Set Borders and Margins in PDF Tables][5]
*   [Apply Column Adjustment to PDF Tables][6]

## Java API to Create Tables in PDF Files {#API-to-Create-Tables-in-PDF}

[Aspose.PDF for Java][7] is a popular API to perform PDF generation and manipulation within Java applications. Using the API, you can seamlessly create PDF files of simple and complex layouts. We will use this API to create tables in new or existing PDF files. You can [download][8] the API or install it using the following Maven configurations.

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

## Create a Table in a PDF File in Java {#Create-a-Table-in-a-PDF-File}

You can create tables in either a new or an existing PDF file using Aspose.PDF for Java. The following are the steps to create a table in a PDF file in Java.

*   Load the PDF file (or create a new one) using [Document][9] class.
*   Initialize a table and set its columns and rows using [Table][10] class.
*   Set table’s settings (i.e. borders).
*   Populate the table by creating rows using [Table.getRows().add()][11] method.
*   Add the table to the page using [Document.getPages().get\_Item(index).getParagraphs().add(Table)][12] method.
*   Save the PDF file using [Document.save(String)][13] method.

The following code sample shows how to create a table in a PDF file using Java.

{{< gist aspose-com-gists 2ab694cf32f62d85efe234bd2c3a2165 "create-table-in-pdf.java" >}}

The following is the output of the above code sample.



{{< figure align=center src="images/Create-Tables-in-PDF.png" alt="Create a Table in a PDF File in Java">}}


## Create PDF Table with Customized Borders and Margins {#Set-Borders-and-Margins-in-PDF-Tables}

You can also customize the borders and margins of the tables in PDF as per your requirements. For example, you can set the border width, border style, and top, bottom, left, and right margins. The following are the steps to set borders and margins for the tables in PDF files in Java.

*   Load the PDF file (or create a new one) using [Document][14] class.
*   Initialize a table and set its columns and rows using [Table][15] class.
*   Create an instance of [BorderInfo][16] class to apply border styling.
*   Create an instance of [MarginInfo][17] class to set margins for the table.
*   Populate the table by creating rows using [Table.getRows().add()][18] method.
*   Add the table to the page using [Document.getPages().get\_Item(index).getParagraphs().add(Table)][19] method.
*   Save the PDF file using [Document.save(String)][20] method.

The following code sample shows how to set borders and margins for tables in PDF using Java.

{{< gist aspose-com-gists 2ab694cf32f62d85efe234bd2c3a2165 "create-table-in-pdf-margin-border.java" >}}

The following screenshot shows the output of the above code sample.



{{< figure align=center src="images/Create-Tables-in-PDF-Border-and-Margins.png" alt="Create PDF Table with Customized Borders and Margins Java">}}


## Apply Column Adjustment to PDF Tables in Java {#Apply-Auto-Fit-Settings-to-PDF-Tables}

Aspose.PDF for Java also allows you to customize the column adjustment of the table in a PDF. For example, you can auto-fit the table to the window or the content. The following are the steps to set the column adjustment of a table in PDF using Java.

*   Load the PDF file (or create a new one) using [Document][21] class.
*   Initialize a table and set its columns and rows using [Table][22] class.
*   Set borders and margins.
*   Set column adjustment with the desired value of [ColumnAdjustment][23] enum.
*   Populate the table by creating rows using [Table.getRows().add()][24] method.
*   Add the table to the page using [Document.getPages().get\_Item(index).getParagraphs().add(Table)][25] method.
*   Save the PDF file using [Document.save(String)][26] method.

The following code sample shows how to set the column adjustment of the table in PDF using Java.

{{< gist aspose-com-gists 2ab694cf32f62d85efe234bd2c3a2165 "create-table-in-pdf-autofit.java" >}}

## Get a Free License {#Get-a-Free-License}

You can [get a free temporary license][27] in order to use Aspose.PDF for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to create tables in PDF files using Java. Furthermore, you have seen how to customize the borders. margins, and column adjustment of a table in PDF. Besides, you can explore more about the Java PDF API using the [documentation][28]. In case you would have any questions or queries, you can contact us via our [forum][29].

## See Also

*   [Creating PDF Files from Scratch using Java][30]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #API-to-Create-Tables-in-PDF
[4]: #Create-a-Table-in-a-PDF-File
[5]: #Set-Borders-and-Margins-in-PDF-Tables
[6]: #Apply-Auto-Fit-Settings-to-PDF-Tables
[7]: https://products.aspose.com/pdf/java/
[8]: https://downloads.aspose.com/pdf/java
[9]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[10]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Table
[11]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Rows#add--
[12]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Paragraphs#add-com.aspose.pdf.BaseParagraph-
[13]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[14]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[15]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Table
[16]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/BorderInfo
[17]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/MarginInfo
[18]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Rows#add--
[19]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Paragraphs#add-com.aspose.pdf.BaseParagraph-
[20]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[21]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[22]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Table
[23]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/ColumnAdjustment
[24]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Rows#add--
[25]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Paragraphs#add-com.aspose.pdf.BaseParagraph-
[26]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[27]: https://purchase.aspose.com/temporary-license
[28]: https://docs.aspose.com/pdf/java/
[29]: https://forum.aspose.com/
[30]: https://blog.aspose.com/2020/12/31/create-pdf-files-in-java/




