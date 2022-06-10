---
title: 'Optimize PDF File Size in Excel to PDF using Java'
date: Tue, 02 Feb 2016 10:07:21 +0000
draft: false
url: /2016/02/02/optimize-pdf-file-size-re-size-charts-data-label-shape-to-fit-text-enhancements-to-protection-module-with-aspose.cells-for-java-8.7.0/
author: Babar Raza
summary: ''
tags: ['Babar Raza', 'Convert to PDF', 'Excel Spreadsheets', 'Excel files API', 'Import CSV', 'Import XML Map', 'Java Excel APIs', 'Macro Protection', 'Protect Worksheet', 'Resize shape to fit text', 'Sign VBA', 'minimize the PDF file size']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


Aspose.Cells for Java API has been upgraded to 8.7.0, and we are pleased to announce, this month's release contains many useful features and improvements along with some critical bug fixes. Please refer to the release notes of [Aspose.Cells for Java 8.7.0][1] for a full list of enhancements. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the Public API Changes section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Excel to PDF - Optimize PDF File Size

Aspose.Cells APIs have provided an enhancement for the PDF rendering engine in order to reduce the resultant PDF file size. Aspose.Cells for Java 8.7.0 has exposed the PdfSaveOptions.OptimizationType property along with an enumeration by the name PdfOptimizationType in order to facilitate the application developers to control the resultant PDF file size to some extent.

The PdfOptimizationType enumeration has 2 constants at the moment exhibiting the following behaviour.

1.  PdfOptimizationType.MINIMUM\_SIZE: API tries to optimize the cell text and cell border records in order to reduce the resultant PDF file size.
2.  PdfOptimizationType.STANDARD: No optimization is done therefore the resultant file size will be large as compared to PdfOptimizationType.MINIMUM\_SIZE selection.

The following piece of code demonstrates the usage of PdfSaveOptions.OptimizationType property to [minimize the resultant PDF file size][2] while exporting spreadsheets to PDF format.

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-SaveExcelToPDF-SaveExcelToPDF.java" >}}

## Re-size Chart's Data Label Shape to Fit Text

Aspose.Cells for Java 8.7.0 has exposed the boolean type DataLabels.ResizeShapeToFitText property in order to mimic the Excel's feature of re-sizing data label shapes to fit the text.

Please note, Excel application provides the **Resize shape to fit text** option for chart's data labels to increase the size of the shape so that the text fits inside of it. This option can be accessed on Excel interface by selecting any of the data labels on the chart. Right click and select **Format DataLabels** menu. On **Size & Properties** tab, expand **Alignment** node to reveal the related properties including the **Resize shape to fix text** option as highlighted below.



{{< figure align=center src="images/Excel-Resize-Shape-To-Fit-Text.png" alt="">}}


The following piece of code shows the simple usage scenario of DataLabels.ResizeShapeToFitText property to re-size the chart's data label shapes to fit text.

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-ResizeChartDataLabelShapeToFitText-ResizeChartDataLabelShapeToFitText.java" >}}

Here is a snapshot showing a simple bar chart before & after executing the above code.



{{< figure align=center src="images/chart-resize-datalabel-shape-to-fit-text.png" alt="">}}


## Enhancements to Protection Module

Aspose.Cells APIs have enhanced the Protection class by introducing some useful properties & methods. Two of the most worth mentioning enhancements are as follow.

### Detect if Worksheet is Password Protected

It is possible to protect the workbooks and worksheets separately. For instance, a spreadsheet may contain one or more worksheets that are password protected, however, the spreadsheet itself may or may not be protected. Aspose.Cells API for Java has provided the Protection.isProtectedWithPassword field to [detect if a worksheet is password protected][3]. Boolean type Protection.isProtectedWithPassword field returns true if Worksheet is password protected and false if not.

### Verify Password Used to Protect the Worksheet

Aspose.Cells for Java 8.7.0 has exposed the Protection.verifyPassword method which allows to specify a password as an instance of String and [verifies if same password has been used to protect the worksheet][4]. The Protection.verifyPassword method returns true if the specified password matches with the password used to protect the given Worksheet, false if the specified password does not match.

The following piece of code uses the Protection.verifyPassword method in conjunction with Protection.isProtectedWithPassword field to detect password protection and verifies the password.

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-VerifyPasswordtoProtectWorksheet-VerifyPasswordtoProtectWorksheet.java" >}}

## Load or Import Delimited File Containing Formulas

Aspose.Cells for Java has provided support to identify & parse the formulas while loading CSV/TXT files having delimited plain data. Newly exposed TxtLoadOptions.HasFormula property when set to true directs the API to parse the formulas from the input delimited file and set them to relevant cells without requiring any additional processing.

The following piece of code demonstrates the usage of TxtLoadOptions.HasFormula property to [load and import the CSV with formulas in it][5].

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-LoadOrImportCSVFile-LoadOrImportCSVFile.java" >}}

## Create 2-Color Scale Conditional Format

This release of the API has has exposed the ColorScale.Is3ColorScale property that can be used to create 2-Color Scale conditional format. The said property is of type boolean with default value of true which means that the conditional format will be of 3-Color Scale by default. However, switching the ColorScale.Is3ColorScale property to false will generate a 2-Color Scale conditional format.

Following is the simple usage scenario to generate 2-color scale conditional format. Please also review the detailed article on Adding 2 & 3-Color Scale Conditional Formatting.

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-AddingTwoAndThreeColorScale-AddingTwoAndThreeColorScale.java" >}}

## Other Enhancements & Improvements

The most notable enhancements in this release are as follow:

*   Newly exposed field VbaProject.isSigned allows to detect if a given VbaProject is digitally signed or not.
*   This release has added support for importing XML map inside an instance of Workbook.
*   Enhanced the PDF rending engine to maximize the fidelity for the Excel Chart objects.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][6].
*   [Aspose.Cells for Java Download Section][7].
*   Aspose.Cells for Java Documentation – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][8] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][9] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][10] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Java Examples][11] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/java
[2]: https://docs.aspose.com/display/cellsjava/Save+Excel+into+PDF+with+Standard+or+Minimum+Size
[3]: https://docs.aspose.com/display/cellsjava/Detect+if+Worksheet+is+Password+Protected
[4]: https://docs.aspose.com/display/cellsjava/Verify+Password+Used+to+Protect+the+Worksheet
[5]: https://docs.aspose.com/display/cellsjava/Load+or+Import+CSV+file+with+Formulas
[6]: https://products.aspose.com/cells/java
[7]: https://downloads.aspose.com/cells/java
[8]: http://www.aspose.com/api/java/cells/com.aspose.cells/index
[9]: https://forum.aspose.com/
[10]: https://blog.aspose.com/
[11]: https://github.com/asposecells/Aspose_Cells_Java




