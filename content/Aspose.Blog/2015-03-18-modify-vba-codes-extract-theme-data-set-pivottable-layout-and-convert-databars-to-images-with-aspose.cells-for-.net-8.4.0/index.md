---
title: 'Modify VBA Codes in Excel and Set PivotTable Layout in C# using Aspose.Cells for .NET'
date: Wed, 18 Mar 2015 10:05:45 +0000
draft: false
url: /2015/03/18/modify-vba-codes-extract-theme-data-set-pivottable-layout-and-convert-databars-to-images-with-aspose.cells-for-.net-8.4.0/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


Aspose.Cells for .NET 8.4.0 has been released. This release contains many useful features and other enhancements including the long-awaited feature to manipulate VBA codes embedded inside the spreadsheets. If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you check the complete [Public API Changes][1] section to know what has been changed in the API so far.

## Modify VBA Macro Code in Excel using C#

Many of the Aspose.Cells users had been waiting for this feature, and now it is available with the release of Aspose.Cells for .NET 8.4.0. The latest version has exposed a new namespace named Aspose.Cells.Vba and a few classes to provide the means to access the VBA code embedded inside the macro-enabled spreadsheets, and to update the code as per your requirements. The details of the newly exposed classes are as follows.

*   VbaProject class can be used to fetch the VBA project from a given spreadsheet.
*   VbaModuleCollection class represents the collection of VBA modules that are part of a given VbaProject.
*   VbaModule class represents a single module from the VbaModuleCollection.

The following C# code snippet shows how to dynamically modify the VBA code segments in Excel.

{{< gist aspose-cells c326c6c668fc372e30569fa9e0f6bf4b "Examples-CSharp-Articles-ManagingVBAModules-ModifyingVBAOrMacroCode-ModifyingVBAOrMacroCode.cs" >}}

See the document on how to [Modify VBA or Macro Code via Aspose.Cells][2] for your reference.

## Extract Theme Data from Excel in C#

Aspose.Cells allows users to extract theme-related data from an Excel file. For example, you can extract Theme Name applied to the workbook, Theme Color applied to cell or borders of the cell, etc. Please see the document on [how to extract theme data][3] for your reference.

## Remove Pivot Table from Worksheet in C#

Another worth mentioning feature is the support for [Pivot Table removal][4]. Aspose.Cells has provided this feature by exposing two new methods for the PivotTableCollection class that allows deleting a specific PivotTable from the collection depending upon the input parameter.

Here are a few details about the newly exposed methods whereas the code snippets are available in the detailed article as linked above.

*   PivotTableCollection.Remove method accepts an object of PivotTable, and removes it from the collection.
*   PivotTableCollection.RemoveAt method accepts a zero index based integer value and removes the particular PivotTable from the collection.

## Support for Different Pivot Table Layouts

Microsoft Excel has predefined layouts for the Pivot Tables as listed below. Upon choosing any of these layouts, Microsoft Excel applies formatting to the Pivot Tables accordingly.

*   Compact Form
*   Outline Form
*   Tabular Form

Aspose.Cells for .NET 8.4.0 provides the same functionality while using the newly exposed methods for the PivotTable class that allows to dynamically set the layouts as discussed above. Detailed article and sample code snippets are available at [Changing the Layout of Pivot Table][5].

## Convert DataBars to Images

With the release of v8.4.0, the Aspose.Cells API has provided the DataBar.ToImage method to [save the conditionally formatted DataBar in image format][6]. The DataBar.ToImage method accepts two parameters as detailed below.

*   The first parameter is of type Cell on which conditional formatting has been applied.
*   The second parameter is of type ImageOrPrintOptions in order to set different parameters of the resultant image.

The following sample code demonstrates the use of DataBar.ToImage method to render the DataBar in image format.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-ManageConditionalFormatting-GenerateDatabarImage-GenerateDatabarImage.cs" >}}

## Custom Properties for the Document Information Panel

Aspose.Cells can be used to [add custom properties][7] inside the workbook object which are visible in the Document Information Panel when accessed through Microsoft Excel using the File > Info > Properties > Show Document Panel menu.

The following code snippet uses the ContentTypePropertyCollection.Add method to add two custom properties.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-AddingCustomPropertiesVisible-1.cs" >}}

## Other Enhancements and Fixes

In the new version, we have also provided the following new enhancements:

*   Customize the generated CSS file while saving Excel to HTML file format
*   Retain the Cell's Number Format after using ImportTwoDimensionArray
*   Aspose.PDF and other tools validates the output PDF/A-1B file by Aspose.Cells API
*   Workbook's RefreshChartCache works with regional and language settings

We have fixed a few exceptions that occurred while reading and writing Microsoft Excel and HTML file formats. We have also fixed the exceptions that occurred while manipulating Pivot tables in the template file and combining workbooks.

In this release, several important issues have been addressed. For example, issues around reading/ writing Microsoft Excel file formats, combining worksheets, Smart Markers, manipulating PivotTables, applying formattings to the cells, using PageSetup options, rendering HTML file format, applying conditional formatting, manipulating shapes, [rendering images from Excel worksheets][8], manipulating charts with formatting, [rendering images files from charts][9] and [exporting Excel workbooks to PDF format][10] have been resolved. We have also enhanced the Aspose.Cells formula calculation engine further and fixed a few relevant issues in this release.

We have fixed an issue regarding the [customize row/column headers][11] in the web-based Grid control provided by Aspose.Cells for .NET. We also figured out issues around setting the background color, alignment of rows and charts in the template file not being refreshed in the web-based Grid control by Aspose.Cells for .NET.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 8.4.0, please visit the [download page][12].




[1]: https://docs.aspose.com/display/cellsnet/Migrating+from+Earlier+Versions+of+Aspose.Cells
[2]: http://docs.aspose.com/display/cellsnet/Modifying+VBA+or+Macro+Code+using+Aspose.Cells
[3]: http://docs.aspose.com/display/cellsnet/Extract+Theme+Data+from+Excel+File
[4]: http://docs.aspose.com/display/cellsnet/Delete+Pivot+Table+from+a+Worksheet
[5]: http://docs.aspose.com/display/cellsnet/Changing+the+Layout+of+Pivot+Table
[6]: http://docs.aspose.com/display/cellsnet/Generate+Conditional+Formatting+DataBars+Images
[7]: https://docs.aspose.com/display/cellsnet/Adding+Custom+Properties+visible+inside+Document+Information+Panel
[8]: http://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Image
[9]: https://docs.aspose.com/display/cellsnet/Convert+an+Excel+Chart+to+Image
[10]: https://docs.aspose.com/display/cellsnet/Convert+Excel+Workbook+to+PDF
[11]: https://docs.aspose.com/display/cellsnet/Customize+Row+and+Column+Headers
[12]: http://downloads.aspose.com/cells/net




