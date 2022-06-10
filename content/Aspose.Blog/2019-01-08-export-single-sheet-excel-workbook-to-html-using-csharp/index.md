---
title: 'Export Single Sheet Excel Workbook to HTML using C#'
date: Tue, 08 Jan 2019 14:46:49 +0000
draft: false
url: /2019/01/08/export-single-sheet-excel-workbook-to-html-using-csharp/
author: Amjad Sahi
summary: ''
tags: ['Export Single Sheet Excel Workbook to HTML', 'Export print area in Excel worksheets to HTML']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce the release of [Aspose.Cells for .NET v18.12][1], the MS Excel file formats API that provides the ability to create, manipulate, convert, or render MS Excel spreadsheets, and more importantly - is fully documented. Please check the [document][2] on how to install Aspose for .NET APIs directly from the NuGet repository. We have added a few important features and other enhancements while keeping the product more stable and feature-rich API. We also included important bug fixes as a part of this release. Please check the [release notes][3] which cover all the new features, enhancements, and list of bugs that are resolved in this new version.

## Export Single Sheet Workbook to HTML

The workbook can have multiple sheets that are rendered as multiple tab pages when converted to HTML using MS Excel. Similarly, if a workbook contains a single sheet, it shows one tab page when converted to HTML using Excel. This conversion was working fine for multiple sheets while using Aspose.Cells. However, for a single sheet workbook, there was no tab page and only HTML file was created without creating a separate folder containing CSS. Now Aspose.Cells has enhanced its library to create similar output for single sheet workbooks as compared to output created by Excel.

For a working example refer to the following article:

*   Export single sheet workbook to HTML

## Load Workbook without Loading VBA Project using C#

In complex Excel files (XLSM/XSLB) there can be a large number of macros which can be very long. Many times there is a need to load the workbooks without loading these VBA projects like just extracting the sheet names from the loaded workbook. In this case, we need a filter that can load/skip VBA projects. This time Aspose.Cells has introduced a filter option **LoadDataFilterOptions.VBA** which can be used for this purpose.

For a working example refer to the following article:

*   [Filter VBA Project while loading a workbook][4]

## Replacing Tags in Textbox within a Worksheet using C#

The textbox is a common control that can be used in a worksheet. This is not necessary that the text in the textbox is fixed. It may have tags that can be replaced with some text at runtime. It helps users to configure the controls as per the data on the sheet or from some other source. Worksheet.replace can be used for this purpose and textbox can be set with the desired text.

For a working example refer to the following article:

*   [Replace tag with text in a textbox inside the worksheet][5]

## Export Print Area Range to HTML

We can convert worksheets to HTML but rendering the entire sheet at once may not be required always. You may require just a selected area of the sheet to be rendered to HTML. Worksheets contain page setup where the print area can be set. There was a need that only this print area shall be rendered to HTML if required. **HtmlSaveOptions** is extended by adding a new enumerator **ExportPrintAreaOnly** which enables users to render only print area in the HTML.

For a working example refer to the following article:

*   Replace tag with text in a textbox inside the worksheet

## Identification of Validation as Dropdown

A worksheet can have different types of validations including dropdown. Users might want to detect the type of validation and take some decisions based on this information. Validation object can be obtained from a cell and a new function is defined for this validation which returns if validation is a dropdown or not. Use the function **Validation.getInCellDropDown()** which returns a Boolean value i.e. true or false.

For a working example refer to the following article:

*   [Check if validation in cell is dropdown][6]

## Other Enhancements and Fixes

There are some other enhancements included and a few exceptions handled in the new release for the users. A few of the worth mentioning features and other improvements are as follows:

*   [Creating and customizing charts][7]
*   Tracked Changes lost during conversion from XLSB to XLSM and XLS to XLSM
*   Text moved a little bit after ungrouping the shape when saving an XLS to XLSX
*   Optimization for memory performance: release original stream after loading Workbook
*   Handled exception "NullReferenceException" when loading an XLSB file format
*   Handled ArgumentException on loading a workbook

In Aspose.Cells 18.12, we fixed several important bugs and other issues. For example, issues around reading/writing MS Excel file formats, reading/writing HTML files, protecting ODS files, setting data validations, manipulating rows and columns, manipulating smart art shapes, refreshing and calculating pivot tables, rendering and manipulating charts and shapes, [rendering images from Excel worksheets][8], [rendering images files from charts][9] and [exporting Excel workbooks to PDF format][10] have been resolved in the release. 

## Changes to the Public API

The following is a list of any changes made to the public API such as added, renamed, removed or deprecated members as well as any non-backward compatible change made to Aspose.Cells for .NET:

*   Adds **HtmlSaveOptions.ExportSingleTab property,** indicates whether exporting the single tab when the file only has one worksheet in it. The default value is false.
*   Adds **HtmlSaveOptions.ExportPrintAreaOnly property, **indicates if only exporting the print area to html file. The default value is false.
*   Deletes **obsoleted Workbook.Initialize() method,** use Workbook constructor instead.
*   Deletes **obsoleted Workbook.Styles property, **use Workbook.CreateStyle() to create and manipulate style for workbook instead of StyleCollection.Add(); Use Workbook.GetNamedStyle(string) to get named style instead of StyleCollection.
*   Deletes **obsoleted Workbook.CheckWriteProtectedPassword() method, **use WorkbookSettings.WriteProtection.ValidatePassword method instead.
*   Deletes **obsoleted Workbook.CheckWriteProtectedPassword() method, **use WorkbookSettings.WriteProtection.ValidatePassword method instead.
*   Adds **LoadDataFilterOptions.VBA enum, **the option used to ignore VBA projects while loading template file.
*   Adds **Style.InvariantCustom property, **gets the culture-independent pattern string for number format (including the pattern string for built-in number).
*   Adds **FindOptions.ValueTypeSensitive property, **indicates whether searched cell value type should be same with the searched key.
*   Obsoletes **FindOptions.SearchNext property, **use FindOptions.SearchBackward property instead, true value for this new property corresponds to false of SearchNext.
*   Deletes **obsoleted Cells.ImportGridView(System.Web.UI.WebControls.GridView,int ,int , bool ,bool ,bool ) method, **use Cells.ImportGridView (System.Web.UI.WebControls.GridView gridView,int firstRow,int firstColumn,ImportTableOptions options) method. instead.
*   Deletes **obsoleted Cells.Start property, **use Cells.FirstCell property instead.
*   Deletes **obsoleted Cells.End property, **use Cells.LastCell property instead.
*   Deletes **Cells\[int\] property, **use Cells.GetEnumerator() method to iterate all cells in this worksheet instead.
*   Deletes **obsoleted Cells.ImportDataColumn() methods, **use Cells.ImportData (DataTable,int,int,ImportTableOptions) method instead.
*   Deletes **obsoleted Cells.ImportDataReader() methods, **use Cells.ImportData (IDataReader, int, int,ImportTableOptions) method instead.
*   Deletes **obsoleted Shape.Rotation property,** use Shape.RotationAngle property instead.
*   Deletes **obsoleted Validation.AreaList property, **use Validation.Areas property instead.
*   Deletes **obsoleted Style constructor, **use CellsFactory.CreateStyle() or Workbook.CreateStyle() method instead.
*   Deletes **obsoleted Shape.IsPrinted property, **use Shape.IsPrintable property instead.
*   Deletes **obsoleted PivotItem.Move(int) method, **using PivotItem.Move(int , bool ) method instead.
*   Deletes **obsoleted  Cells.ExportDataTable(int, int, int, int,bool, bool),Cells.ExportDataTable(int, int, int, int,object\[\]), Cells.ExportDataTable(int, int, int, int,bool), **  
    **Cells.ExportDataTable(DataTable, int, int\[\],int, bool) and Cells.ExportDataTable(DataTable,int, int, int, bool, bool) methods, **use ExportDataTable(firstRow,firstColumn, totalRows, totalColumns,ExportTableOptions) method instead.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][11].
*   [Install Aspose for .NET APIs from NuGet repository][12]
*   [Aspose.Cells for .NET Documentation][13] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][14] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][15] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][16] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Cells/18.12.0
[2]: https://docs.aspose.com/display/cellsnet/Installation#Installation-InstallAspose.Cellsfor.NETthroughNuGet
[3]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+18.12+Release+Notes
[4]: https://docs.aspose.com/display/cellsnet/Filter+VBA+Project+while+loading+a+workbook
[5]: https://docs.aspose.com/display/cellsnet/Replace+tag+with+text+in+a+textbox+inside+the+Worksheet
[6]: https://docs.aspose.com/display/cellsnet/Data+Validation#DataValidation-Checkifvalidationincellisdropdown
[7]: https://docs.aspose.com/
[8]: https://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Different+Image+Formats
[9]: https://docs.aspose.com/display/cellsnet/Chart+Rendering
[10]: https://docs.aspose.com/display/cellsnet/Convert+Excel+Workbook+to+PDF
[11]: https://products.aspose.com/cells/net
[12]: https://www.nuget.org/packages/Aspose.Cells
[13]: https://docs.aspose.com/display/cellsnet/home
[14]: https://apireference.aspose.com/
[15]: https://forum.aspose.com/c/cells
[16]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




