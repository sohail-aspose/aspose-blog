---
title: 'Parse HTML Tags while Importing Data to Excel using C#'
date: Mon, 04 Jan 2016 11:11:41 +0000
draft: false
url: /2016/01/04/parse-html-tags-while-importing-data-to-excel-using-csharp/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


Aspose.Cells for .NET 8.6.3 has been released. This release contains many useful features and other enhancements along with critical bug fixes. If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you to check the complete [Public API Changes][1] section to know what has been changed in the API so far. We have highlighted some important features (of this month's release) here.

## Import HTML Formatted Data

Aspose.Cells for .NET now allows you to respect HTML formatted values while importing data to spreadsheet. When HTML parsing is enabled while importing data, Aspose.Cells converts the HTML into corresponding cell formatting. This release of Aspose.Cells for .NET APIs has exposed the ImportTableOptions.IsHtmlString property which directs the APIs to parse the HTML tags while importing data onto the Worksheet and set the parsed result as cell value. See the document that explains how to [Import HTML Formatted Data][2].

## Load Only Visible Worksheets from Existing Spreadsheet

Aspose.Cells APIs provide a set of classes for the developers to influence the spreadsheet loading mechanism. While using the LoadOptions & LoadDataOptions classes, the developers can set a number of options such as force the API to load specific worksheets, where the worksheets can be specified via their indices or names.

Aspose.Cells for .NET 8.6.3 has exposed another useful property for the LoadDataOptions class which allows to load only the visible worksheets from an existing spreadsheet, where the hidden worksheets will be simply ignored and will not be available in the Aspose.Cells object model for any processing. The newly exposed property LoadDataOptions.OnlyVisibleWorksheet is of type Boolean; setting it to true means that the API will ignore the hidden worksheets and load only the visible worksheets for further processing.

The following piece of code demonstrates the usage of LoadDataOptions.OnlyVisibleWorksheet property to [load only visible worksheets][3].

```
string samplePath = "Sample.out.xlsx";

// Create a sample workbook
// and put some data in first cell of all 3 sheets
Workbook createWorkbook = new Workbook();
createWorkbook.Worksheets["Sheet1"].Cells["A1"].Value = "Aspose";
createWorkbook.Worksheets.Add("Sheet2").Cells["A1"].Value = "Aspose";
createWorkbook.Worksheets.Add("Sheet3").Cells["A1"].Value = "Aspose";
createWorkbook.Worksheets["Sheet3"].IsVisible = false;
createWorkbook.Save(samplePath);

// Load the sample workbook
LoadDataOption loadDataOption = new LoadDataOption();
loadDataOption.OnlyVisibleWorksheet = true;
LoadOptions loadOptions = new LoadOptions();
loadOptions.LoadDataAndFormatting = true;
loadOptions.LoadDataOptions = loadDataOption;

Workbook loadWorkbook = new Workbook(samplePath, loadOptions);
Console.WriteLine("Sheet1: A1: {0}", loadWorkbook.Worksheets["Sheet1"].Cells["A1"].Value);
Console.WriteLine("Sheet1: A2: {0}", loadWorkbook.Worksheets["Sheet2"].Cells["A1"].Value);
Console.WriteLine("Sheet1: A3: {0}", loadWorkbook.Worksheets["Sheet3"].Cells["A1"].Value); 
```

## Create MS Excel's Built-in Styles

Aspose.Cells for .NET 8.6.3 has exposed the Workbook.CreateBuiltinStyle method that can be used to create an object of the Style class that corresponds to one of the built-in styles offered by the MS Excel. The Workbook.CreateBuiltinStyle method accepts a constant from the enumeration BuiltinStyleType.

Please note, with previous releases of the Aspose.Cells APIs, same task could be accomplished via StyleCollection.CreateBuiltinStyle method but as the recent releases of Aspose.Cells APIs have removed the StyleCollection class from the public API therefore the newly exposed Workbook.CreateBuiltinStyle method can be considered as an alternative approach to achieve the same goal.

The following sample code explains how to create Excel's built-in styles.

```
//Create an instance of Workbook
//Optionally load a spreadsheet
Workbook workbook = new Workbook();

//Create a built-in style of type Title
Style style = workbook.CreateBuiltinStyle(BuiltinStyleType.Title); 
```

## Other Enhancements & Fixes

The most notable enhancements in this release are as follow:

*   Exposed an overloaded version of the Cells.ImportGridView that can now accept an instance of ImportTableOptions to give more control over the import process.
*   Supported the Print Page Size Thermal 3x11.
*   Provided support for nested object collection in Smart Markers.

We have handled a few exceptions regarding reading/writing Excel file formats and rendering to PDF documents.

Moreover, in the new release, we have also fixed a few issues in the grid controls provided by Aspose.Cells for .NET.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 8.6.3, please visit the [download page][4].




[1]: https://docs.aspose.com/cells/net/migrating-from-earlier-versions-of-aspose-cells/
[2]: https://docs.aspose.com/cells/net/import-data-into-worksheet/#importing-html-formatted-data
[3]: https://docs.aspose.com/cells/net/different-ways-to-open-files/#loading-visible-sheets-only
[4]: https://downloads.aspose.com/cells/net/




