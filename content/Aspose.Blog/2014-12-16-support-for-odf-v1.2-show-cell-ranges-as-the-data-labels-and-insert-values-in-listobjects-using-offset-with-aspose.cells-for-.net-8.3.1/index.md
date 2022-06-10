---
title: 'Support for ODF 1.2, Show Cell Ranges as Data Labels and Insert Values in ListObjects using Offset with Aspose.Cells for .NET 8.3.1'
date: Tue, 16 Dec 2014 09:31:02 +0000
draft: false
url: /2014/12/16/support-for-odf-v1.2-show-cell-ranges-as-the-data-labels-and-insert-values-in-listobjects-using-offset-with-aspose.cells-for-.net-8.3.1/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for .NET logo][1]](https://www.aspose.com/ "Aspose.Cells for .NET API")Aspose.Cells for .NET 8.3.1 has been released. This release contains a few useful features and a number of other enhancements. It contains over 40 improvements, including the new features listed below. It also includes the long awaited support for ODF 1.2 specifications. If you are planning to upgrade the API from a previous release, we suggest you to check documents in the Public API Changes section.

## Save ODS file in ODF 1.1 and 1.2 Specifications

The Aspose.Cells APIs have extended support for the OpenDocument format. Now it is possible to save the ODS (OpenDocument Spreadsheets) in conformance with the ODF 1.2 specifications. The Aspose.Cells APIs have exposed the methods IsStrictSchema11 for the OdsSaveOptions class to allow developers to save spreadsheets in ODS format conforming to ODF 1.2 specification. The default value of IsStrictSchema11 property is false, and means that from version 8.3.1 of the Aspose.Cells APIs, the ODS files will be saved as ODF format version 1.2 by default. For more details, please check the article Save ODS file in ODF 1.1 and 1.2 Specifications.

## Insert Values in ListObjects using Row/Column Offset

Normally, you add values inside the ListObject/Table using the Cell.PutValue method, however, the PutValue method must be associated with an instance of a cell to identify the location the value should be inserted at. This mechanism can't be sued when you need to add values inside the ListObject using the row and column offsets. Aspose.Cells for .NET 8.3.1 has exposed the Cell.GetTable and ListObject.PutCellValue methods to allow you to access the ListObject from a cell and add values using row and column offsets.

The following sample code loads the source spreadsheet, and adds values inside the table.

```
//Create workbook from source Excel file
Workbook workbook = new Workbook("source.xlsx");

//Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];

//Access cell D5 which lies inside the table
Cell cell = worksheet.Cells["D5"];

//Put value inside the cell D5
cell.PutValue("D5 Data");

//Access the Table from this cell
ListObject table = cell.GetTable();

//Add some value using Row and Column Offset
table.PutCellValue(2, 2, "Offset [2,2]");

//Save the workbook
workbook.Save("output.xlsx"); 
```

## Show Cell Ranges as Data Labels

Aspose.Cells provides the DataLabels.ShowCellRange property to select or clear the option **Label Contains - Value From Cells**. For more details, please see the article Showing Cell Range as the Data Labels.

## Create Sparkline by Specifying Data Range and Location

Aspose.Cells APIs have exposed the SparklineCollection.Add(String dataRange, int row, int column) method to specify the data range and location of the sparkline group.

You may achieve the same as discussed above while using the following code snippet.

```
//Create workbook from source Excel file
Workbook workbook = new Workbook("source.xlsx");

//Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];

//Access the first sparkline group
SparklineGroup group = worksheet.SparklineGroupCollection[0];

//Add Data Ranges and Locations inside this sparkline group
group.SparklineCollection.Add("D5:O5", 4, 15);
group.SparklineCollection.Add("D6:O6", 5, 15);
group.SparklineCollection.Add("D7:O7", 6, 15);
group.SparklineCollection.Add("D8:O8", 7, 15);

//Save the workbook
workbook.Save("output.xlsx"); 
```

## Other Enhancements and Fixes

In the new version, we have also provided the following new enhancements:

*   Specify a prefix for image URLs in CSS and HTML files.
*   Get/set Cell background color in Cell.HtmlString attribute.
*   Retrieve Cell.DisplayStringValue with conditional formatting.

We have fixed a few exceptions that occurred while loading and opening Microsoft Excel file formats. We have also fixed the exceptions that occurred in manipulating shapes, rendering sheets, calculating formulas and manipulating pivot tables. We have also improved the performance when loading Microsoft Excel files.

In this release, several important issues have been addressed. For example, issues around reading/writing Microsoft Excel file formats, printing spreadsheets, rendering HTML file format, manipulating OLE Objects, copying worksheets, manipulating shapes, manipulating rows and columns, rendering images from Excel worksheets, manipulating charts with formatting, rendering images files from charts and exporting Excel workbooks to PDF format have been resolved. We have also fixed some issues regarding the Aspose.Cells formula calculation engine to enhance it.

We have also fixed a few issues in the web based Grid control by Aspose.Cells for .NET while loading/saving an Excel file.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 8.3.1, please visit the [download page][2].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png "Aspose.Cells for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.cells-for-.net/entry592614.aspx




