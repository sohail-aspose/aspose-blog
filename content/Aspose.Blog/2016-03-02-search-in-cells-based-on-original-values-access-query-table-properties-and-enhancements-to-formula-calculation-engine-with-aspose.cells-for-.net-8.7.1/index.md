---
title: 'Search in Cells based on Original Values, Access Query Table Properties and Enhancements to Formula Calculation Engine with Aspose.Cells for .NET 8.7.1'
date: Wed, 02 Mar 2016 11:39:51 +0000
draft: false
url: /2016/03/02/search-in-cells-based-on-original-values-access-query-table-properties-and-enhancements-to-formula-calculation-engine-with-aspose.cells-for-.net-8.7.1/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for .NET logo][1]](https://www.aspose.com/ "Aspose.Cells for .NET API")Aspose.Cells for .NET 8.7.1 has been released. This release contains some valuable features and other enhancements along with critical bug fixes. If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you to check the complete Public API Changes section to know what APIs are changed so far. We have highlighted some important features (of this month's release) here.

While you are downloading the latest build, we provide details about the biggest features in this release.

## Search in Cells Based on Original Values

Aspose.Cells APIs already support the Find or Search Data feature for spreadsheets in order to find some particular piece of contents in cell value & formula. However, this feature was lacking the aspect of formatting applied onto the cell that may change the appearance as well as the underlying value of the cell, consequently making the content unsearchable using the original value. With this release of Aspose.Cells for .NET API, another enum constant by the name LookInType.OriginalValues has been exposed to the public API which allows to overcome the situation as discussed above.

The following piece of code demonstrates the usage of LookInType.OriginalValues attribute to search the cells based on original values.

```
//Create workbook object
Workbook workbook = new Workbook();

//Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];

//Add 10 in cell A1 and A2
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(10);

//Add Sum formula in cell D4 but customize it as ---
Cell cell = worksheet.Cells["D4"];

Style style = cell.GetStyle();
style.Custom = "---";
cell.SetStyle(style);

//The result of formula will be 20
//but 20 will not be visible because
//the cell is formated as ---
cell.Formula = "=Sum(A1:A2)";

//Calculate the workbook
workbook.CalculateFormula();

//Create find options, we will search 20 using
//original values otherwise 20 will never be found
//because it is formatted as ---
FindOptions options = new FindOptions();
options.LookInType = LookInType.OriginalValues;
options.LookAtType = LookAtType.EntireContent;

Cell foundCell = null;
object obj = 20;

//Find 20 which is Sum(A1:A2) and formatted as ---
foundCell = worksheet.Cells.Find(obj, foundCell, options);

//Print the found cell
Console.WriteLine(foundCell);

//Save the workbook
workbook.Save("output.xlsx"); 
```

## Access Query Table Properties

Aspose.Cells for .NET 8.7.1 has exposed the boolean type QueryTable.PreserveFormatting & QueryTable.AdjustColumnWidth properties in order to mimic the MS Excel's features of preserving cell formatting & adjusting column widths while working with External Data Range of type Query Table.

Please note, Excel application provides these options to influence the formatting of the data where the options can be accessed on Excel interface from **Data** tab by clicking the **Properties** button as shown below.

The following piece of code shows the simple usage scenario of QueryTable.PreserveFormatting &QueryTable.AdjustColumnWidth properties.

```
//Create workbook from source excel file
Workbook workbook = new Workbook("Sample.xlsx");

//Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];

//Access first Query Table
QueryTable qt = worksheet.QueryTables[0];

//Print Query Table Data
Console.WriteLine("Adjust Column Width: " + qt.AdjustColumnWidth);
Console.WriteLine("Preserve Formatting: " + qt.PreserveFormatting);

//Now set Preserve Formatting to true
qt.PreserveFormatting = true;

//Save the workbook
workbook.Save("Output.xlsx"); 
```

## Enhancements to Formula Calculation Engine

Aspose.Cells APIs have enhanced the formula calculation engine with this release where the most worth mentioning enhancements are as follow.

### Support for Array Formulas of Data Tables

In perspective of Excel application, Data tables are part of a suite of commands that are called what-if analysis tools. These tools can be used to process the formulas by changing the values in cells to see how those changes will affect the outcome of formulas on the worksheet. With this release of Aspose.Cells for .NET, the API now allows you to calculate the array formula of Data Tables. Please note, no new API have been exposed for this feature and all enhancements are done internally to the formula calculation engine therefore by simply calling the Workbook.CalculateFormula method, all formulas including the array formulas will be computed automatically.

### Support for FORMULATEXT Function

Aspose.Cells for .NET 8.7.1 has provided support for the MS Excel's FORMULATEXT Function which can be used to get the formula string for any given cell as it is being displayed in the Excel's formula bar.

## Other Enhancements and Fixes

We have handled a few exceptions regarding reading/writing Excel files and copying worksheets.

In this release, several important issues have been addressed. For example, issues around manipulating Microsoft Excel file formats, manipulating List Objects, manipulating named ranges, encrypting files, rendering to HTML file format, rendering images from Excel worksheets, manipulating charts, rendering images files from charts and exporting Excel workbooks to PDF format have been resolved.

Moreover, in the new release, we have also fixed an issue regarding removing rows in the desktop based grid control provided by Aspose.Cells for .NET.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 8.7.1, please visit the [download page][2].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png "Aspose.Cells for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.cells-for-.net/entry693090.aspx




