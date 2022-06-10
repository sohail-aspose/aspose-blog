---
title: 'Render MS Excel Worksheet to Graphics Context using C#'
date: Mon, 24 Aug 2015 09:29:48 +0000
draft: false
url: /2015/08/24/render-ms-excel-worksheet-to-graphics-context-using-c/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


[Aspose.Cells for .NET][1] 8.5.2 has been released. This release contains some useful features and other enhancements along with important bug fixes. If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you to check the complete Public API Changes section to know what has been changed in the API so far. We have provided a few important features in this month’s release.

## Render Worksheet to Graphics Context in C#

Aspose.Cells for .NET APIs have exposed an overloaded version of SheetRender.ToImage method/overload that can accept an instance of System.Drawing.Graphics object along with usual parameters to render the Worksheet in Graphics context. This feature is helpful in scenario where you wish to get high (scalable) print quality by redirecting the Graphics context to PostScript printer and create a PDF from the PostScript.

Following code snippet demonstrates how to use the newly exposed SheetRender.ToImage method to render the Worksheet in Graphics context.

```
string filePath = @"F:\Downloads\source.xlsx";

//Create workbook object from source file
Workbook workbook = new Workbook(filePath);

//Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];

//Create empty Bitmap
Bitmap bmp = new Bitmap(800, 800);

//Create Graphics Context
Graphics g =Graphics.FromImage(bmp);
g.Clear(Color.Blue);

//Set one page per sheet to true in image or print options
ImageOrPrintOptions opts = new ImageOrPrintOptions();
opts.OnePagePerSheet = true;

//Render worksheet to graphics context
SheetRender sr = new SheetRender(worksheet, opts);
sr.ToImage(0, g, 0, 0);

//Save the graphics context image in Png format
bmp.Save("test.png", ImageFormat.Png); 
```

## Access Cell by PivotField Name in C#

Aspose.Cells for .NET now provides the PivotTable.GetCellByDisplayName method to obtain the Cell reference by PivotField display name. This method is useful in scenarios where application requirement is to format the PivotField header in the PivotTable.

The following sample code explains the usage of PivotTable.GetCellByDisplayName method to format the PivotField header.

```
string filePath = @"F:\Downloads\source.xlsx";

//Create workbook object from source excel file
Workbook workbook = new Workbook(filePath);

//Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];

//Access first pivot table inside the worksheet
PivotTable pivotTable = worksheet.PivotTables[0];

//Access cell by display name of 2nd data field of the pivot table
Cell cell = pivotTable.GetCellByDisplayName(pivotTable.DataFields[1].DisplayName);

//Access cell style and set its fill color and font color
Style style = cell.GetStyle();
style.ForegroundColor = Color.LightBlue;
style.Font.Color = Color.Black;

//Set the style of the cell
pivotTable.Format(cell.Row, cell.Column, style);

//Save workbook
workbook.Save("output.xlsx"); 
```

## Apply Consolidation Functions for the DataFields of PivotTable

Aspose.Cells APIs provide the means to apply Consolidation Function to DataFields (or value fields) of the PivotTable. In Microsoft Excel, you can right click the value field and then select Value Field Settings... option and then select the tab Summarize Values By. From there, you can select any Consolidation Function of your choice like Sum, Count, Average, Max, Min, Product, Distinct Count etc.

Aspose.Cells provides ConsolidationFunction enumeration to support the following consolidation functions.

The following code applies Average consolidation function to first DataField and DistinctCount consolidation function to second DataField of a sample PivotTable.

```
//Create workbook from source excel file
Workbook workbook = new Workbook("source.xlsx");

//Access the first worksheet of the workbook
Worksheet worksheet = workbook.Worksheets[0];

//Access the first pivot table of the worksheet
PivotTable pivotTable = worksheet.PivotTables[0];

//Apply Average consolidation function to first data field
pivotTable.DataFields[0].Function = ConsolidationFunction.Average;

//Apply DistinctCount consolidation function to second data field
pivotTable.DataFields[1].Function = ConsolidationFunction.DistinctCount;

//Calculate the data to make changes affect
pivotTable.CalculateData();

//Save the workbook
workbook.Save("output.xlsx");
```

## Change Shape's Adjustment Values

Aspose.Cells for .NET 8.5.2 has exposed the Geometry.ShapeAdjustValues attribute that can be used to make changes to the adjustment points within the shapes. Please note, Microsoft Excel application displays the adjustments points as yellow diamond nodes while allowing to change the arc for rounded rectangle, point location for triangle, top width of a trapezoid and shape of head & tail for arrows.

## Other Enhancements and Fixes

In the new version, we have also provided a few enhancements:

e.g

*   Exposed SaveOptions.MergeAreas property to handle scenarios if a spreadsheet has too many individual cells with validation applied, there are chances that the resultant spreadsheet may get corrupted. One possible solution is to merge the cells with identical validation rules or you can now use the SaveOptions.MergeAreas property to direct the API to auto merge the CellAreas before the save operation.
*   Supported Keyboard Shortcuts in the desktop based grid control provided by Aspose.Cells for .NET to allow users to select or navigate b/w cells in the worksheet.

We have handled some exceptions when reading/writing Excel spreadsheets, rendering and refreshing Pivot tables, rendering images from Charts and merging spreadsheets.

In this release, several important issues have been addressed. For example, issues around reading/ writing Microsoft Excel file formats, manipulating Pivot Tables, combining workbooks, applying PageSetup options, rendering MS Excel Slicers, manipulating drawing objects and shapes, rendering images from Excel worksheets, manipulating charts, rendering images files from charts and exporting Excel workbooks to PDF format have been resolved. We have enhanced the Aspose.Cells formula calculation engine further and fixed a few issues in this regard.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 8.5.2, please visit the [download page][2].




[1]: https://products.aspose.com/cells/net
[2]: https://downloads.aspose.com/cells/net




