---
title: 'Detect Circular References in Excel in C# using Aspose.Cells for .NET'
date: Fri, 07 Dec 2018 11:25:58 +0000
draft: false
url: /2018/12/07/detect-circular-references-for-formulas-and-update-smart-art-text-using-aspose.cells-for-.net-v18.11/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce the release of [Aspose.Cells for .NET v18.11][1], the MS Excel file formats API that provides the ability to create, manipulate, convert or render MS Excel spreadsheets, and more importantly - is fully documented. We have added a few important features while keeping the product more stable and feature-rich API. Smart art is addressed in this release such that text can be updated in the shapes. This feature will enable users to modify these objects at runtime rather than fixed text in the shapes. Moreover, using the new version, circular references for formulas can be detected. The last section on this page contains more details and links about this product.

## Detect Circular References for Formulas in Excel

Using Aspose.Cells, circular references can be detected when the formula is calculated because the references of one formula commonly depend on the calculated results of other parts or other formulas. So we provide new APIs for this requirement (to gather cells with circular references) in the process of formula calculations. **AbstractCalculationMonitor.OnCircular(IEnumerator circularCellsData)** will be invoked by a formula calculation engine when encounter circular references, the element in the enumerator is CalculationCell objects which represent all cells in one circle. The returned value denotes whether the formula engine needs to calculate those cells in circular after this call.

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-Formulas-DetectCircularReference-1.cs" >}}

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-Formulas-DetectCircularReference-2.cs" >}}

For a working example along with a template file refer to the following article:

*   [Detect Circular Reference][2]

## Update Smart Art Text in C#

Smart art is used for better representation of information however earlier the text in the smart art shapes was fixed. This limitation is gone as now smart art text can be updated. For this purpose Shape.Text can be used which sets new text in the smart art shape.

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-Articles-ReplaceTextInSmartArt-1.cs" >}}

For a working example refer to the following article:

*   [Replace smart art text][3]

## Convert Worksheets to SVG in C#

SVG stands for Scalable Vector Graphics. SVG is a specification based on XML standards for two-dimensional vector graphics. It is an open standard that has been under development by the World Wide Web Consortium (W3C) since 1999. Aspose.Cells for .NET supports to convert worksheets to SVG image since version 7.1.0. The conversion is enhanced in a way that now it renders the workbook to SVG with an active sheet in tact.

For a working example, refer to the following article:

*   [Convert Worksheet to SVG][4]

## Get Pivot Table Refresh Date

Pivot tables are very common reports which are present in the workbooks. These reports are updated from time to time and it is important to know the last time when the report was updated for better decision making. Aspose.Cells has provided this feature by introducing property RefreshDate. Similarly, the name of the person who updated the pivot table is also provided as property **RefreshedByWho**. 

For a working example refer to the following article:

*   [Get PivotTable refresh date and refreshed by who information][5]

## Data Validation for Huge Numbers

Data validation is done in variety of ways to control the input in the Excel file. Like limit can be defined for a cell within which some number can be entered, otherwise error message is raised. Issues were faced for validation of large numbers like 12345678901 etc. in the past but now this much larger numbers are supported by Aspose.Cells.

For a working example along with a template file refer to the following article:

*   [Data validation for large numbers][6]

## Other Enhancements and Fixes

There are some other enhancements included and a few exceptions handled in the new release for the users. A few of the worth mentioning features and other improvements are as follows:

*   Text position changes a bit on ungrouping the shape
*   Handled ArgumentException while working with the generated HTML file
*   Handled an exception while calling AutoFitColumns operation
*   Handled CellsException during saving when ParsingFormulaOnOpen is set to false

In Aspose.Cells 18.11, we fixed several important bugs and other issues. For example, issues around reading/writing MS Excel file formats, reading/writing HTML files, applying data validation, applying auto-fit rows/columns, formatting cells, manipulating smart art shapes, manipulating named ranges, refreshing and calculating pivot tables, rendering and manipulating charts and shapes, [rendering images from Excel worksheets][7], [rendering images files from charts][8] and [exporting Excel workbooks to PDF format][9] have been resolved in the release. The Aspose.Cells formula calculation engine is further enhanced too.

## Changes to the Public API

The following is a list of any changes made to the public API such as added, renamed, removed or deprecated members as well as any non-backward compatible change made to Aspose.Cells for .NET:

*   Adds **PivotTable.RefreshedByWho property,** gets the name of the user who refreshed the PivotTable last time.
*   Adds **PivotTable.RefreshDate property,** gets the date when the PivotTable was refreshed last time.
*   Adds **CalculationData.CellRow/CellColumn properties, **provides an efficient way for the user to get the cell's row and column indices instead of fetching the Cell object.
*   Adds CalculationCell class, represents the calculation data about one cell being calculated.
*   Adds **AbstractCalculationMonitor.OnCircular(IEnumerator circularCellsData)** method, provides the method for the user to gather and process circular references.
*   Adds **TxtLoadOptions.TreatConsecutiveDelimitersAsOne property,** allows users to choose whether consecutive delimiters should be taken as one when importing the CSV file.
*   Adds **FormatCondition.SetFormulas(string formula1, string formula2, bool isR1C1, bool isLocal) method,**provides an efficient and convenient way for the user to set formulas for FormatCondition.
*   Adds **Validation.GetListValue(int row, int column) method,**allows users to get the value to produce the list for the Validation of specific cells.
*   **Obsoletes ValidationCollection.Add(Validation validation) method,** use ValidationCollection.Add(CellArea) method instead.
*   Adds **Validation.Copy(Aspose.Cells.Validation,Aspose.Cells.CopyOptions ) method,**copies validation.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][10].
*   [Install Aspose for .NET APIs from NuGet repository][11]
*   [Aspose.Cells for .NET Documentation][12] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][13] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][14] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][15] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Cells/18.11.0
[2]: https://docs.aspose.com/display/cellsnet/Detecting+Circular+Reference
[3]: https://docs.aspose.com/display/cellsnet/Replace+text+in+smart+art
[4]: https://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Different+Image+Formats#ConvertingWorksheettoDifferentImageFormats-ConvertingWorksheettoSVG
[5]: https://docs.aspose.com/display/cellsnet/Get+Pivot+Table+refresh+date+and+refresh+by+who+information
[6]: https://docs.aspose.com/display/cellsnet/Data+Validation#DataValidation-DataValidationRules
[7]: https://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Different+Image+Formats
[8]: https://docs.aspose.com/display/cellsnet/Chart+Rendering
[9]: https://docs.aspose.com/display/cellsnet/Convert+Excel+Workbook+to+PDF
[10]: https://products.aspose.com/cells/net
[11]: https://www.nuget.org/packages/Aspose.Cells
[12]: https://docs.aspose.com/display/cellsnet/home
[13]: https://apireference.aspose.com/
[14]: https://forum.aspose.com/c/cells
[15]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




