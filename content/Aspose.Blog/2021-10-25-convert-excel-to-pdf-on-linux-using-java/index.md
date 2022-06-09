---
title: 'Convert Excel Files to PDF on Linux using Java'
seoTitle: "Convert Excel to PDF on Linux | Convert XLSX or XLS to PDF using Java"
description: "Convert MS Excel files to PDF using Excel to PDF converter API for Linux. Convert XLSX to PDF or XLS to PDF or PDF/A from within your applications."
date: Mon, 25 Oct 2021 13:33:00 +0000
draft: false
url: /2021/10/25/convert-excel-to-pdf-on-linux-using-java/
author: Usman Aziz
summary: "In various cases, you need to convert the Excel spreadsheets to PDF format, for example, to print or share the worksheets. In this article, you'll learn **how to convert Excel files to PDF format on the Linux** platform using Java. Furthermore, you'll come to know about different options to customize the Excel to [PDF][1] conversion."
tags: ['Excel to pdf converter for linux', 'excel to pdf linux', 'xls to pdf linux', 'xlsx to pdf linux']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Convert-Excel-to-PDF.jpg" alt="Convert Excel to PDF Linux">}}


In various cases, you need to convert the Excel spreadsheets to PDF format, for example, to print or share the worksheets. In this article, you'll learn **how to convert Excel files to PDF format on the Linux** platform using Java. Furthermore, you'll come to know about different options to customize the Excel to [PDF][2] conversion.

*   [Excel to PDF Converter API for Linux][3]
*   [Convert Excel XLS/XLSX to PDF][4]
*   [Excel to PDF Conversion with Compliance Option][5]
*   [Convert Range of Excel Sheets to PDF][6]

## Excel to PDF Converter API for Linux {#Java-Excel-to-PDF-Converter-API}

In order to convert Excel files to PDF format, we will use [Aspose.Cells for Java][7]. It is a feature-rich API that lets you create, manipulate, and convert Excel files seamlessly. You can download the API's [JAR][8] or install it using the following Maven configurations.

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
    <artifactId>aspose-cells</artifactId>
    <version>21.9</version>
</dependency>
```

## Convert Excel XLS or XLSX to PDF on Linux {#Convert-Excel-Files-to-PDF-using-Java}

The following are the steps to convert an Excel XLS or XLSX file to PDF on Linux.

*   Load the Excel file using [Workbook][9] class.
*   Convert Excel file to PDF using [Workbook.save(String, SaveFormat)][10] method.

The following code sample shows how to convert XLSX to PDF.

{{< gist aspose-com-gists 2396821770031adfbe82eee1d66854f0 "excel-to-pdf.java" >}}

## Specify Compliance Level in Excel to PDF Conversion {#Convert-Excel-to-PDF-with-Particular-Compliance-using-Java}

PDF format supports various compliance standards such as PDF/A and etc. Aspose.Cells for Java allows specifying the desired PDF compliance level in Excel to PDF conversion. To achieve this, the API provides the [PdfSaveOptions][11] class. The following are the steps to specify the compliance level for the output PDF.

*   Load the Excel file using [Workbook][12] class.
*   Create an instance of the [PdfSaveOptions][13] class and set compliance using [PdfSaveoptions.setCompliance(PdfCompliance)][14] method.
*   Convert Excel file to PDF using [Workbook.save(String, PdfSaveOptions)][15] method.

The following code sample shows how to convert an Excel XLSX file to PDF format with a particular PDF standard.

{{< gist aspose-com-gists 2396821770031adfbe82eee1d66854f0 "excel-to-pdfa.java" >}}

## Convert Specific Excel Sheets to PDF on Linux {#Convert-a-Range-of-Sheets-to-PDF-using-Java}

In certain cases, you may need to convert a range of sheets instead of the whole Excel file. For this, you can specify the range of sheets to be converted using [PdfSaveOptions.setPageIndex(int)][16] and [PdfSaveOptions.setPageCount(int)][17] methods.

The following code sample shows how to convert a range of Excel sheets to PDF.

{{< gist aspose-com-gists 2396821770031adfbe82eee1d66854f0 "excel-to-pdf-sheet-range.java" >}}

## Conclusion

In this article, you have learned how to convert Excel files to PDF on the Linux platform. Moreover, you have seen how to customize Excel to PDF conversion with various options. You can learn more about Aspose.Cells for Java using the [documentation][18]. In case you would have any questions, feel free to let us know via our [forum][19].

## See Also

*   [CSV to Excel or Excel to CSV on Linux using .NET][20]
*   [Create or Edit Excel Files on Linux using .NET][21]
*   [Create or Edit Excel Files on Linux using Java][22]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #Java-Excel-to-PDF-Converter-API
[4]: #Convert-Excel-Files-to-PDF-using-Java
[5]: #Convert-Excel-to-PDF-with-Particular-Compliance-using-Java
[6]: #Convert-a-Range-of-Sheets-to-PDF-using-Java
[7]: https://products.aspose.com/cells/java
[8]: https://downloads.aspose.com/cells/java
[9]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[10]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String,%20int)
[11]: https://apireference.aspose.com/cells/java/com.aspose.cells/PdfSaveOptions
[12]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[13]: https://apireference.aspose.com/cells/java/com.aspose.cells/PdfSaveOptions
[14]: https://apireference.aspose.com/cells/java/com.aspose.cells/pdfsaveoptions#Compliance
[15]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String,%20com.aspose.cells.SaveOptions)
[16]: https://apireference.aspose.com/cells/java/com.aspose.cells/pdfsaveoptions#PageIndex
[17]: https://apireference.aspose.com/cells/java/com.aspose.cells/pdfsaveoptions#PageCount
[18]: https://docs.aspose.com/cells/java/getting-started/
[19]: https://forum.aspose.com/
[20]: https://blog.aspose.com/2021/10/21/csv-to-excel-or-excel-to-csv-on-linux/
[21]: https://blog.aspose.com/2021/10/20/create-or-edit-excel-files-on-linux/
[22]: https://blog.aspose.com/2021/10/08/create-excel-files-on-linux/




