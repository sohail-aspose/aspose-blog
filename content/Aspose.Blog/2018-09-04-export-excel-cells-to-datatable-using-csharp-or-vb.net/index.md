---
title: 'Export Excel Cells to DataTable using C# or VB.NET'
date: Tue, 04 Sep 2018 09:47:52 +0000
draft: false
url: /2018/09/04/export-excel-cells-to-datatable-using-csharp-or-vb.net/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce the release of [Aspose.Cells for .NET v18.8][1]. Please check the [document][2] on how to install Aspose for .NET APIs directly from NuGet repository. Every release has new features to enrich the product for its stability and feature-rich flavor. In this release, we have added some useful features for the users. We made more efforts to address all the known issues and to fulfill requests for a rapid development of feature-rich market-oriented products. Moreover, we included important fixes and other enhancements in the release. Please check the [release notes][3] in order to get an idea about what is new and what has been enhanced or fixed with this revision of Aspose.Cells for .NET.

## Export Excel Cells to DataTable using C#

Data from a range of cells can be exported to DataTable where a flag is available now to skip/include header row or utilize other options in the exported data.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Data-Handling-ExportRangeWithFlagToSkipColumnHeader-1.cs" >}}

For a working example refer to the following article:

*   [Export Range with flag to skip column name][4] 

## Apply Text Alignment to Partial Text inside the TextBox

It is common to apply different alignments to the partial texts in the text box. This feature was having some issues but now it is reviewed and bugs are removed to incorporate proper alignment.   

For a working example refer to the following article:

*   [Applying text alignment to partial text inside the Textbox][5]  

## Content Copying for Accessibility

This option allows screen reader software to utilize the text within the PDF file for reading the PDF file.  You can disable it by applying a change permissions password and deselecting few options in Adobe Acrobat. Same functionality can be achieved using Aspose.Cells for .NET now. 

For a working example refer to the following article:

*   [Set content copy for accessibility option][6] 

## Disable Pivot Table Ribbon 

Pivot table based reports are useful but prone to error if target users do not have detailed knowledge of Excel to configure these reports. In these circumstances, organizations will want to restrict users from being able to change a pivot table based report. Common pivot table features like adding additional filters, slicers, fields, or changing the order of certain things in the report are mostly not recommended for every user. On the other hand, these users shall also be able to refresh the report and use existing filters or slicers. Aspose.Cells has provided this ability to developers for restricting users from changing these reports while creating these reports. For this purpose, Excel provides a feature to disable the pivot table ribbon and a similar thing is provided by Aspose.Cells i.e., the developer can disable the ribbon which contains controls to modify these reports.

For a working example along with a template file refer to the following article:

*   [Disable Pivot Table Ribbon][7]

## Pasting Rows/Columns with Paste Option 

While working with Excel, pasting rows and columns is very common and this feature was introduced in the earliest versions of Aspose.Cells. However limited paste options were available in contrast to MS Excel where variety of options are available when we paste data somewhere in MS Excel. Now Aspose.Cells has provided this feature and you can paste data with multiple options.   

For a working example refer to the following article:

*   [Pasting rows and columns with paste options][8] 

## Other Enhancements and Fixes

There are some other enhancements included and a few exceptions handled in the new release for the users. A few of the worth mentioning features and other improvements are as follows.

*   Encrypting/decrypting ODS files
*   Read/write connections of XLSB file
*   Support parsing formulas of revision logs to binary array
*   Retrieve Subtotaling settings
*   Ink Annotations become regular images after conversion
*   Handled exception when calculating formulas
*   Handled exceptions when reading/loading HTML/XLSX file formats

In Aspose.Cells 18.8, we fixed several important bugs and other issues. For example, issues around reading/writing MS Excel file formats, applying auto-fit rows/cols, applying validations, reading/writing HTML files, rendering and manipulating charts and shapes, manipulating PivotTables, [rendering images from Excel worksheets][9], [rendering images files from charts][10] and [exporting Excel workbooks to PDF format][11] have been resolved in the release. Moreover, the Aspose.Cells formula calculation engine is enhanced.

## Changes to the Public API

The following is a list of any changes made to the public API such as added, renamed, removed or deprecated members as well as any non-backward compatible change made to Aspose.Cells for .NET:

*   Adds **PdfSecurityOptions.AccessibilityExtractContent,** Permission to copy or extract content (in support of accessibility to disabled users or for other purposes)
*   Adds **SubtotalSetting class, **Represents the setting of subtotal.
*   Adds **Cells.RetrieveSubtotalSetting(CellArea)** method, Retrieves the setting of subtotal
*   Adds overload **Range.ExportDataTable (Aspose.Cells.ExportTableOptions)** method, Supports options of exporting range
*   Adds **WebQueryConnection.IsSameSetting** property and deletes **WebQueryConnection.IsFirstRow** property, Use WebQueryConnection.IsSameSetting property instead
*   Adds **WebQueryConnection.IsXmlSourceData** property and deletes **WebQueryConnection.IsSourceData** property, Use WebQueryConnection.IsXmlSourceData property instead
*   Adds **Shape.IsEquation** property, Indicates whether the shape contains equation
*   Adds overload **Cells.CopyColumns(Int32,Int32,PasteOptions)** and **Cells.CopyRows(Int32,Int32,PasteOptions)** method, Supports paste options when copying rows and columns
*   Adds **Axis.IsAutoTickLabelSpacing** property, Indicates whether tick label spacing is automatic

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][12].
*   [Install Aspose for .NET APIs from NuGet repository][13]
*   [Aspose.Cells for .NET Documentation][14] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][15] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][16] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][17] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Cells/18.8.0
[2]: https://docs.aspose.com/display/cellsnet/Installation#Installation-InstallAspose.Cellsfor.NETthroughNuGet
[3]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+18.8+Release+Notes
[4]: https://docs.aspose.com/display/cellsnet/Export+Data+from+Worksheet#ExportDatafromWorksheet-ExportRangewithflagtoskipcolumnname
[5]: https://docs.aspose.com/display/cellsnet/Applying+text+alignment+to+partial+text+inside+the+TextBox
[6]: https://docs.aspose.com/display/cellsnet/Convert+Excel+Workbook+to+PDF#ConvertExcelWorkbooktoPDF-SetContentCopyForAccessibilityoption
[7]: https://docs.aspose.com/display/cellsnet/Disable+Pivot+Table+Ribbons
[8]: https://docs.aspose.com/display/cellsnet/Copying+Rows+and+Columns#CopyingRowsandColumns-PastingRows/ColumnswithPasteOptions
[9]: https://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Different+Image+Formats
[10]: https://docs.aspose.com/display/cellsnet/Chart+Rendering
[11]: https://docs.aspose.com/display/cellsnet/Convert+Excel+Workbook+to+PDF
[12]: https://products.aspose.com/cells/net
[13]: https://www.nuget.org/packages/Aspose.Cells
[14]: https://docs.aspose.com/display/cellsnet/home
[15]: https://apireference.aspose.com/
[16]: https://forum.aspose.com/c/cells
[17]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




