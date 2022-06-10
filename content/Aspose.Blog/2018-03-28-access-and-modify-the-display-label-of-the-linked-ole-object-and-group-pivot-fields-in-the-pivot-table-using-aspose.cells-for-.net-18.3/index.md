---
title: 'Access and Modify Display Label of Linked Ole Object in Excel using C#'
date: Wed, 28 Mar 2018 14:29:01 +0000
draft: false
url: /2018/03/28/access-and-modify-the-display-label-of-the-linked-ole-object-and-group-pivot-fields-in-the-pivot-table-using-aspose.cells-for-.net-18.3/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce the release of [Aspose.Cells for .NET v18.3][1]. Please check the [document][2] on how to install Aspose for .NET APIs directly from NuGet repository. In this release, we have added some worthy features and other enhancements for the users. Please check the [release notes][3] in order to get an idea about what is new and what has been enhanced or fixed with this revision of Aspose.Cells for .NET.

## Access and Modify the Display Label of the Linked Ole Object

Microsoft Excel allows you to change the display label of the Ole Object. You can also access or modify the display label of the Ole object via Aspose.Cells APIs using the **OleObject.Label** property. The following sample code loads an Excel file that contains the Ole Object. The code accesses the Ole Object and changes its Label. Please notice the console output that will show the effect of the sample code.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "DrawingObjects-AccessAndModifyLabelOfOleObject.cs" >}}

Please see the document/article with attachment(s) on how to access and modify the display label of the linked Ole Object for your reference.

*   [Access and Modify the Display Label of the Linked Ole Object][4]

## Group Pivot Fields in the Pivot Table

Microsoft Excel allows you to group pivot fields in the Pivot Table. When there is a large amount of data related to a pivot field, it is better to group them into sections. Aspose.Cells provides this feature via the **PivotTable.SetManualGroupField()** method. This was a long-awaited feature requested by many users. The following sample code loads the template Excel file and performs grouping operation on the first pivot field in the Pivot Table using the **PivotTable.SetManualGroupField()** method.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "PivotTables-GroupPivotFieldsInPivotTable.cs" >}}

Please see the document/article with attachment(s) on how to group pivot fields in the Pivot Table for your reference.

*   [Group Pivot Fields in the Pivot Table][5]

## Export Similar Border Style when Border Style is not Supported by Web Browsers

Microsoft Excel also supports dashed border types that are not supported by most web browsers. When you convert such an Excel file into HTML using Aspose.Cells, the borders are removed. However, Aspose.Cells allows you to accomplish the task and supports to display such borders with **HtmlSaveOptions.ExportSimilarBorderStyle** property. For more detail on the feature, please see this article/document for your reference.

*   [Export similar Border Style when Border Style is not supported by Web Browsers][6]

## Find if the Worksheet is a Dialog Sheet

Dialog sheet is an older format that contains a dialog box. You can find if a sheet is a dialog or some other type with **Worksheet.Type** property. If it returns enumeration value SheetType.Dialog, then it means, you are dealing with Dialog sheet. For more detail, please see this article.

*   [Find if the Worksheet is Dialog Sheet][7]

## Preserve Single Quote Prefix of Cell Value or Range

When you put some value inside a cell that has leading apostrophe or single quote mark, then Microsoft Excel hides it, but when you select the cell, it displays the leading apostrophe or single quote in a formula bar. Aspose.Cells provides **StyleFlag.QuotePrefix** property that will handle either preserving the quote or not preserving the quote for your needs. For more detail, please see this article.

*   [Preserve Single Quote Prefix of Cell Value or Range][8]

## Change the Decimal Separator from Numeric Keypad

By default, Aspose.Cells.GridWeb (similar to MS Excel) displays numeric data accordingly based on the locale/regional settings on the machine. You can change the decimal separator from Numeric keypad programmatically using Aspose.Cells.GridWeb API. So, when a file is imported into GridWeb matrix or you input some numeric data (from the numeric keypad) into a new worksheet cell, it should have your desired decimal separator set visually. For more detail, please see this article.

*   [Change the decimal separator from Numeric keypad][9]

## Other Enhancements and Fixes

There are a few other enhancements included and some exceptions handled in the new release for the users. A few of the worth mentioning features and other improvements are as follows.

*   [Read axis labels after calculating the chart][10].
*   [Specify document Version number of the Excel File using built-in Document Properties][11].
*   [Add custom server-side function validation][12].
*   Handled System.IndexOutOfRangeException, System.FormatException and StackOverflowException when loading on XLSX/XLSB files.

## Changes to the Public API

This version of Aspose.Cells for .NET has made some changes to the Public API. A few of the worth mentioning changes are as follow:

*   Added **HtmlSaveOptions.ExportSimilarBorderStyle** property, it indicates whether exporting the similar border style when the border style is not supported by browsers.
*   Added new enum **GridValidationType.CustomServerFunction** type, it represents custom server-side function validation.
*   Added **ChartType.Map** enum member, it represents the map chart.
*   Added **OleObject.Label** property, it gets and sets the display label of the linked Ole Object.
*   Added **StyleFlag.QuotePrefix** enum member, it indicates whether applying the style's QuotePrefix property.
*   Added **DialogBox** class, it represents the dialog box sheet.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][13].
*   [Install Aspose for .NET APIs from NuGet repository][14]
*   [Aspose.Cells for .NET Documentation][15] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][16] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][17] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][18] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Cells/18.3.0
[2]: https://docs.aspose.com/display/cellsnet/Installation#Installation-InstallAspose.Cellsfor.NETthroughNuGet
[3]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+18.3+Release+Notes
[4]: https://docs.aspose.com/display/cellsnet/Access+and+Modify+the+Display+Label+of+the+Linked+Ole+Object
[5]: https://docs.aspose.com/display/cellsnet/Group+Pivot+Fields+in+the+Pivot+Table
[6]: https://docs.aspose.com/display/cellsnet/Export+similar+Border+Style+when+Border+Style+is+not+supported+by+Web+Browsers
[7]: https://docs.aspose.com/display/cellsnet/Find+if+the+Worksheet+is+Dialog+Sheet
[8]: https://docs.aspose.com/display/cellsnet/Preserve+Single+Quote+Prefix+of+Cell+Value+or+Range
[9]: https://docs.aspose.com/display/cellsnet/Change+the+decimal+separator+from+Numeric+keypad
[10]: https://docs.aspose.com/display/cellsnet/Read+Axis+Labels+after+Calculating+the+Chart
[11]: https://docs.aspose.com/display/cellsnet/Specify+Document+Version+of+the+Excel+File+using+BuiltIn+Document+Properties
[12]: https://docs.aspose.com/display/cellsnet/Add+Custom+Server-side+Function+Validation
[13]: https://products.aspose.com/cells/net
[14]: https://www.nuget.org/packages/Aspose.Cells
[15]: https://docs.aspose.com/display/cellsnet/home
[16]: https://apireference.aspose.com/
[17]: https://forum.aspose.com/c/cells
[18]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




