---
title: 'Calculate the Width and Height of the Cell Value and Get an Array of Values from ICustomFunction using Aspose.Cells for .NET 8.5.1'
date: Mon, 27 Jul 2015 09:08:06 +0000
draft: false
url: /2015/07/27/calculate-the-width-and-height-of-the-cell-value-and-get-an-array-of-values-from-icustomfunction-using-aspose.cells-for-.net-8.5.1/
author: Amjad Sahi
summary: ''
tags: ['Aspose.Cells for .NET', 'Set Cell Size in Excel', 'Set Excel Row Height Column Width', 'calculate excel cell size', 'calculate the size of a Excel cell']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


Aspose.Cells for .NET 8.5.1 has been released. This release contains some useful features and other enhancements along with some critical bug fixes. If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you to check the complete Public API Changes section to know what has been changed in the API so far. We have provided a few important features in this month’s release.

## Calculate the Width and Height of the Cell Value in Excel

Aspose.Cells for .NET provides Cell.GetWidthOfValue and Cell.GetHeightOfValue methods to calculate the width & height of the cell value in the unit of pixels. These methods are useful in scenarios where application requirement is to set the width of the column and height of the row according to the size of cell value.

The following sample code explains the usage of Cell.GetWidthOfValue and Cell.GetHeightOfValue methods.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-ManagingRowsColumnsCells-CalculateWidthAndHeight-CalculateWidthAndHeightOfCellValueInUnitOfPixel.cs" >}}

## Get a Range of Values using ICustomFunction

Aspose.Cells APIs provide the ICustomFunction interface which can be used to implement the user defined or custom functions that are not supported by Microsoft Excel as built-in functions. While implementing the ICustomFunction interface, most of the times we require to return a single cell value however, sometimes we may also need to return a range of values.

Following code snippet demonstrates how to return a range of values from ICustomFunction.

{{< gist aspose-cells c326c6c668fc372e30569fa9e0f6bf4b "Examples-CSharp-Articles-WorkingWithCalculationEngine-ReturnRangeOfValuesUsingICustomFunction-CustomFunctionStaticValue.cs" >}}

{{< gist aspose-cells c326c6c668fc372e30569fa9e0f6bf4b "Examples-CSharp-Articles-WorkingWithCalculationEngine-ReturnRangeOfValuesUsingICustomFunction-1.cs" >}}

## Release Unmanaged Resources of Workbook

Aspose.Cells for .NET 8.5.1 has exposed the Workbook.Dispose() method to release the unmanaged resources of the Workbook object. The dispose pattern is used only for objects that access unmanaged resources, such as file and pipe handles, registry handles, wait handles, or pointers to blocks of unmanaged memory. This is because the garbage collector is very efficient at reclaiming unused managed objects, but it is unable to reclaim unmanaged objects.

## Detect the Data Source Type of ListObject

With this revision, the API has exposed the TableDataSourceType enumeration & readonly ListObject.DataSourceType property that can be used to detect the data source type of a ListObject.

The TableDataSourceType enumeration has the following fields.

*   TableDataSourceType.QueryTable
*   TableDataSourceType.XML
*   TableDataSourceType.Worksheet
*   TableDataSourceType.SharePoint

## Other Enhancements and Fixes

In the new version, we have also provided the following enhancements:

*   Provided support to link to external workbooks in the desktop grid control provided by Aspose.Cells for .NET.
*   Support Right-to-Left Display of Worksheets in desktop grid control provided by Aspose.Cells for .NET.

We have handled some exceptions when reading/writing Excel spreadsheets and copying worksheets from other workbook. We have also fixed an exception in Shape to Image rendering.

In this release, several important issues have been addressed. For example, issues around reading/ writing Microsoft Excel file formats, manipulating Pivot Tables, combining workbooks, setting conditional formatting, protecting workbooks, manipulating drawing objects and shapes, rendering images from Excel worksheets, manipulating charts with formatting, [rendering images files from charts][1] and exporting Excel workbooks to PDF format have been resolved. We have also enhanced the Aspose.Cells formula calculation engine and fixed a few issues in this regard.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 8.5.1, please visit the [download page][2].




[1]: https://docs.aspose.com/display/cellsnet/Convert+Chart+to+Images
[2]: https://downloads.aspose.com/cells/net




