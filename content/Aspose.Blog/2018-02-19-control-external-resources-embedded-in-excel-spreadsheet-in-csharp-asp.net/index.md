---
title: 'Control External Resources Embedded in Excel Spreadsheets using C# .NET'
date: Mon, 19 Feb 2018 14:22:11 +0000
draft: false
url: /2018/02/19/control-external-resources-embedded-in-excel-spreadsheet-in-csharp-asp.net/
author: Amjad Sahi
summary: ''
tags: ['Control External Resources in Excel in Csharp']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce the release of [Aspose.Cells for .NET v18.2][1]. Please check the [document][2] on how to install Aspose for .NET APIs directly from NuGet repository. In this release, we have added a few valuable features for the users. For example, we included support to control/manage external resources embedded in the Excel document. You can filter formulas and defined names separately when loading Excel spreadsheets. Some other enhancements are also added regarding shapes. Please check the [release notes][3] in order to get an idea about what is new and what has been enhanced or fixed with this revision of Aspose.Cells for .NET.

## Control External Resources in Spreadsheet in C#

If your Excel file contains external resources e.g. linked images etc. and you need to control these external resources, Aspose.Cells supports to manage external resources using **Workbook.Settings.StreamProvider** which takes the implementation of **IStreamProvider** interface. Whenever you will try to render your worksheet containing external resources, the methods of IStreamProvider interface will be invoked which will enable you to take appropriate actions for your external resources. The following snippet loads an Excel file (containing a linked image). The code replaces the linked image with Aspose Logo and renders the entire sheet into a single image using SheetRender class.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "WorkbookSettings-ControlExternalResourcesUsingWorkbookSetting_StreamProvider.cs" >}}

Please see the document/article with attachment(s) on how to control external resources embedded in an Excel worksheet for your reference.

*   [Control External Resources using WorkbookSetting.StreamProvider][4]

## Filter Defined Names while loading Workbook

Aspose.Cells now allows you to filter/exclude defined names present inside the workbook while loading the spreadsheet. You may use **LoadDataFilterOptions.DefinedNames** to load defined names and use **~LoadDataFilterOptions.DefinedNames** to remove them while loading the workbook. For more detail on the feature, please see this article/document for your reference.

*   [Filter Defined Names while loading Workbook][5]

## Set Margins of Comment or Shape inside the Worksheet

Using Aspose.Cells APIs, you can set the margins of any shape including comments using the **Shape.TextBody.TextAlignment** property. This property returns the object of **Aspose.Cells.Drawing.Texts.ShapeTextAlignment** class which has different properties e.g. **TopMarginPt**, **LeftMarginPt**, **BottomMarginPt**, **RightMarginPt** etc. that can be used to set the top, left, bottom and right margins. For more detail, please see this article.

*   [Set Margins of Comment or Shape inside the Worksheet][6]

## Specify Formula Fields while Importing Data to Worksheet

You can specify formula fields when you import data into your worksheet using the **ImportTableOptions.IsFormulas**. This property takes the Boolean array where the value true means the field is a formula field. For example, if the third field is a formula field, then third value in the array will be true. For more detail, please see this article.

*   [Specify Formula Fields while Importing Data to Worksheet][7]

## Specify Maximum Rows of Shared Formula

Aspose.Cells provides the **Workbook.Settings.MaxRowsOfSharedFormula** property that can be used to specify the maximum rows of the shared formula. The shared formula will be split into several shared formulas if the total rows of the shared formula are greater than it. For more detail, please see this article.

*   [Specify Maximum Rows of Shared Formula][8]

## Other Enhancements and Fixes

There are some other enhancements included and a few exceptions handled in the new release for the users. A few of the worth mentioning features and other enhancements are as follows.

*   Implemented Aspose.Cells for .NET Standard and Aspose.Cells for .NET Core.
*   And enhancement is made:`=cmd|' /c calc'!A0`is not present inside Worksheets.ExternalLinks.
*   Mimic behavior of MS Excel when entering text (while wrapping text is enabled) into Aspose.Cells.GridWeb.
*   Handled an exception "Input string was not in a correct format" when importing the Excel file into Aspose.Cells.GridWeb.

In Aspose.Cells 18.2, we fixed several important bugs and other issues. For example, issues around reading/writing MS Excel file formats, rendering Excel to HTML and vice versa, manipulating shapes, Smart Markers, using PageSetup options, rendering and manipulating charts, manipulating PivotTables, [rendering images from Excel worksheets][9], [rendering images files from charts][10] and [exporting Excel workbooks to PDF format][11] have been resolved. Moreover, the Aspose.Cells formula calculation engine is further optimized.

## Changes to the Public API

This version of Aspose.Cells for .NET has made some changes to the Public API. A few of the worth mentioning changes are as follow:

*   Added **LoadDataFilterOptions.DefinedNames** enum member, it indicates whether loading defined Name objects when loading template file.
*   Added **SheetType.Dialog** enum member, it represents dialog sheet.
*   Added **WorkbookSettings.MaxRowsOfSharedFormula** property, it gets and sets the max row number of shared formula. The shared formula will be split to several shared formula if the total rows of shared formula is greater than it.
*   Added **ImportTableOptions.IsFormulas** property, it represents which column in the datatable should be imported as formulas.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][12].
*   [Install Aspose for .NET APIs from NuGet repository][13]
*   [Aspose.Cells for .NET Documentation][14] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][15] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][16] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][17] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Cells/18.2.0
[2]: https://docs.aspose.com/display/cellsnet/Installation#Installation-InstallAspose.Cellsfor.NETthroughNuGet
[3]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+18.2+Release+Notes
[4]: https://docs.aspose.com/display/cellsnet/Control+External+Resources+using+WorkbookSetting.StreamProvider
[5]: https://docs.aspose.com/display/cellsnet/Filter+Defined+Names+while+loading+Workbook
[6]: https://docs.aspose.com/display/cellsnet/Set+Margins+of+Comment+or+Shape+inside+the+Worksheet
[7]: https://docs.aspose.com/display/cellsnet/Specify+Formula+Fields+while+Importing+Data+to+Worksheet
[8]: https://docs.aspose.com/display/cellsnet/Specify+Maximum+Rows+of+Shared+Formula
[9]: https://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Different+Formats
[10]: https://docs.aspose.com/display/cellsnet/Chart+Rendering
[11]: https://docs.aspose.com/display/cellsnet/Convert+Excel+Workbook+to+PDF
[12]: https://products.aspose.com/cells/net
[13]: https://www.nuget.org/packages/Aspose.Cells/18.2.0
[14]: https://docs.aspose.com/display/cellsnet/home
[15]: https://apireference.aspose.com/
[16]: https://forum.aspose.com/c/cells
[17]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




