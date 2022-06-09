---
title: 'Convert PDF Documents to Excel XLS/XLSX using Java'
seoTitle: ""
description: ""
date: Wed, 24 Jun 2020 00:21:50 +0000
draft: false
url: /2020/06/24/convert-pdf-to-excel-xls-xlsx-using-java/
author: Usman Aziz
summary: ''
tags: ['convert PDF to Excel using Java', 'convert PDF to XLS using Java', 'convert PDF to XLSX using Java', 'export table from PDF to Excel in Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/PDF-to-Excel.jpg" alt="PDF to Excel Java">}}


There could be various scenarios when you need to export the data within the tables from **PDF to Excel** workbooks. PDF to Excel lets you edit the data, apply formulas, plot charts, and perform other operations that are supported by the spreadsheets. In this article, I'll show you how to automate the PDF to Excel conversion and **convert PDF to XLS to XLSX workbooks programmatically using Java**. For this, we'll leverage the capabilities of [Aspsoe.PDF for Java][1] API.

*   [PDF to Excel Converter API - Installation][2]
*   [Convert PDF to XLS using Java][3]
*   [Convert PDF to XLSX using Java][4]
*   [PDF to Excel - Minimize the Number of Worksheets][5]

## Java PDF to Excel Converter - Installation {#PDF-to-Excel-Converter-API-Installation}

[Aspose.PDF for Java][6] is available for [download][7] as a JAR file. In addition, you can install it in your Maven-based applications using the following configurations.

### Repository```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```

### Dependency```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-pdf</artifactId>
    <version>20.5</version>
    <classifier>jdk17</classifier>
</dependency>
```

## Convert PDF to Excel XLS using Java {#Convert-PDF-to-XLS-using-Java}

In order to convert PDF to Excel XLS, you simply need to load the PDF document and save it with _.xls_ extension. The following are the steps to perform this conversion.

*   Load the PDF file using [Document][8] class.
*   Save the PDF as Excel XLS using [Document.save(String outputFileName, int format)][9] method.

The following code sample shows how to convert PDF to Excel XLS using Java.

{{< gist aspose-com-gists 54bc1b3bf672553e34f2b7a317cffb6c "convert-pdf-to-xls.java" >}}

### Input PDF Document



{{< figure align=center src="images/Convert-pdf-to-excel-C.png" alt="Convert PDF to Excel">}}


### Output Excel Spreadsheet



{{< figure align=center src="images/Convert-pdf-to-excel-C-2.png" alt="PDF to XLS XLSX">}}


## Convert PDF to Excel XLSX using Java {#Convert-PDF-to-XLSX-using-Java}

For converting PDF to XLSX spreadsheet, you need to define the output Excel format using [ExcelSaveOptions][10] class. The following are the steps to perform PDF to XLSX conversion using Aspose.PDF for Java.

*   Load the input PDF document using the [Document][11] class.
*   Create an instance of [ExcelSaveOptions][12] class.
*   Set the output format using [ExcelSaveOptions.setFormat(ExcelSaveOptions.ExcelFormat.XLSX)][13] method.
*   Convert PDF to Excel using [Document.save(String outputFileName, SaveOptions options)][14] method.

The following code sample shows how to convert PDF to XLSX using Java.

{{< gist aspose-com-gists 54bc1b3bf672553e34f2b7a317cffb6c "convert-pdf-to-xlsx.java" >}}

## Minimize the Number of Worksheets in PDF to Excel {#Minimize-the-Number-of-Worksheets-in-the-Converted-Excel-Workbook}

By default, Aspose.PDF converts each page in the PDF document to a separate worksheet. However, you may customize the API to minimize the number of worksheets in case of large PDF documents. The following are the steps to perform this operation.

*   Use the [Document][15] class to load the input PDF document.
*   Create an instance of [ExcelSaveOptions][16] class.
*   Set option [ExcelSaveOptions.setMinimizeTheNumberOfWorksheets(true)][17].
*   Save PDF as XLSX.

The following code sample shows how to convert PDF to XLSX with a minimized number of worksheets using Java.

{{< gist aspose-com-gists 54bc1b3bf672553e34f2b7a317cffb6c "convert-pdf-to-xlsx-minimized-sheets.java" >}}

## Conclusion

In this article, you have seen **how to convert PDF to Excel XLS or XLSX files using Java**. Furthermore, the feature of minimizing the number of worksheets in PDF to Excel is also discussed with the help of the code sample. You can explore more about Aspose.PDF for Java using the [documentation][18].

## See Also

*   [Convert PDF to Excel XLS/XLSX using C#][19]




[1]: https://products.aspose.com/pdf/java
[2]: #PDF-to-Excel-Converter-API-Installation
[3]: #Convert-PDF-to-XLS-using-Java
[4]: #Convert-PDF-to-XLSX-using-Java
[5]: #Minimize-the-Number-of-Worksheets-in-the-Converted-Excel-Workbook
[6]: https://products.aspose.com/pdf/java
[7]: https://downloads.aspose.com/pdf/java
[8]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[9]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-int-
[10]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/ExcelSaveOptions
[11]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[12]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/ExcelSaveOptions
[13]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/ExcelSaveOptions#setFormat-int-
[14]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-com.aspose.pdf.SaveOptions-
[15]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[16]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/ExcelSaveOptions
[17]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/ExcelSaveOptions#setMinimizeTheNumberOfWorksheets-boolean-
[18]: https://docs.aspose.com/pdf/java
[19]: https://blog.aspose.com/2020/01/03/convert-pdf-to-excel-in-csharp-net-pdf-to-xls-pdf-to-xlsx/





