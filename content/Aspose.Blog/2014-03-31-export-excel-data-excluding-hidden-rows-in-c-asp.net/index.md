---
title: 'Export Excel Data Excluding Hidden Rows in C# using Aspose.Cells for .NET'
date: Mon, 31 Mar 2014 19:24:36 +0000
draft: false
url: /2014/03/31/export-excel-data-excluding-hidden-rows-in-c-asp.net/
author: Amjad Sahi
summary: ''
tags: ['Calculate Excel formulas', 'Excel Files', 'advanced conditional formatting', 'export Excel workbooks to PDF', 'manipulate PivotTables', 'render MS Excel file formats', 'render images files from Charts', 'rendering Charts']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


Aspose.Cells for .NET 8.0.0 has been released. This new release supports optimizing memory use when working with big Microsoft Excel files that have large data sets. When building a workbook with a large data set, or reading a big template file, the total amount of RAM the process will take is always a concern. Aspose.Cells provide measures to cope with this challenge. Aspose.Cells provides relevant options and API calls to lower, reduce and optimize memory usage accordingly. For example, MemorySetting.MemoryPreference option optimizes memory use for the data in cells to decrease the overall memory cost.

## Export Excel Data Excluding Hidden Rows in C#

Aspose.Cells allows [export visible rows data only from a worksheet][1]. Sometimes you need to export data in such a way that the data of only visible rows is to be exported (excluding hidden rows). Aspose.Cells provides a way to achieve this. You can use the ExportTableOptions.PlotVisibleRows option to specify that you want to export visible rows data only.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-ExportVisibleRowsData-1.cs" >}}

## Show Excel Formulas Instead of Values in C#

There is another valuable Microsoft Excel feature to show formulas instead of values in a worksheet. You can show formulas instead of the calculated values in Microsoft Excel by selecting the **Formulas** menu, then **Show Formulas**. Once this option is enabled, Microsoft Excel will display formulas inside the worksheet. You can achieve this using Aspose.Cells APIs. It provides a Worksheet.ShowFormulas property which you can set to true to set Microsoft Excel to display formulas.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-ShowFormulasInsteadOfValues-1.cs" >}}

## Fixes and Other Enhancements

In the new version, we also support to get/set the time of generating the PDF document. Moreover, we have enhanced the auto-fit row operation in the new release.

In this release, several important issues have been addressed. For example, issues around reading and writing Microsoft Excel file formats, protecting worksheets, Smart Markers, custom numbers formatting, [applying conditional formatting][2], [rendering and manipulating pivot tables][3], [rendering images from Excel worksheets][4], reading and writing HTML files, rendering and manipulating charts, [rendering images files from charts][5] and [exporting Excel workbooks to PDF format][6] have been resolved. A few improvements are also made to Aspose.Cells for .NET's formula calculation engine. We have fixed an exception that occurred when reading named ranges in Microsoft Excel files too. We also fixed a few bugs in the web-based Grid control provided by Aspose.Cells for .NET regarding copy/paste operations, applying borders to the cells and set formulas, etc.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 8.0.0, please visit the [download page][7].




[1]: https://docs.aspose.com/display/cellsnet/Export+visible+rows+data+from+worksheet
[2]: http://docs.aspose.com/display/cellsnet/Conditional+Formatting
[3]: https://docs.aspose.com/display/cellsnet/Home
[4]: http://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Image
[5]: https://docs.aspose.com/display/cellsnet/Chart+Rendering#ChartRendering-RenderingChartstoImages
[6]: http://docs.aspose.com/display/cellsnet/Converting+Excel+to+PDF+Files
[7]: http://downloads.aspose.com/cells/net




