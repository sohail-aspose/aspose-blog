---
title: 'Apply Values Format Code to Chart Series and Interrupt Formula Calculations in the Workbook using Aspose.Cells for .NET 17.10'
date: Wed, 01 Nov 2017 12:00:46 +0000
draft: false
url: /2017/11/01/apply-values-format-code-to-chart-series-and-interrupt-formula-calculations-in-the-workbook-using-aspose.cells-for-.net-17.10/
author: Amjad Sahi
summary: ''
tags: ['Cancel the formula calculation of in Excel', 'Interrupt formula calculation of in Excel']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce the release of [Aspose.Cells for .NET v17.10][1]. This release includes some useful features along with critical bug fixes that further improve the overall stability of the APIs. Please check the [release notes][2] in order to get an idea about what is new and what has been enhanced or fixed with this revision of Aspose.Cells for .NET. You can also install [Aspose for .NET APIs directly from NuGet repository][3].

## Set the Values Format Code of Chart Series

Aspose.Cells supports to set the values format code of chart series using the **Series.ValuesFormatCode** property. This property is useful for the series which are based on the range inside the worksheet, it also works well for the series created with array of values. The following sample code formats values with the formatting "$#,##0" using the **Series.ValuesFormatCode** property so the number, e.g "10000" will become "$10,000".

{{< gist aspose-cells c326c6c668fc372e30569fa9e0f6bf4b "Examples-CSharp-Charts-SetValuesFormatCodeOfChartSeries.cs" >}}

Please see the document/article with attachments and screenshots on how to set values format code of the chart series for your complete reference.

*   [Set the Values Format Code of Chart Series][4]

## Utilize Sheet.SheetId Property of OpenXml using Aspose.Cells

The property _Sheet.SheetId_ is found inside the DocumentFormat.OpenXml.Spreadsheet namespace and is a part of OpenXml. Aspose.Cells provides the equivalent property named **Worksheet.TabId**. For more detail, please see this article.

*   [Utilize Sheet.SheetId property of OpenXml using Aspose.Cells][5]

## Read and Write External Connection of XLSB file

Aspose.Cells already supports reading and writing external connections of an XLSX file format. We have added similar support for XLSB file format now. The code is same for both formats (XLSX and XLSB). For more detail, please see this article.

*   [Read and Write External Connection of XLSB file][6]

## Interrupt or Cancel the Formula Calculation of Workbook

Aspose.Cells provides a mechanism to interrupt or cancel the formula calculation of workbook using the **AbstractCalculationMonitor.Interrupt()** method. This is useful when formula calculations in the workbook is taking too much time and you want to cancel its processing at certain point. For more detail, please see this article.

*   [Interrupt or Cancel the Formula Calculation of Workbook][7]

## Specify How to Cross String in Output HTML using HtmlCrossType

When a cell contains text or string but it is larger than the width of the cell, then the string overflows if the next cell in next column is null or empty. When you save your Excel file into HTML, you can control this overflow for your needs by specifying the cross type using the **HtmlCrossType** enumeration. For more detail, please see this article.

*   [Specify how to cross string in output HTML using HtmlCrossType][8]

## Other Enhancements and Fixes

There are some other enhancements included in the new release for the users. A few of the worth mentioning features/enhancements are as follow.

*   Sheet to Image rendering - Text alignment for Asian fonts improved.
*   Handled/resolved "Input string was not in a correct format" - Exception on Pivot.CalculateData() method.
*   Handled an exception when converting XLSM file back to XLS file format.

In Aspose.Cells 17.10 we fixed many critical bugs and other issues. For example, issues around reading/writing MS Excel file formats, data sorting, rendering shapes and drawing objects, rendering and manipulating charts, inserting/deleting rows/columns, [rendering images from Excel worksheets][9], [rendering images files from charts][10] and [exporting Excel workbooks to PDF format][11] have been resolved. The Aspose.Cells formula calculation engine is improved too.

## Changes to the Public API

This version of Aspose.Cells for .NET has made some changes to the Public API. A few of the worth mentioning changes are as follow:

*   Added **_AbstractCalculationMonitor.Interrupt(string)_** method, it allows users to interrupt the progress of formula calculations.
*   Added **_HtmlCrossType.MSExport_** enum, it displays the string like MS Excel exporting HTML.
*   Added **Worksheet.TabId** property, it sets/gets the internal identifier for the sheet.
*   Added **Seris.ValuesFormatCode** property, it represents number format code of series values.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][12].
*   [Aspose.Cells for .NET Download Section][13].
*   [Aspose.Cells for .NET Documentation][14] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][15] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][16] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][17] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/net/new-releases/aspose.cells-for-.net-17.10/
[2]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+17.10+Release+Notes
[3]: https://www.nuget.org/packages/Aspose.Cells/
[4]: https://docs.aspose.com/display/cellsnet/Set+the+Values+Format+Code+of+Chart+Series
[5]: https://docs.aspose.com/display/cellsnet/Utilize+Sheet.SheetId+property+of+OpenXml+using+Aspose.Cells
[6]: https://docs.aspose.com/display/cellsnet/Home
[7]: https://docs.aspose.com/display/cellsnet/Interrupt+or+Cancel+the+Formula+Calculation+of+Workbook
[8]: https://docs.aspose.com/display/cellsnet/Specify+how+to+cross+string+in+output+HTML+using+HtmlCrossType
[9]: https://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Different+Formats
[10]: https://docs.aspose.com/display/cellsnet/Chart+Rendering
[11]: https://docs.aspose.com/display/cellsnet/Convert+Excel+Workbook+to+PDF
[12]: https://products.aspose.com/cells/net
[13]: https://downloads.aspose.com/cells/net
[14]: https://docs.aspose.com/display/cellsnet/home
[15]: https://apireference.aspose.com/
[16]: https://forum.aspose.com/c/cells
[17]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




