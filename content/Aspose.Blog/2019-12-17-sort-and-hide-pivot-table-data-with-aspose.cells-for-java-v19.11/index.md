---
title: 'Sort and Hide Pivot Table Data in Excel using Java'
date: Tue, 17 Dec 2019 16:04:30 +0000
draft: false
url: /2019/12/17/sort-and-hide-pivot-table-data-with-aspose.cells-for-java-v19.11/
author: Ahsaniqbal
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose_cells-for-java-e1558954178996.jpg" alt="This image has an empty alt attribute; its file name is aspose_cells-for-java-e1558954178996.jpg">}}


[Aspose.Cells for Java v19.11][1] is released which contains many new features and upgrades. Pivot tables processing is enhanced by providing the sorting and hiding data based upon some criteria to get compact information for reporting and presentations. Reading and writing to tables with QueryTable as a data source is available now. This is not the end of this release but the beginning of a long list of new features like modifying the existing validation by adding CellArea, retrieving OData connection information and getting text width of cell value for better layouts. All the details of this release can be found in the [release notes][2] published with every new release. Let us have a look at these new exciting features one by one.

## Sort and Hide Data in Excel Pivot Table using Java

There are cases where crisp information is required in the pivot table. We may require some features to sort data in the pivot table and then hide rows against certain criteria. Following sample code demonstrates this feature

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-PivotTables-PivotTableSortAndHide-1.java" >}}

The following image shows the pivot table before and after running this code on a sample data.



{{< figure align=center src="images/PivotTableSortHide.png" alt="">}}


Visit the following article for more information and sample files.

*   [Pivot table hide and sort data][3]

## Read and Write Table with Query Table Data Source

Tables having a query table as a data source are very common. We may require to read such tables and modify them like showing the total etc. Earlier this feature was available however support for XLS file is provided. Here is an example code which reads a table and then changes it to show the total at the end.

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-Tables-ReadAndWriteTableWithQueryTableDataSource-1.java" >}}

The following image shows how setShowTotals() function works:



{{< figure align=center src="images/QueryTable.png" alt="">}}


You may get the sample files and more details in the following article:

*   [Read and write table with query table data source][4]

## Fetch OData Connection Information

OData can be used to get the feed or data from RESTful API which can be used in Excel file as well. This information can be retrieved from the Excel file using Apose.Cells API using DataMashup class of Workbook. Get the desired information from PowerQueryFormulas property having PowerQueryFormula and PowerQueryFormulaItem.

The following code snippet demonstrates the use of these classes to retrieve the OData information.

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-Workbook-GetOdataDetails-1.java" >}}

The following image shows a sample file that is used in the above code sample to fetch the OData connection information.



{{< figure align=center src="images/OData-1024x562.png" alt="">}}


Here is the program output using the sample file:



{{< figure align=center src="images/Screenshot-2019-12-16-at-6.01.00-AM-1024x262.png" alt="">}}


This article contains a sample file and more details to check this feature:

*   [How to get OData connection information][5]

## Add CellArea to Existing Validation

Suppose that you have an Excel file that has [validation][6] which is working fine. Aspose.Cells always performs a check to verify if the area is already there or not whenever a cell area is added to validation. You may face performance hit during this check if there are a large number of validations in your Excel file. To handle this issue, there is a need to configure the API to get control over performing this check. [Validation.AddAreaCellArea cellArea, bool checkIntersection, bool checkEdge)][7] method is there to get this control as the parameter _checkIntersection_ directs the API to check the intersection of this newly added area with existing areas. If you set this parameter to false, the checking for other areas will be disabled. If you want to check the applied areas, set the _checkEdge _parameter to true. Note that internal settings are rebuilt if the top-left area is reset to the new area. However, if you are sure that new area is not the top-left area, then set the value of the property checkEdge to false.

You may give a try to the following sample code which demonstrates adding new CellArea to a validation which already exists there in the Excel file.

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-Data-AddValidationArea-1.java" >}}

Have a look at the following article for more details and sample file to test this feature.

*   [Add CellArea to existing validation][8]

## Get Text Width of Cell Value

Better data presentation layout is the target of every developer. For this support is required in the API to calculate the cell width when formatting the reports/presentations. To assist the developers, Aspose.Cells provides a function GetTextWidth() in the CellsHelper class. Using this function developer will get the text width in a cell, based upon the text length and style. Following sample code demonstrates the usage of [CellsHelper.GetTextWidth][9]by getting the text width of the value in a cell.

The following sample code demonstrates this feature:

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-CellsHelperClass-GetTextWidth-1.java" >}}

You may download the sample file here.

## Other Enhancements

Following are a few enhancements and improvements which are made in this release:

*   Cells.importCSV function is improved to avoid exception "string value cannot exceed 255 characters"
*   Improvement is made in the performance of Cells.removeDupilcates for large dataset
*   Radial graph rendering to HTML is improved
*   More accuracy is added to scaling of the axis during rendition to PNG
*   Enhancements are made to avoid corruption after updating the source data for a pivot table.
*   Get more accurate Russian (custom) date format output using this release
*   LoadFilter is made error-free to consider the required sheet
*   Proper borders are maintained while converting Excel file to EMF
*   SheetRender improved to provide a more accurate page count
*   Rendering of the chart to an image is enhanced. You will get Data Labels with the same style and proper values in the output image
*   Cell.setHtmlString() function improved for processing hyperlinks and HTML tags/scripts.

Following are few important resources which can be referred to while testing the new release:

*   [Developer's Guide][10]
*   [Code Samples][11]
*   [Forums﻿][12]




[1]: https://downloads.aspose.com/cells/java/new-releases/aspose.cells-for-java-19.11/
[2]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+19.11+Release+Notes
[3]: https://docs.aspose.com/display/cellsjava/Pivot+Table+Hide+and+Sort+data
[4]: https://docs.aspose.com/display/cellsjava/Read+and+Write+Table+with+Query+Table+Data+Source
[5]: https://docs.aspose.com/display/cellsjava/How+to+get+OData+Connection+Information
[6]: https://apireference.aspose.com/java/cells/com.aspose.cells/Validation
[7]: https://apireference.aspose.com/java/cells/com.aspose.cells/validation#addArea(com.aspose.cells.CellArea,%20boolean,%20boolean)
[8]: https://docs.aspose.com/display/cellsjava/Data+Validation#DataValidation-AddCellAreatoexistingValidation
[9]: https://apireference.aspose.com/java/cells/com.aspose.cells/cellshelper#getTextWidth(java.lang.String,%20com.aspose.cells.Font,%20double)
[10]: https://docs.aspose.com/display/cellsjava/Developer+Guide
[11]: https://github.com/aspose-cells/Aspose.Cells-for-Java
[12]: https://forum.aspose.com/c/cells




