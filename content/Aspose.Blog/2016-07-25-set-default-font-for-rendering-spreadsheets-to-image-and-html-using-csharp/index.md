---
title: 'Set Default Font for Rendering Spreadsheets to Image and HTML using C#'
date: Mon, 25 Jul 2016 11:03:37 +0000
draft: false
url: /2016/07/25/set-default-font-for-rendering-spreadsheets-to-image-and-html-using-csharp/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce our next version of [Aspose.Cells for .NET v8.9.0][1]. This release includes some new features and other enhancements with critical bug fixes. Please see the release notes in order to know what is new and what has been changed/fixed with this version of Aspose.Cells for .NET. If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you to check the complete Public API Changes section to know what APIs are changed so far. We have highlighted some important features and other enhancements here.

## Set Default Font for Rendering Spreadsheets to Image Formats

Aspose.Cells for .NET API has provided the ability to specify the default font name for rendering spreadsheets to image formats by exposing the ImageOrPrintOptions.DefaultFont property. The DefaultFont property is of type System.String with default value as null. The said property can be used when Unicode characters in the spreadsheet have not been formatted with appropriate font in the cell's style, consequently such characters may appear as blocks in the resultant images. It is advised to set the DefaultFont property to MingLiu or MS Gothic to show Unicode characters. If the DefaultFont property is not set, Aspose.Cells for .NET API will use the system's default font to show the Unicode characters.

Below provided code snippet demonstrates the simple usage scenario of newly exposed ImageOrPrintOptions.DefaultFont. Please check the detailed article on Setting Default Font for Rendering Spreadsheets in Image Formats if you wish to get more in-depth understanding of the aforementioned feature.

```
// Create an instance of ImageOrPrintOptions
var options = new ImageOrPrintOptions();
// Set default font name for image rendering
options.DefaultFont = "Arial";

// Load a spreadsheet in an instance of Workbook
var book = new Workbook(dir + "sample.xlsx");
// Access the worksheet to be rendered
var sheet = book.Worksheets[0];

// Create an instance of SheetRender
var render = new SheetRender(sheet, options);
// Save spreadsheet to image
render.ToImage(0, dir + "output.png");
```

## Set Default Font for Rendering Spreadsheets to HTML

Aspose.Cells for .NET 8.9.0 has exposed the DefaultFontName property for the HtmlSaveOptions class that allows to specify the default font name while rendering spreadsheets to HTML format. The default font will be used only when a particular font used to format some contents in the spreadsheet does not exist on the machine where conversion process has to take place. The default value of HtmlSaveOptions.DefaultFontName property is null that means, Aspose.Cells for .NET API will use the universal font which has the same family with the original font.

Below provided code snippet demonstrates the simple usage scenario of newly exposed HtmlSaveOptions.DefaultFontName. In order to get a more detailed understanding of this feature, please check the article on Setting Default Font for Rendering Spreadsheets to HTML Format.

```
// Create an instance of HtmlSaveOptions
var options = new HtmlSaveOptions();
// Set default font name for Html rendering
options.DefaultFontName = "Arial";

// Load a spreadsheet in an instance of Workbook
var book = new Workbook(dir + "sample.xlsx");
// Save the spreadsheet in Html format while passing instance of HtmlSaveOptions
book.Save(dir + "output.html", options);
```

## Impose Restrictions of Excel 2003 while Refreshing Pivot Table

Aspose.Cells for .NET API has exposed the Boolean type IsExcel2003Compatible property for the PivotTable class which allows to specify if a given PivotTable is Excel 2003 compatible for refreshing purposes. The default value of IsExcel2003Compatible property is true, that means a string must be less than or equal to 255 characters. If the string is greater than 255 characters, it will be truncated. If false, the aforementioned restriction will not be imposed.

Below provided code snippet demonstrates the simple usage scenario of PivotTable.IsExcel2003Compatible property. In order to get a more detailed understanding of this feature, please check the article on Compatibility for Excel 2003 while Refreshing Pivot Tables.

```
// Load a spreadsheet in an instance of Workbook
var book = new Workbook(dir + "sample.xlsx");

// Access the desired Pivot Table from the spreadsheet
var pivot = book.Worksheets[0].PivotTables[0];

// Set Excel 2003 compatibility to false
pivot.IsExcel2003Compatible = false;

// Refresh & recalculate Pivot Table
pivot.RefreshData();
pivot.CalculateData();
```

## Other Enhancements and Fixes

The most notable enhancements in this release are as follow:

*   Expanding text from right to left while exporting spreadsheets to HTML.
*   Get the Release or Running Version of Aspose.Cells.GridWeb.
*   Add or Remove Context Menu Items in Aspose.Cells.GridWeb.

We have handled a few exceptions regarding reading and writing Excel and HTML file formats. We have also handled an exception when calling Autofit operation on a worksheet.

In this release, several important issues have been addressed. For example, issues around reading and writing Microsoft Excel file formats, copying worksheets, manipulating PivotTables, adding List Objects/Tables, converting spreadsheets to HTML files and vice versa, manipulating and rendering charts and shapes, rendering images from Excel worksheets, rendering images files from charts and exporting Excel workbooks to PDF format have been resolved. We have also enhanced the Aspose.Cells' formula calculation engine and fixed a few issues in this regard.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][2].
*   [Aspose.Cells for .NET Download Section][3].
*   [Aspose.Cells for .NET Documentation][4] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][5] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][6] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][7] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/net
[2]: https://products.aspose.com/cells/net
[3]: https://downloads.aspose.com/cells/net
[4]: https://docs.aspose.com/cells/net
[5]: https://apireference.aspose.com/cells/net
[6]: https://forum.aspose.com/
[7]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




