---
title: 'Add VBA Modules to Excel  Workbook in C# with Aspose.Cells for .NET'
date: Mon, 25 May 2015 10:10:53 +0000
draft: false
url: /2015/05/25/add-new-vba-modules-to-the-workbook-and-utilize-improved-chart-creation-approach-with-aspose.cells-for-.net-8.4.2/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


Aspose.Cells for .NET 8.4.2 has been released. This release contains some useful features and other enhancements. The most worth mentioning feature of the release is the support for adding VBA modules to the spreadsheets. If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you to check the complete [Public API Changes][1] section to know what has been changed in the API so far. We have provided a few important features in this month’s release.

## Adding VBA Modules to Excel Spreadsheet in C#

Starting with this release, Aspose.Cells for .NET has provided support for [adding VBA modules to the spreadsheets][2]. Aspose.Cells for .NET 8.4.2 has exposed the VbaModuleCollection.Add method to add a new VBA module to the instance of Workbook. The VbaModuleCollection.Add method accepts a parameter of type of Worksheet to add a worksheet specific module, whereas the existing VbaModule class contains all the module-specific properties.

The following code snippet shows how to add VBA to Excel Workbook in C#.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-ManagingVBAModules-AddVBAModuleOrCode-AddVBAModuleOrCode.cs" >}}

## Improved Chart Creation Mechanism

Aspose.Cells for .NET 8.4.2 has exposed a [simplified mechanism to create charts][3] on the fly. Please note, the conventional means of creating charts involves several steps that may include, but not limited to specifying the series and category axis data ranges separately. With new mechanism, all you have to do is to specify the chart's data range while using the Chart.SetChartDataRange method.

The SetChartDataRange method accepts two parameters, where first parameter is of type String in order to specify the cell area from which to plot the data series. The second parameter is of type Boolean that specifies the plot orientation, that is; whether to plot the chart data series from a range of cell values by row or by columns.

The following code snippet shows how to create a column chart with few lines of code assuming that the chart's plot series data is present on the same worksheet from cell A1 to D4.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-ManageChartsAndShapes-ChartSetupUsingSetChartDataRange-EasyWayToChartSetupUsingSetChartDataRange.cs" >}}

## Other Enhancements and Fixes

In the new version, we have also provided the following new enhancements:

*   Provided [support for IFNA function][4].
*   Added an overloaded version of Cells.CopyColumns method that can be used to repeat the source columns onto the destination while copy operation.
*   Exposed 2 new fields for the PasteType enumeration in order to mimic the Excel's 'All' & 'All except borders' functionality for pasting range of cells.

For more details on the above enhancements, please see the document [Public API Changes in Aspose.Cells 8.4.2][5].

We have fixed a few exceptions that occurred while reading and writing Microsoft Excel file formats, rendering Excel spreadsheets to PDF format and rendering images from worksheets in the workbook.

In this release, several important issues have been addressed. For example, issues around reading/ writing Microsoft Excel file formats, deleting rows, retrieving data validation applied on the cells, manipulating list objects/ tables, rendering to HTML file format, manipulating drawing objects and shapes, [rendering images from Excel worksheets][6], manipulating charts with formatting, [rendering images files from charts][7] and [exporting Excel workbooks to PDF format][8] have been resolved. We have also enhanced the Aspose.Cells formula calculation engine and fixed a few relevant issues in this release.

We have also figured out a few issues posted by the users in the web-based Grid control by Aspose.Cells for .NET.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 8.4.2, please visit the [download page][9].




[1]: http://docs.aspose.com/display/cellsnet/Migrating+from+Earlier+Versions+of+Aspose.Cells
[2]: http://docs.aspose.com/display/cellsnet/Adding+VBA+Module+and+Code+using+Aspose.Cells
[3]: http://docs.aspose.com/display/cellsnet/Easy+way+for+Chart+Setup+using+Chart.SetChartDataRange+method
[4]: http://docs.aspose.com/display/cellsnet/Calculating+IFNA+function+using+Aspose.Cells
[5]: http://docs.aspose.com/display/cellsnet/Public+API+Changes+in+Aspose.Cells+8.4.2
[6]: http://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Image
[7]: https://docs.aspose.com/display/cellsnet/Convert+an+Excel+Chart+to+Image
[8]: http://docs.aspose.com/display/cellsnet/Converting+Excel+to+PDF+Files
[9]: https://downloads.aspose.com/cells/net




