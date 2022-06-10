---
title: 'Save Charts to SVG format, Get Equation Text of Chart Trendline and Retrieve Workbook State with Aspose.Cells for .NET 8.3.0'
date: Thu, 20 Nov 2014 09:01:36 +0000
draft: false
url: /2014/11/20/save-charts-to-svg-format-get-equation-text-of-chart-trendline-and-retrieve-workbook-state-with-aspose.cells-for-.net-8.3.0/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Total Product Family', 'Aspose.Cells Product Family']
---

[![Aspose.Cells for .NET logo][1]](https://www.aspose.com/ "Aspose.Cells for .NET API")Aspose.Cells for .NET 8.3.0 has been released. This release contains a few useful features and a number of other enhancements. It contains over 60 improvements, including the new features as listed below. If you are planning to upgrade the API from a previous release, we suggest you to check documents in the Public API Changes section.

## Save Charts in SVG Format

Aspose.Cells for .NET 8.3.0 provides support for exporting charts in Scalable Vector Graphics (SVG) format, an XML-based vector image format for two-dimensional graphics which supports interactivity and animation. Please refer to the following piece of code to see how it works and feel free to read the detailed article on saving charts to SVG.

```
//Create workbook object from source Excel file
Workbook workbook = new Workbook("source.xlsx");

//Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];

//Access the first chart inside the worksheet
Chart chart = worksheet.Charts[0];

//Save the chart into image in SVG format
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.SaveFormat = SaveFormat.SVG;
chart.ToImage("ChartImage.svg", options); 
```

## Get Equation Text of Chart Trendline

Aspose.Cells allows you to retrieve the equation text of a chart trendline. Aspose.Cells provides the Trendline.DataLabels.Text property which returns the equation text of a chart's trendline. To make use of this property, first call the Chart.Calculate() method. Please see the detailed article on retrieving the equation text of a chart trendline.

## Track Workbook State

Aspose.Cells for .NET 8.3.0 has added several properties that could enable the developers to track & manipulate the Workbook file's state. The aforesaid properties and their brief descriptions are as follow.

*   WorkbookSettings.CrashSave: Indicates whether the application last saved the workbook file after a crash.
*   WorkbookSettings.DataExtractLoad: Indicated whether the application last opened the workbook file for data recovery.
*   WorkbookSettings.RepairLoad: Provides information if the application last opened the workbook file in safe or repair mode.
*   WorkbookSettings.AutoRecover: Indicates if auto-recovery has been performed on the Workbook file.

## Other Enhancements and Fixes

In the new version, we have fixed a few exceptions that occurred while loading and opening Microsoft Excel file formats (XLS/XLSX, CSV, ODS etc.) and converting them to PDF format.

In this release, several important issues have been addressed. For example, issues around reading/ writing Microsoft Excel file formats (XLS, XLSX, XLSB, SpreadsheetML, ODS etc.), rendering to HTML format, printing spreadsheets, combining workbooks, manipulating shapes and rendering to XPS/PDF, manipulating conditional formatting, rendering images from Excel worksheets, manipulating charts with formatting, rendering images files from charts, creating and manipulating comments and exporting Excel workbooks to PDF format have been resolved. We have also fixed some issues regarding Aspose.Cells formula calculation engine to enhance it further.

We have also fixed a few issues in the web based Grid control by Aspose.Cells for .NET regarding TableItemStyle. We have fixed an out of memory issue while loading/saving an Excel file. We have added support for changing the position of a horizontal scrollbar with respect to the tab bar via code in the GridWeb control.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 8.3.0, please visit the [download page][2].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png "Aspose.Cells for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.cells-for-.net/entry586604.aspx




