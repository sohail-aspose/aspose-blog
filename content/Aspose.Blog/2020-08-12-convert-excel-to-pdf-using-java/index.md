---
title: 'Convert Excel Files to PDF using Java'
seoTitle: "Convert Excel to PDF using Java | Convert XLSX or XLS to PDF in Java"
description: "Convert MS Excel files to PDF using Java Excel to PDF converter API. Convert XLSX to PDF or XLS to PDF or PDF/A from within your Java applications."
date: Wed, 12 Aug 2020 20:37:06 +0000
draft: false
url: /2020/08/12/convert-excel-to-pdf-using-java/
author: Usman Aziz
summary: ''
tags: ['XLSX to PDF using Java', 'convert excel to pdf using java', 'excel to pdfa using java', 'xls to pdf using java']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Convert-Excel-to-PDF.jpg" alt="Convert Excel to PDF Java">}}


Excel to PDF conversion might be required in various scenarios for exporting tabular data from worksheets to PDF pages. In this article, you'll learn how to **convert Excel files to PDF using Java** in order to automate XLS/XLSX to PDF conversion within your web or desktop applications.

*   [Java Excel to PDF Converter API - Installation][1]
*   [Convert Excel XLS/XLSX to PDF using Java][2]
*   [Convert Excel to PDF with Particular Compliance using Java][3]
*   [Render One PDF Page Per Sheet using Java][4]
*   [Convert a Range of Sheets to PDF using Java][5]

## Java Excel to PDF Converter API - Installation {#Java-Excel-to-PDF-Converter-API}

[Aspose.Cells for Java][6] is a well-known spreadsheet processing API that lets you create, manipulate, and convert Excel XLS/XLSX and other spreadsheet formats quite easily. With a few lines of code and easy to use methods, you can perform quality Excel to PDF conversion with high fidelity. Aspose.Cells for Java can be downloaded as [JAR][7] or installed using the following Maven configurations.

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
    <artifactId>aspose-cells</artifactId>
    <version>20.7</version>
</dependency>
```

## Convert Excel XLS/XLSX to PDF using Java {#Convert-Excel-Files-to-PDF-using-Java}

The following are the steps to convert an Excel XLS or XLSX file to PDF using Aspose.Cells for Java API. The links to API references let you explore more about the classes and methods of the API.

*   Create an object of [Workbook][8] class and initialize it with the path to Excel file.
*   Save the Excel file as PDF using [Workbook.save(String, SaveFormat)][9] method.

The following code sample shows how to convert XLSX to PDF using Java.

{{< gist aspose-com-gists 2396821770031adfbe82eee1d66854f0 "excel-to-pdf.java" >}}

## Convert Excel to PDF with Particular Compliance using Java {#Convert-Excel-to-PDF-with-Particular-Compliance-using-Java}

PDF format supports various compliance standards such as PDF/A and etc. Being compliant with a particular standard means that the file fulfills the requirements or rules defined in that standard. In order to convert Excel to PDF with a particular compliance standard, you can use the [PdfSaveOptions][10] class. The following are the steps to set a particular compliance standard for the output PDF.

*   Initialize [Workbook][11] object with the Excel file's path.
*   Create an instance of the [PdfSaveOptions][12] class.
*   Set the compliance using [PdfSaveoptions.setCompliance(PdfCompliance)][13] method.
*   Save the Excel file as PDF using [Workbook.save(String, PdfSaveOptions)][14] method.

The following code sample shows how to convert XLSX to PDF with a particular PDF standard using Java.

{{< gist aspose-com-gists 2396821770031adfbe82eee1d66854f0 "excel-to-pdfa.java" >}}

## Excel to PDF with One Page Per Sheet Settings using Java {#Excel-to-PDF-with-One-Page-Per-Sheet-Settings-using-Java}

By default, the API renders the worksheets according to the page size in the PDF document. In this case, one worksheet can possibly be rendered on multiple pages in the PDF. In order to override this operation, you can configure the API to render all the content of a worksheet on one page using [PdfSaveOptions.setOnePagePerSheet(boolean)][15] method.

The following code sample shows how to convert XLSX to PDF with one page per sheet settings using Java.

{{< gist aspose-com-gists 2396821770031adfbe82eee1d66854f0 "excel-to-pdf-one-page-per-sheet.java" >}}

## Convert a Range of Sheets to PDF using Java {#Convert-a-Range-of-Sheets-to-PDF-using-Java}

In certain cases, you may need to convert only a selective range of the Excel sheets instead of the whole workbook. In such a case, you can tell the API about the range of the sheets to be included in the rendering process using [PdfSaveOptions.setPageIndex(int)][16] and [PdfSaveOptions.setPageCount(int)][17] methods.

The following code sample shows how to render a range of sheets to PDF using Java.

{{< gist aspose-com-gists 2396821770031adfbe82eee1d66854f0 "excel-to-pdf-sheet-range.java" >}}

## Conclusion

In this article, you have learned how to convert Excel files to PDF using Java. Furthermore, you have seen how to customize Excel to PDF conversion in various scenarios. You can learn more about Aspose.Cells for Java using the [documentation][18].

## See Also

*   [Convert Excel to PDF using C#][19]




[1]: #Java-Excel-to-PDF-Converter-API
[2]: #Convert-Excel-Files-to-PDF-using-Java
[3]: #Convert-Excel-to-PDF-with-Particular-Compliance-using-Java
[4]: #Excel-to-PDF-with-One-Page-Per-Sheet-Settings-using-Java
[5]: #Convert-a-Range-of-Sheets-to-PDF-using-Java
[6]: https://products.aspose.com/cells/java
[7]: https://downloads.aspose.com/cells/java
[8]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[9]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String,%20int)
[10]: https://apireference.aspose.com/cells/java/com.aspose.cells/PdfSaveOptions
[11]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[12]: https://apireference.aspose.com/cells/java/com.aspose.cells/PdfSaveOptions
[13]: https://apireference.aspose.com/cells/java/com.aspose.cells/pdfsaveoptions#Compliance
[14]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String,%20com.aspose.cells.SaveOptions)
[15]: https://apireference.aspose.com/cells/java/com.aspose.cells/pdfsaveoptions#OnePagePerSheet
[16]: https://apireference.aspose.com/cells/java/com.aspose.cells/pdfsaveoptions#PageIndex
[17]: https://apireference.aspose.com/cells/java/com.aspose.cells/pdfsaveoptions#PageCount
[18]: https://docs.aspose.com/cells/java/getting-started/
[19]: https://blog.aspose.com/2019/11/29/convert-xls-and-xlsx-to-pdf-in-c/





