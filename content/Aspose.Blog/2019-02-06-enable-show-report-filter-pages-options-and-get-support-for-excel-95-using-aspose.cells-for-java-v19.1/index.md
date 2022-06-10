---
title: 'Enable Show Report Filter Pages and Work with Excel 95 in Java'
date: Wed, 06 Feb 2019 02:27:14 +0000
draft: false
url: /2019/02/06/enable-show-report-filter-pages-options-and-get-support-for-excel-95-using-aspose.cells-for-java-v19.1/
author: Ahsaniqbal
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="">}}


It is a pleasure for us to announce the release of the new updated version Aspose.Cells for Java v19.1 with exciting new features. This time along with adding new features, we have resolved many bugs and handled exceptions to assist the developers' community. Aspose is committed to achieving maximum user satisfaction by providing innovative solutions and enhancements. We are always in the process of making improvements by analyzing different features of Excel and providing support for the same in our product.

[Release notes][1] is one of the important document where all the detailed information is available about the changes made in the new release.  This time new features are introduced like "Show report filter pages option", using text cross-type option to handle overflowing cell content, support for legacy Excel 95/5.0, and sorting data based on the background color. You may go through the release notes to have a glimpse of all the changes in this new version. For more details about this product, you may visit the links in the last section of this document. For an easy access and utilization  Aspose for Java APIs can be directly installed from Maven repository for which check [document][2].

## Enable Show Report Filter Pages Option in Excel

Excel supports creating pivot tables, adding report filters and enable "Show Report Filter Pages" option. Aspose.Cells has also provided this support now to enable the "Show Report Filter Pages"option on created pivot table. As a result of this option the created workbook will contain more worksheets. It will split every possible value of report filter in a separate worksheet.

For a working example refer to the following article:

*   [Show report filter pages option][3]

## Support for legacy Excel 95/5.0

Excel 95 support was not available earlier which was causing issues in using legacy Excel 95/5.0 files. Aspose.Cells has provided the support for this old file format now. For this purpose FileFormatType.EXCEL\_95 is introduced which can be used for creating new workbook and LoadFormat.Auto can be used to open these file formats.

For a working example refer to the following article:

*   [Support for opening Excel95/5.0][4]

## Specify How to Cross String in Output PDF and Image

When a cell contains text or string but it is larger than the width of the cell, then the string overflows if the next cell in next column is null or empty. While saving Excel file into PDF/Image, we can control this overflow by specifying the cross-type using the TextCrossType enumeration. It has the values TextCrossType.DEFAULT, TextCrossType.CROSS\_KEEP, TextCrossType.CROSS\_OVERRIDE and TextCrossType.STRICT\_IN\_CELL. This feature will create similar output as Excel while rendering sheets to PDF and images.

For a working example refer to the following article:

*   [Specify how to cross string in output PDF and image][5]

## Sorting Data Based on Cell's Background Color

Excel provides feature to sort data based on background color. Same feature was required by users while using Aspose.Cells. This feature is provided now by using DataSorter where SortOnType.CELL\_COLOR can be used in addKey() to sort data based on background color. All the cells which contain specified color in the addKey() function are placed on top or bottom according to the SortOrder setting and order of the rest of the cells is not changed at all.

For a working example refer to the following article:

*   [Sorting data with background color][6]

## Using Custom Functions from Add-in  

There is a common scenario when there are custom formulas which we want to include as an excel add-in. While setting the cell.setFormula value to some function, built-in functions work fine however there is a need to set the custom functions or formulas using the add-in functions. Aspose.Cells provides features to register add in functions using Worksheets.registerAddInFunction(). Afterwards when we set cell.setFormula(anyFunctionFromAddIn), the output Excel file will contain the calculated value from the Add-In function. This feature is available now where an add-in can be registered and function from the newly added add-in can be called.

For a working example refer to the following article:

*   [Registering and calling add-in function][7]

## Other Enhancements and Fixes

There are some other enhancements included and a few exceptions handled in the new release for the users. A few of the worth mentioning features and other improvements are as follows.

*   Bug removal for change in text color while converting ODS to XLSX
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

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][8].
*   [Download Aspose.Cells for Java][9].
*   [Aspose.Cells for Java Documentation][10] – up-to-date documentation containing Programmer’s Guide, Knowledge Base, and much more.
*   [Aspose.Cells for Java API Reference Guide][11] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][12] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for Java Examples][13] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+18.12+Release+Notes
[2]: https://docs.aspose.com/display/cellsjava/Installation#Installation-InstallingAspose.CellsforJavafromMavenRepository
[3]: https://docs.aspose.com/display/cellsjava/Show+Report+Filter+Pages+option
[4]: https://docs.aspose.com/display/cellsjava/Opening+Files+with+Different+Formats#OpeningFileswithDifferentFormats-OpeningMicrosoftExcel95/5.0Files
[5]: https://docs.aspose.com/display/cellsjava/Specify+how+to+cross+string+in+output+PDF+and+image
[6]: https://docs.aspose.com/display/cellsjava/Data+Sorting#DataSorting-Sortingdatawithbackgroundcolour
[7]: https://docs.aspose.com/display/cellsjava/Using+Formulas+or+Functions+to+Process+Data#UsingFormulasorFunctionstoProcessData-addin
[8]: https://products.aspose.com/cells/java
[9]: https://artifact.aspose.com/repo/com/aspose/aspose-cells/
[10]: https://docs.aspose.com/display/cellsjava/home
[11]: https://apireference.aspose.com/java/cells
[12]: https://forum.aspose.com/c/cells
[13]: https://github.com/aspose-cells/Aspose.Cells-for-Java




