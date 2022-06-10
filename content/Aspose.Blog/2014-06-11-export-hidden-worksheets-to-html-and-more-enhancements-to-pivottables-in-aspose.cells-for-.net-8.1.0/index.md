---
title: 'Export Hidden Worksheets to HTML and more Enhancements to PivotTables in Aspose.Cells for .NET 8.1.0'
date: Wed, 11 Jun 2014 09:05:10 +0000
draft: false
url: /2014/06/11/export-hidden-worksheets-to-html-and-more-enhancements-to-pivottables-in-aspose.cells-for-.net-8.1.0/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for .NET logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png)Aspose.Cells for .NET 8.1.0 has been released. The new release contains many useful improvements.  It also includes several fixes and other enhancements. Before you go ahead and start exploring the new features and other enhancements, we will list here some major features and other enhancements in this month’s release.

## New Enhancements to the PivotTable Class

Aspose.Cells has exposed the getter/setters for the DisplayNullString & NullString properties for the PivotTable class to handle the pivot table option "For empty cells show" offered by Microsoft Excel. These properties allow users to set display option for the empty cells inside the Pivot Table to any specified string. Please check the detailed article on Setting Pivot Table Option - For empty cells show.

## Enhancements to the HtmlSaveOptions Class

Aspose.Cells for .NET API now provides ExportHiddenWorksheet property exposed by the HtmlSaveOptions class. The Boolean property allows users to choose whether to render the hidden worksheets or not. The default value is true which means that the hidden worksheet will be rendered as HTML; switching the to false excludes hidden worksheets from the rendering process. More details on this topic can be found on the Prevent Exporting Hidden Worksheet Contents while Saving to HTML.

## Added Cell.StringValueWithoutFormat Property

The StringValueWithoutFormat property has been added to the Cell Class, in order to let developers retrieve the cell value without formatting applied. The code snippet below demonstrate how to use Cell.StringValueWithoutFormat property as compared to the Cell.DisplayStringValue by creating a spreadsheet from the scratch and applying the number format to one of the cells.

```
 //Create an instance of Workbook 
Workbook book = new Workbook();

//Access first worksheet
Worksheet sheet = book.Worksheets[0];

//Access A1 cell
Cell cell = sheet.Cells["A1"];

//Put a value cell and convert it to number
cell.PutValue("123456", true);

//Create a new Style object and add it to Workbook's Style Collection
Style style = book.Styles[book.Styles.Add()];

//Set Number format for Style object
style.Number = 3;

//Set the style of A1 cell
cell.SetStyle(style, new StyleFlag() { NumberFormat = true });

//Get formatted string value
string formatted = cell.DisplayStringValue;
Console.WriteLine(formatted);

//Get un-formatted string value
string unformatted = cell.StringValueWithoutFormat;
Console.WriteLine(unformatted); 
```

## Other Enhancements and Fixes

In the new version, we have fixed an exception while saving XLSX file to CSV file format.

In this release, several important issues have been addressed. For example, issues around reading and writing Microsoft Excel file formats (XLS, XLSX, XLSB etc.), manipulating style and formatting, rendering and manipulating pivot tables, rendering images from Excel worksheets, Smart Markers, adding page breaks, rendering and manipulating charts, rendering images files from charts and exporting Excel workbooks to PDF format have been resolved. A few enhancements have also been made to Aspose.Cells for .NET's formula calculation engine, we have also improved the performance when applying formatting to Pivot Tables.

We also fixed a bug in the web based Grid control provided by Aspose.Cells for .NET regarding worksheets navigation after loading the Excel file to GridWeb.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 8.1.0, please visit the [download page][2].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png "Aspose.Cells for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.cells-for-.net/entry551086.aspx




