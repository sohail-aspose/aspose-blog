---
title: 'Enable Show Report Filter Pages Options using Aspose.Cells for JavaScript via Java 19.1'
date: Tue, 12 Feb 2019 08:38:43 +0000
draft: false
url: /2019/02/12/enable-show-report-filter-pages-options-in-excel/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

We are pleased to announce the release of [Aspose.Cells for JavaScript via Java 19.1][1]. This release includes new features, enhancements and bug fixes which further improve the overall stability and usability of the API. Since Aspose.Cells for JavaScript is a subset component, so it includes all the important and useful features present in its native Aspose.Cells for Java, please visit [features comparison page][2] for your reference. Aspose.Cells for JavaScript via Java has almost full functionality of Aspose.Cells for Java with a few limitations, minor API changes and additional requirements. See the following release notes on major features and other improvements for your reference

## Enable Show Report Filter Pages Option while Managing Pivot Table

Excel supports creating pivot tables, adding report filters and enable "Show Report Filter Pages" option. Aspose.Cells has also provided this support now to enable the "Show Report Filter Pages"option on created pivot table. As a result of this option the created workbook will contain more worksheets. It will split every possible value of report filter in a separate worksheet.

For a working example refer to the following article:

*   [Show report filter pages option][3]

## Support for legacy Excel 95/5.0

Excel 95 support was not available earlier which was causing issues in using legacy Excel 95/5.0 files. Aspose.Cells has provided the support for this old file format now. For this purpose FileFormatType.EXCEL\_95 is introduced which can be used for creating new workbook and LoadFormat.Auto can be used to open these file formats.

For a working example refer to the following article:

*   [Support for opening Excel95/5.0][4]

## Specify How to Cross String in Output PDF and Image

When a cell contains text or string but it is larger than the width of the cell, then the string overflows if the next cell in next column is null or empty. While saving Excel file into PDF/Image, we can control this overflow by specifying the cross type using the TextCrossType enumeration. It has the values TextCrossType.DEFAULT, TextCrossType.CROSS\_KEEP, TextCrossType.CROSS\_OVERRIDE and TextCrossType.STRICT\_IN\_CELL. This feature will create similar output as Excel while rendering sheets to PDF and images.

For a working example refer to the following article:

*   [Specify how to cross string in output PDF and image][5]

## Sorting Data Based on Cell Background Colour

Excel provides features to sort data based on background color. Same feature was required by users while using Aspose.Cells. This feature is provided now by using DataSorter where SortOnType.CELL\_COLOR can be used in addKey() to sort data based on background color. All the cells which contain specified color in the addKey() function are placed on top or bottom according to the SortOrder setting and order of the rest of the cells is not changed at all.

For a working example refer to the following article:

*   [Sorting data with background-color][6]

## Using Custom Functions From Add-in

There is a common scenario when there are custom formulas which we want to include as an excel add-in. While setting the cell.setFormula value to some function, built-in functions work fine however there is a need to set the custom functions or formulas using the add-in functions. Aspose.Cells provides features to register add-in functions using Worksheets.registerAddInFunction(). Afterwards when we set cell.setFormula(anyFunctionFromAddIn), the output Excel file will contain the calculated value from the Add-In function. This feature is available now where an add-in can be registered and function from the newly added add-in can be called.

For a working example refer to the following article:

*   [Registering and calling add-in function][7]

## Other Enhancements and Fixes

There are some other enhancements included and a few exceptions handled in the new release for the users. A few of the worth mentioning features and other improvements are as follows.

*   Bug removal for change in text color while converting ODS to XLSX
*   Support for preserving the strikethrough font while ODS to XLSX
*   Problem with strikethrough text in generated HTML file format
*   ODS to XLSX - Text box dimensions changed
*   ODS -> XLSX - Hyperlink is functional but shown as plain text
*   ODS to XLSX, Percentages are lost in bar graph chart
*   Some styles are not rendered in HTML input

In Aspose.Cells 19.1, we fixed several important bugs and other issues. For example, CellsException while converting files, Exception "java.lang.ArrayIndexOutOfBoundsException: -32768" when loading an XLSX file format and ArrayIndexOutOfBoundsException when loading a workbook.

## Changes to the Public API

The following is a list of any changes made to the public API such as added, renamed, removed or deprecated members as well as any non-backward compatible change made to Aspose.Cells for Java:

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
*   Deletes **Obsoletes Cell.SetAddInFormula() method, **register the addin functions firstly by WorksheetCollection.RegisterAddInFunction() and then setting the formula for Cell by Cell.Formula/Cell.SetFormula() instead.

## Aspose.Cells for JavaScript via Java Resources

The following are the links to some useful resources you may need to accomplish your tasks.

*   Aspose.Cells for JavaScript via Java Online Documentation (Aspose.Cells for JavaScript via Java is ported from Aspose.Cells for Java. So, you can use the same documentation)
*   Features
*   Release Notes
*   [Product Page][8]
*   [Download Aspose.Cells for JavaScript via Java][9]
*   [API Reference Guide][10] 
*   [Free Support Forum][11]
*   [Paid Support Helpdesk][12]




[1]: https://downloads.aspose.com/cells/javascript/new-releases/aspose.cells-for-javascript-via-java-19.1/
[2]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Node.js+via+Java+Features
[3]: https://docs.aspose.com/display/cellsjava/Show+Report+Filter+Pages+option
[4]: https://docs.aspose.com/display/cellsjava/Opening+Files+with+Different+Formats#OpeningFileswithDifferentFormats-OpeningMicrosoftExcel95/5.0Files
[5]: https://docs.aspose.com/display/cellsjava/Specify+how+to+cross+string+in+output+PDF+and+image
[6]: https://docs.aspose.com/display/cellsjava/Data+Sorting#DataSorting-Sortingdatawithbackgroundcolour
[7]: https://docs.aspose.com/display/cellsjava/Using+Formulas+or+Functions+to+Process+Data#UsingFormulasorFunctionstoProcessData-addin
[8]: https://www.aspose.com/products/cells/javascript
[9]: https://downloads.aspose.com/cells/javascript
[10]: https://apireference.aspose.com/javascript/cells
[11]: https://forum.aspose.com/c/cells
[12]: https://helpdesk.aspose.com/




