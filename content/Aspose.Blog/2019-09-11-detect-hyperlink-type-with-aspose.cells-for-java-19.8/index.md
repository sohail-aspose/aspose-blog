---
title: 'Detect Hyperlink Type in Excel Spreadsheets using Java'
date: Wed, 11 Sep 2019 14:07:33 +0000
draft: false
url: /2019/09/11/detect-hyperlink-type-with-aspose.cells-for-java-19.8/
author: Ahsaniqbal
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose_cells-for-java-e1558954178996.jpg" alt="">}}


You get a list of hyperlinks from an Excel file and now thinking about how to categorise them into different types in order to select the appropriate method for processing each of them. Don't panic! [Aspose.Cells for Java 19.8][1] is released containing the solution for this problem. This is not the only feature introduced in this release but there are many more to explore like extracting embedded MOL file, getting total page count before converting to PDF/Image, inserting SVG file into a worksheet and supporting Java 12 are just a few to list here. You may have a look at the [release notes][2] to get the complete list of features and bug fixes which are part of this new release. Let us see in detail what are these features and how to use them.

## Detect Hyperlink Type in Spreadsheet

There can be different types of hyperlinks that can be used in an Excel file like external, cell reference, file path and email. Our new release has introduced an enumerator [TargetModeType][3] which represents the type of hyperlink. A new property [LinkType][4] is introduced in Hyperlink class which return the hyperlink type using above mentioned enumerator. Following are the enumerator members:

*   [EXTERNAL][5]: External link
*   [FILE\_PATH][6]: Local and full path to files\\folders.
*   [EMAIL][7]: Email
*   [CELL\_REFERENCE][8]: Link to cell or named range.

Here is an example which can be used to exercise this new feature. Also for more details visit [here][9].

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-Workbook-DetectLinkTypes-1.java" >}}



{{< figure align=center src="images/Screenshot-2019-09-03-at-8.43.27-PM-1024x446.png" alt="" caption="Program output vs template Excel file">}}


## Get Total Page Count Before PDF/image Creation

Well, the title is explaining this new feature. When a file has too many pages, the process of converting to pdf/image may use too much memory and CPU, and OOM exception may be thrown. Getting total page count before converting can indicate this risk, and do some actions(e.g. skip this file) or print the selected pages to avoid the undesired results. For example one of my sample Excel file (870 KB) was showing about 38 million pages. Just imagine, what will happen if you come across a conversion containing such a huge number of pages!!! Following is an example to show the usage of new classes SheetPrintingPreview and WorkbookPrintingPreview. Both of these classes contain a property EvaluatedPageCount which returns the page count of the printout or PDF file. Here is an [article][10] which provides more details in this regard.

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-Workbook-PrintPreview-1.java" >}}

## Extracting Embedded MOL File

As you know that molecular data file created in the MDL Molfile format, a chemical file format; contains plain text information and stores information about atoms and bonds; often used as a standard exchange format for molecular information. This type of file can be embedded in the Excel file. In this latest release, support is provided to extract object of such an uncommon type i.e. MOL. The following code snippet demonstrates extracting embedded MOL file and saving it to disk. For more details and sample file please visit [here][11].

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-Workbook-ExtractEmbeddedMolFile-1.java" >}}

## Other Features and Enhancements

*   Support for Java 12 is available now
*   Enhancements to avoid high CPU and memory usage during Excel to PDF conversion
*   Copying waterfall chart style while copying the workbook
*   Proper refreshing of PivotTable and PivotCharts
*   Avoid differences during conversion to HTML
*   Remove unwanted extended borderline in Excel to PDF rendering
*   Calculate appropriate image position while rendering to PDF
*   Ensure copying table properties while using copyColumns() function
*   Keep the image transparent instead of opaque during picture copy

The wait is over and you may get ready to test the new features. Following resources may help you to achieve your targets using Aspose.Cells.

*   [Developer's Guide][12]
*   [Code Samples][13]
*   [Forums][14]




[1]: https://downloads.aspose.com/cells/java/new-releases/aspose.cells-for-java-19.8/
[2]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+19.8+Release+Notes
[3]: https://apireference.aspose.com/java/cells/com.aspose.cells/TargetModeType
[4]: https://apireference.aspose.com/java/cells/com.aspose.cells/hyperlink#LinkType
[5]: https://apireference.aspose.com/java/cells/com.aspose.cells/targetmodetype#EXTERNAL
[6]: https://apireference.aspose.com/java/cells/com.aspose.cells/targetmodetype#FILE_PATH
[7]: https://apireference.aspose.com/java/cells/com.aspose.cells/targetmodetype#EMAIL
[8]: https://apireference.aspose.com/java/cells/com.aspose.cells/targetmodetype#CELL_REFERENCE
[9]: https://docs.aspose.com/display/cellsjava/Detect+Hyperlink+Type
[10]: https://docs.aspose.com/display/cellsjava/Workbook+and+Worksheet+Print+Preview
[11]: https://docs.aspose.com/display/cellsjava/Managing+OLE+Objects#ManagingOLEObjects-ExtractingEmbeddedMOLFile
[12]: https://docs.aspose.com/display/cellsjava/Developer+Guide
[13]: https://github.com/aspose-cells/Aspose.Cells-for-Java
[14]: https://forum.aspose.com/c/cells




