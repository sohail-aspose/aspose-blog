---
title: 'Create PDF Bookmark for Chart Sheet in C# using Aspose.Cells for .NET 18.1'
date: Tue, 30 Jan 2018 10:59:43 +0000
draft: false
url: /2018/01/30/create-pdf-bookmark-for-chart-sheet-using-csharp-asp.net-excel-library/
author: Amjad Sahi
summary: ''
tags: ['Convert Excel to HTML', 'Create PDF bookmark for the chart sheets', 'export document properties in Excel to HTML']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce the release of [Aspose.Cells for .NET v18.1][1]. We have added some useful features and enhancements regarding Pivot Tables, Charts, and Excel to HTML renderings. Please check the [release notes][2] in order to get an idea about what is new and what has been enhanced or fixed with this revision of Aspose.Cells for .NET. You can also install [Aspose for .NET APIs directly from NuGet repository][3].

## Create PdfBookmarkEntry for Chart Sheet using C#

In previous versions, we can create **PdfBookmarkEntry** for normal sheets only. But now Aspose.Cells can also create **PdfBookmarkEntry** for chart sheet. Since the chart sheet does not have any other cell except cell A1, so it will create **PdfBookmarkEntry** for cell A1 only. The following sample code loads an Excel file that has four sheets in it. Two of them are normal sheets and others are chart sheets. It creates four bookmarks, one for each sheet.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Rendering-CreatePdfBookmarkEntryForChartSheet.cs" >}}

Please see the document/article with attachment(s) on how to create bookmarks for the chart sheet for your reference.

*   [Create PdfBookmarkEntry for chart sheet][4]

## Convert Excel to HTML - Exclude Unused Styles

Microsoft Excel file may contain many unnecessary unused styles. When you export the Excel file to an HTML file format, these unused styles are also exported. This could increase the size of HTML. You can exclude the unused styles during the conversion of Excel file to HTML using the **HtmlSaveOptions.ExcludeUnusedStyles** property.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "HTML-ExcludeUnusedStylesInExcelToHTML.cs" >}}

For more detail on the feature, please see this article/document for your reference.

*   [Exclude unused styles during Excel to HTML][5]

## Export Document, Workbook and Worksheet Properties in Excel to HTML

When Microsoft Excel file is exported to HTML using Microsoft Excel or Aspose.Cells APIs, it also exports various types of Document, Workbook, and Worksheet properties. You can avoid exporting these properties by setting the **HtmlSaveOptions.ExportDocumentProperties**, **HtmlSaveOptions.ExportWorkbookProperties** and **HtmlSaveOptions.ExportWorksheetProperties** as false. The default value of these properties is true. For more detail, please see this article.

*   [Export document, workbook and worksheet properties in Excel to HTML][6]

## Find and Refresh the Nested or Children Pivot Tables of Parent Pivot Table

A Pivot table may use other pivot tables as a data source. Such a Pivot table is called a child or nested Pivot table to its parent Pivot table. You can find the children Pivot tables for a parent Pivot table using the **PivotTable.GetChildren()** method. For more detail, please see this article.

*   [Find and refresh the nested or children Pivot Tables of parent pivot table][7]

## Parse Pivot Cached Records while Loading Excel file

When you create a Pivot Table, Microsoft Excel takes a copy of the source data and stores it in the Pivot Cache. The Pivot Cache is held inside the memory of Microsoft Excel. When you load your Excel file inside the Workbook object, you can decide whether you also want to load the records of Pivot Cache or not, using the **LoadOptions.ParsingPivotCachedRecords** property. The default value of this property is false. If Pivot Cache is quite big, it can increase the performance. For more detail, please see this article.

*   [Parsing pivot cached records while loading Excel file][8]

## Handle Events after Deleting Rows and Columns in GridDesktop

Aspose.Cells.GridDesktop has introduced two new events i.e. **AfterDeleteColumns** and **AfterDeleteRows**. These events are fired when you delete column(s) and row(s) respectively. For more detail, please see this article.

*   [Handle events after deleting columns and rows in GridDesktop][9]

## Other Enhancements and Fixes

There are some other enhancements included and a few exceptions handled in the new release for the users. A few of the worth mentioning features and other enhancements are as follows.

*   [Handle automatic units of chart axis like Microsoft Excel][10]
*   [Render interactive scrollbar in GridWeb][11]
*   Handled IndexOutOfRangeException while converting XLSX to HTML.
*   Handled System.OutOfMemoryException when rendering the image of the chart.
*   Handled an exception when setting HtmlString on a cell to a specific value.

In Aspose.Cells 18.1, we fixed several important bugs and other issues. For example, issues around reading/writing MS Excel file formats, manipulating Ole Objects in Excel file, rendering Excel to HTML and vice versa, converting SpreadsheetML to XLSX,  import custom objects to Excel sheet, rendering and manipulating charts, manipulating PivotTables, [rendering images from Excel worksheets][12], [rendering images files from charts][13] and [exporting Excel workbooks to PDF format][14] have been resolved. Moreover, the Aspose.Cells formula calculation engine is also optimized.

## Changes to the Public API

This version of Aspose.Cells for .NET has made some changes to the Public API. A few of the worth mentioning changes are as follow:

*   Added **LoadOptions.ParsingPivotCachedRecords** property, it indicates whether parsing pivot cached records when loading the file. The default value is false.
*   Added **HtmlSaveOptions.ExcludeUnusedStyles** property, it indicates whether excluding unused styles.The default value is false.
*   Added **HtmlSaveOptions.ExportDocumentProperties** property, it indicates whether exporting document properties.The default value is true.
*   Added **HtmlSaveOptions.ExportWorksheetProperties** property, it indicates whether exporting worksheet properties.The default value is true.
*   Added **PivotTable.GetChildren()** method, it gets the the children Pivot Tables which use this PivotTable data as data source.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][15].
*   [Aspose.Cells for .NET Download Section][16].
*   [Aspose.Cells for .NET Documentation][17] – up-to-date documentation containing Programmer's Guide, Knowledge Base, and much more.
*   [Aspose.Cells for .NET API Reference Guide][18] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][19] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][20] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/net/new-releases/-aspose.cells-for-.net-18.1/
[2]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+18.1+Release+Notes
[3]: https://www.nuget.org/packages/Aspose.Cells/
[4]: https://docs.aspose.com/display/cellsnet/Create+PdfBookmarkEntry+for+Chart+Sheet
[5]: https://docs.aspose.com/display/cellsnet/Exclude+Unused+Styles+during+Excel+to+HTML+conversion
[6]: https://docs.aspose.com/display/cellsnet/Export+Document+Workbook+and+Worksheet+Properties+in+Excel+to+HTML+conversion
[7]: https://docs.aspose.com/display/cellsnet/Find+and+Refresh+the+Nested+or+Children+Pivot+Tables+of+Parent+Pivot+Table
[8]: https://docs.aspose.com/display/cellsnet/Parsing+Pivot+Cached+Records+while+loading+Excel+file
[9]: https://docs.aspose.com/display/cellsnet/Handling+Events+after+Deleting+Columns+and+Rows+in+GridDesktop
[10]: https://docs.aspose.com/display/cellsnet/Handle+Automatic+Units+of+Chart+Axis+like+Microsoft+Excel
[11]: https://docs.aspose.com/display/cellsnet/Render+Interactive+Scrollbar+in+GridWeb
[12]: https://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Different+Formats
[13]: https://docs.aspose.com/display/cellsnet/Chart+Rendering
[14]: https://docs.aspose.com/display/cellsnet/Convert+Excel+Workbook+to+PDF
[15]: https://products.aspose.com/cells/net
[16]: https://downloads.aspose.com/cells/net
[17]: https://docs.aspose.com/display/cellsnet/home
[18]: https://apireference.aspose.com/
[19]: https://forum.aspose.com/c/cells
[20]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




