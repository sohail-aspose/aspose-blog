---
title: 'Show Report Filter Pages Option in PivotTables in Excel using Aspose.Cells for .NET 19.1'
date: Tue, 05 Feb 2019 18:50:06 +0000
draft: false
url: /2019/02/05/show-report-filter-pages-in-excel-pivot-tables-sort-data-based-on-background-color-using-csharp/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce the release of [Aspose.Cells for .NET v19.1][1], the MS Excel file formats API that provides the ability to create, manipulate, convert or render MS Excel spreadsheets, and more importantly - is fully documented. Please check the [document][2] on how to install Aspose for .NET APIs directly from NuGet repository. We have added a few important features and other enhancements while keeping the product more stable and feature rich API. We also included important bug fixes as a part of this release. Moreover, fixing bugs and issues leads us to new enhancements and features which increases our customer base.

Please check the [release notes][3] which cover all the new features, enhancements and list of bugs that are resolved in this new version. New features are always introduced while enhancing this product which helps us to compete with the ever-growing software industry. Exceptions handling empowers the developers to keep control of the applications and assist users in a better way to continue using the application without any interruption. You will get an idea about what is new and what has been enhanced or fixed with this revision of Aspose.Cells for .NET.

## Show Report Filter Pages Option in Pivot Table

MS Excel supports creating PivotTables, adding report filters, and enabling the "Show Report Filter Pages" option. Aspose.Cells has also provided this support now to enable the "Show Report Filter Pages" option on the created pivot table. As a result of this option, the created workbook will contain more worksheets in it. It will split every possible value of the report filter in a separate worksheet.

For a working example refer to the following article:

*   [Show report filter pages option][4]

## Work with Legacy Excel 95/5.0

MS Excel 95 support was not available earlier which was causing issues when using legacy Excel 95/5.0 files. This support is available now and these older file formats can be used now. For this purpose **FileFormatType.Excel95** is introduced which can be used for opening these file formats.

For a working example refer to the following article:

*   [Support for opening Excel95/5.0][5]

## Specify How to Cross String in Output PDF and Image

When the cell contains text or string but it is larger than the width of the cell, then the string overflows if the next cell in the next column is null or empty. When the MS Excel file is saved into PDF/Image, we can control this overflow by specifying the cross-type using the **TextCrossType** enumeration. It has the values **TextCrossType.Default**, **TextCrossType.CrossKeep**, **TextCrossType.CrossOverride** and **TextCrossType.StrictInCell**. This feature will create a similar output as Excel while rendering sheets to PDF and images.

For a working example refer to the following article:

*   [Specify how to cross string in output PDF and image][6]

## Sorting Data Based on Cell Background Color

MS Excel provides a **feature to sort data based on the** background color. The same feature was required by some users while using Aspose.Cells. This feature is provided now by using DataSorter where SortOnType.CellColor can be used in the AddKey method to sort data based on the background color. All the cells which contain specified color in the AddKey(), function are placed on top or bottom according to the SortOrder setting, and the order of the rest of the cells is not changed at all.

For a working example refer to the following article:

*   [Sorting data with background color][7]

## Using custom functions from Add-in  

In a common scenario, there can be custom formulas that we want to include as an Excel add-in. Setting the Cell.Formula value to some function, built-in functions work fine however there can be a need to set the custom functions or formulas using the add-in functions. Aspose.Cells provides features to register to add-in functions using Worksheets.RegisterAddInFunction method. Afterward when we set **Cell.Formula** attribute, the output Excel file shall contain the calculated value from the AddIn function. This feature is available now where an add-in can be registered and function from the newly added add-in can be called.

For a working example refer to the following article:

*   [Registering and calling add-in function][8]

## Other Enhancements and Fixes

There are some other enhancements included and a few exceptions handled in the new release for the users. A few of the worth mentioning features and other improvements are as follows:

*   Detect if generated MHT file is a worksheet or not
*   Handled an exception that raised while converting to the Open Strict XML format
*   Handled an exception when loading an XLSB/XLSX file format
*   Handled an exception while calling Cells.DeleteBlankRows

In Aspose.Cells 19.1, we fixed several important bugs and other issues. For example, issues around reading/writing MS Excel file formats, using PageSetup options, importing objects into the worksheet, manipulating rows and columns, refreshing and calculating pivot tables, rendering and manipulating charts and shapes, [rendering images from Excel worksheets][9], [rendering images files from charts][10] and [exporting Excel workbooks to PDF format][11] have been resolved in the release. Moreover, Aspose.Cells formula calculation engine is further improved.

## Changes to the Public API

The following is a list of any changes made to the public API such as added, renamed, removed or deprecated members as well as any non-backward compatible change made to Aspose.Cells for .NET:

*   Adds **PivotTable.ShowReportFilterPageByName (string fieldName) method,** shows all the report filter pages according to PivotField's name, the PivotField must be located in the PageFields.
*   Adds **PivotTable.ShowReportFilterPageByIndex(int posIndex) method** , shows all the report filter pages according to the position index in the PageFields.  
    
*   Adds **PivotTable.ShowReportFilterPage(PivotField pageField) method, **shows all the report filter pages according to PivotField, the PivotField must be located in the PageFields.
*   Adds **DataSorterKey and DataSorterKeyCollection class **, represents the key of the data sorter.
*   Adds **DataSorter.AddKey(Int32,SortOnType,SortOrder,Object) method, **adds the sort key such as cell's background color, font color.
*   Adds **Aspose.Cells.DataSorter.Keys property, **gets all keys of the data sorter.
*   Adds **SortOnType enum, **represents the type of sorted data.
*   Adds **ODSLoadOptions class,** represents the options of loading ODS file.
*   Adds **HTMLLoadOptions.ProgId property, **gets the program id of creating the file. used only for MHT files.
*   Adds **PdfSaveOptions.TextCrossType property, **gets or sets displaying text type when the text width is larger than cell width.
*   Adds **TextCrossType enum class, **Enumerates displaying text type when the text width is larger than cell width.
*   Adds **WorksheetCollection.RegisterAddInFunction() methods, **replacement of Cell.SetAddInFormula(), a more convenient and efficient way for users to add and use addin functions.
*   Obsoletes **Cell.SetAddInFormula() method,**register the addin functions firstly by WorksheetCollection.RegisterAddInFunction() and then set the formula for Cell by Cell.Formula/Cell.SetFormula() instead.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][12].
*   [Install Aspose for .NET APIs from NuGet repository][13]
*   [Aspose.Cells for .NET Documentation][14] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][15] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][16] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][17] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Cells/19.1.0
[2]: https://docs.aspose.com/display/cellsnet/Installation#Installation-InstallAspose.Cellsfor.NETthroughNuGet
[3]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+19.1+Release+Notes
[4]: https://docs.aspose.com/display/cellsnet/Show+Report+Filter+Pages+option
[5]: https://docs.aspose.com/display/cellsnet/Opening+Different+Microsoft+Excel+Versions+Files#OpeningDifferentMicrosoftExcelVersionsFiles-OpeningMicrosoftExcel95/5.0Files
[6]: https://docs.aspose.com/display/cellsnet/Specify+how+to+cross+string+in+output+PDF+and+image
[7]: https://docs.aspose.com/display/cellsnet/Data+Sorting#DataSorting-Sortingdatawithbackgroundcolour
[8]: https://docs.aspose.com/display/cellsnet/Using+Formulas+or+Functions+to+Process+Data#UsingFormulasorFunctionstoProcessData-UsingAdd-inFunctions
[9]: https://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Different+Image+Formats
[10]: https://docs.aspose.com/display/cellsnet/Chart+Rendering
[11]: https://docs.aspose.com/display/cellsnet/Convert+Excel+Workbook+to+PDF
[12]: https://products.aspose.com/cells/net
[13]: https://www.nuget.org/packages/Aspose.Cells
[14]: https://docs.aspose.com/display/cellsnet/home
[15]: https://apireference.aspose.com/
[16]: https://forum.aspose.com/c/cells
[17]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




