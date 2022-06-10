---
title: 'Update Smart Art Text in Excel Worksheets using Java'
date: Fri, 07 Dec 2018 13:03:27 +0000
draft: false
url: /2018/12/07/update-smart-art-text-and-large-numbers-validation-with-aspose.cells-18.11/
author: Ahsaniqbal
summary: ''
tags: ['Update Smart Art Text in Excel Worksheets']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="">}}


We are pleased to announce the release of new updated version [Aspose.Cells for Java v18.11.][1] It contains enhancements and bugs resolution for many of the issues. Whenever some enhancement or new feature is requested, effort is made to provide more and more additional features to help the common users. New properties, methods and classes are added to support these features along with special focus on achieving maximum possible performance.

Detailed overview of all the enhancements, bugs and changes in the APIs are documented and shared with the user as [Release notes][2]. This document can be used as a reference to keep track of all the changes which are made in the current and previous versions. Smart art is addressed in this release such that text can be updated in the shapes. This feature will enable users to modify these objects at runtime rather than fixed text in the shapes. Last section on this page contains more details and links about this product. Aspose for Java APIs can be directly installed from Maven repository for which check the [document][3].

## Update Smart Art Text in Excel using Java

Smart art is used for better representation of information however earlier the text in the smart art shapes was fixed. This limitation is gone now as now smart art text can be updated. For this purpose shape.setText() function is introduced which sets new text in the smart art shape.  

For a working example refer to the following article:

*   [Replace smart art text][4]

## Pivot Table Refresh Date/Time and Refreshed by Who

Pivot tables are very common reports which are present in the workbooks. These reports are updated time by time and it is important to know the last time when the report was updated for better decision making. Aspose.Cells has provided this feature by introducing property RefreshDate. Similarly, name of the person who updated the pivot table is also provided as property RefreshedByWho. 

For a working example refer to the following article:

*   [Get PivotTable refresh date and refreshed by who information][5]

## Data Validation for Huge Numbers

Data validation is done in a variety of ways to control the input in the Excel file. Like limit can be defined for a cell within which some number can be entered, otherwise an error message is raised. Issues were faced for validation of large numbers like 12345678901 etc. in the past but now these much large numbers are supported by Aspose.Cells.

For a working example along with a template file refer to the following article:

*   [Data validation for large numbers][6]

## Rendering Active Worksheet in a Workbook to SVG

Aspose.Cells has introduced rendering active worksheet in a workbook to SVG. For this purpose load an Excel file into the workbook object and set the active sheet index like for Sheet2, set index to 1. Then save the Workbook as SVG which will render active worksheet to SVG:

For a working example refer to the following article:

*   [Rendering active worksheet in a workbook][7]

## Other Enhancements and Fixes

There are some other enhancements included and a few exceptions handled in the new release for the users. A few of the worth mentioning features and other improvements are as follows:

*   The wrong count of validation values is read from XLSX
*   Issue while treating consecutive delimiters as distinct
*   Date format is incorrect for Japanese locale
*   Aspose.Cells.GridWeb (Java) crashes when using it concurrently in a multi user environment
*   Resolving issues in getting actual chart size

In Aspose.Cells 18.11, we fixed several important bugs and other issues. For example, not copying the smart art while copying the workbook, detecting the circular reference in a workbook and treating consecutive delimiters as one similar to Excel.

## Changes to the Public API

The following is a list of any changes made to the public API such as added, renamed, removed or deprecated members as well as any non-backward compatible change made to Aspose.Cells for Java:

*   Adds **PivotTable.RefreshedByWho property,** gets the name of the user who refreshed the PivotTable last time.
*   Adds **PivotTable.RefreshDate property, g**ets the date when the PivotTable was refreshed last time.
*   Adds **CalculationData.CellRow/CellColumn properties, **provides efficient way for user to get cell's row and column indices instead of fetching the Cell object.
*   Adds **CalculationCell class,**represents the calculation data about one cell being calculated.
*   Adds **AbstractCalculationMonitor.OnCircular(IEnumerator circularCellsData) method,**provides method for user to gather and process circular references.
*   Adds **TxtLoadOptions.TreatConsecutiveDelimitersAsOne property,** allows user to choose whether consecutive delimiters should be taken as one when importing CSV file.
*   Adds **FormatCondition.SetFormulas(string formula1, string formula2, bool isR1C1, bool isLocal) method,**provides efficient and convenient way for user to set formulas for FormatCondition.
*   Adds **Validation.GetListValue(int row, int column) method,**allows user to get the value to produce the list for the Validation of specific cell.
*   **Obsoletes ValidationCollection.Add(Validation validation) method,** use ValidationCollection.Add(CellArea) method instead.
*   Adds **Validation.Copy(Aspose.Cells.Validation,Aspose.Cells.CopyOptions ) method,**copies validation.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][8].
*   [Download Aspose.Cells for Java][9].
*   [Aspose.Cells for Java Documentation][10] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][11] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][12] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for Java Examples][13] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://artifact.aspose.com/repo/com/aspose/aspose-cells/18.11/
[2]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+18.11+Release+Notes
[3]: https://docs.aspose.com/display/cellsjava/Installation#Installation-InstallingAspose.CellsforJavafromMavenRepository
[4]: https://docs.aspose.com/display/cellsjava/Replace+text+in+smart+art
[5]: https://docs.aspose.com/display/cellsjava/Get+Pivot+Table+refresh+date+and+refresh+by+who+information
[6]: https://docs.aspose.com/display/cellsjava/Data+Validation#DataValidation-DataValidationRules
[7]: https://docs.aspose.com/display/cellsjava/Converting+Worksheet+to+Different+Image+Formats#ConvertingWorksheettoDifferentImageFormats-Renderactiveworksheetinaworkbook
[8]: https://products.aspose.com/cells/java
[9]: https://artifact.aspose.com/repo/com/aspose/aspose-cells/
[10]: https://docs.aspose.com/display/cellsjava/home
[11]: https://apireference.aspose.com/java/cells
[12]: https://forum.aspose.com/c/cells
[13]: https://github.com/aspose-cells/Aspose.Cells-for-Java




