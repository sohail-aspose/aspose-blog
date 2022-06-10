---
title: 'Export Microsoft Excel Charts to PDF and Rotate Text with Shape in Excel using Java'
date: Sat, 05 May 2018 01:27:51 +0000
draft: false
url: /2018/05/05/export-microsoft-excel-charts-to-pdf-in-java/
author: Mshakeel Faiz
summary: ''
tags: ['Muhammad Shakeel Faiz', 'Export Excel Charts to PDF in Java', 'Save Charts in Excel as PDF in Java']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We are pleased to announce the release of [Aspose.Cells for Java 18.4][1]. This release includes many new features and enhancements along with some critical bug fixes that further improve the overall stability of the APIs. We also recommend our clients to use the powerful Aspose for Java APIs directly in their Maven Projects with simple configurations. Please check the [release notes][2] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Java. Here is a look at the major features in this release.

## Export Excel Chart to PDF with Desired Page Size in Java

You can create a chart's PDF file with your desired page size using Aspose.Cells and specify how you want to align the chart inside the page like top, bottom, center, left, right, etc. Besides this, the output chart can be created in a stream or on disk. 

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Charts-CreateChartPDFWithDesiredPageSize.java" >}}

### Output



{{< figure align=center src="images/Create-Chart-PDF-With-Desired-Page-Size.png" alt="Save Excel Chart as PDF in Java">}}


Please see the following article for more detail on this topic.

*   [Create Chart PDF with Desired Page Size][3]

## Rotate Text with Shape Inside the Worksheet

You can add text inside any shape using Microsoft Excel. If you add shape using the older Microsoft Excel 2003, then the text will not rotate with shape. But if you add shape using newer versions of Microsoft Excel e.g. 2007, 2010, 2013 or 2016, etc. then the text will be rotated with shape. You can control if the text should rotate with the shape or not using the **ShapeTextAlignment.RotateTextWithShape** property.

*   [Rotate Text with Shape inside the Worksheet][4]

## Read/Write TSV (Tab-Separated Values) Files

TSV files are used to contain spreadsheet data but without any formatting. The format is the same as Tab Delimited where data is arranged in rows and columns such as tables and spreadsheets. To open tab-delimited files, developers should call the **LoadOptions** method and select the **TSV** value, predefined in the **FileFormatType** enumeration. Please see the following sample code and the related article for your reference.

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-Files-Handling-OpeningTSVFiles-1.java" >}}

*   [Opening Tab-Separated Values (TSV) Files][5]Files)

## Get All Hidden Rows Indices after Refreshing AutoFilter

When you apply the auto filter on worksheet cells, then some of the rows get hidden automatically. But it might be the case that some of the rows are already hidden manually by MS Excel end user and they are not hidden by auto filter feature. It, therefore, makes difficult to know which of the rows are hidden by the auto filter and which rows are hidden manually by MS Excel end user. Aspose.Cells deals with this problem using the int\[\] AutoFilter.refresh(boolean hideRows) method. This method returns the row indices of all the rows that are hidden by the auto filter and not by the manual way in MS Excel.

*   [Get All Hidden Rows Indices after Refreshing AutoFilter][6]

## Avoid Blank Page in Output PDF

When the Excel file is empty and the user saves it to PDF using Aspose.Cells, it renders the blank page in output PDF. Sometimes, this default behavior is undesirable. Aspose.Cells provides the **PdfSaveOptions.OutputBlankPageWhenNothingToPrint** property to deal with this issue. If you will set it as false, then CellsException will occur whenever there is nothing to print in the output PDF.

*   [Avoid Blank Page in Output Pdf when there is Nothing to Print][7]

## Find Type of X and Y Values of Points in Chart Series

Sometimes, you want to know the type of X and Y values of chart points in a series. Aspose.Cells provides **ChartPoint.XValueType** and **ChartPoint.YValueType** properties that can be used for this purpose. Please note, you will have to call **Chart.calculate()** method before you could use these properties effectively.

*   [Find Type of X and Y Values of Points in Chart Series][8]

## Get HTML5 String from Cell

Aspose.Cells returns the HTML string of the cell using the string **Cell.getHtmlString (boolean html5)** method. If you pass "false" as the parameter, it will return you Normal HTML but if you pass "true" as the parameter, it will return Html5 string.

*   [Get HTML5 string from Cell][9]

## Hiding Overlaid Content with CrossHideRight while Saving to HTML

When you save your MS Excel file to HTML, you can specify different cross types for cell strings. By default, Aspose.Cells generates HTML as per Microsoft Excel but when you change cross-type to **CrossHideRight** then it hides all the strings from the right side of the cell which are overlaid or overlapping with cell string.

*   Hiding Overlaid Content with CrossHideRight while saving to Html

## Specify the Language of the Excel File using Built-In Document Properties

You can change the Language of MS Excel file by right-clicking the file and then selecting Properties > Details and then editing the Language field. Please use **BuiltInDocumentPropertyCollection.Language** property to change it programmatically using Aspose.Cells APIs.

*   [Specify the Language of the Excel File using BuiltIn Document Properties][10]

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][11].
*   [Download Aspose.Cells for Java][12].
*   [Aspose.Cells for Java Documentation][13] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][14] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][15] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for Java Examples][16] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://artifact.aspose.com/repo/com/aspose/aspose-cells/18.4/
[2]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+18.4+Release+Notes
[3]: https://docs.aspose.com/display/cellsjava/Create+Chart+PDF+with+Desired+Page+Size
[4]: https://docs.aspose.com/display/cellsjava/Rotate+Text+with+Shape+inside+the+Worksheet
[5]: https://docs.aspose.com/display/cellsjava/Opening+Files+with+Different+Formats#OpeningFileswithDifferentFormats-OpeningTab-SeparatedValues(TSV
[6]: https://docs.aspose.com/display/cellsjava/Get+All+Hidden+Rows+Indices+after+Refreshing+AutoFilter
[7]: https://docs.aspose.com/display/cellsjava/Avoid+Blank+Page+in+Output+Pdf+when+there+is+Nothing+to+Print
[8]: https://docs.aspose.com/display/cellsjava/Find+Type+of+X+and+Y+Values+of+Points+in+Chart+Series
[9]: https://docs.aspose.com/display/cellsjava/Get+HTML5+string+from+Cell
[10]: https://docs.aspose.com/display/cellsjava/Specify+the+Language+of+the+Excel+File+using+BuiltIn+Document+Properties
[11]: https://products.aspose.com/cells/java
[12]: https://artifact.aspose.com/repo/com/aspose/aspose-cells/
[13]: https://docs.aspose.com/display/cellsjava/home
[14]: https://apireference.aspose.com/java/cells
[15]: https://forum.aspose.com/c/cells
[16]: https://github.com/aspose-cells/Aspose.Cells-for-Java




