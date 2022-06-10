---
title: 'Directly Render Chart to PDF, Get Notification while Processing Smart Markers and Remove Unused Styles from Workbook with Aspose.Cells for .NET 8.6.2'
date: Thu, 26 Nov 2015 10:21:55 +0000
draft: false
url: /2015/11/26/directly-render-chart-to-pdf-get-notification-while-processing-smart-markers-and-remove-unused-styles-from-workbook-with-aspose.cells-for-.net-8.6.2/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for .NET logo][1]](https://www.aspose.com/ "Aspose.Cells for .NET API")Aspose.Cells for .NET 8.6.2 has been released. This release contains many useful features and other enhancements along with critical bug fixes. We have improved our important Smart Markers feature to next level in this release.  If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you to check the complete Public API Changes section to know what has been changed in the API so far. We have provided some important features in this month’s release.

## Get Notification while Processing Smart Markers

Smart Markers are one of the advanced features offered by Aspose.Cells APIs to dynamically merge data with the help of specialized markers defined in a designer spreadsheet. Such spreadsheets can be considered as templates as they contain the formatting as well as the formulas along with the markers but no contents, where the data gets populated at runtime based on the marker definition and associated data source. Aspose.Cells APIs have provided the specialized WorkbookDesigner class that is used to load the designer spreadsheets and process them against the particular source to populate the data.

Recently we received requests in Aspose.Cells support forum to provide call back facility for the WorkbookDesigner class so that the process could emit notifications about the cell and/or smart marker being processed. With the release of Aspose.Cells for .NET 8.6.2, the API has exposed the ISmartMarkerCallBack interface along with the WorkbookDesigner.CallBack property to fulfill this requirement. The current implementation of ISmartMarkerCallBack interface allows to capture the references of worksheet, cell & smart marker being processed.

The following piece of code demonstrates the usage of ISmartMarkerCallBack interface to define a new class that handles the call back for WorkbookDesigner.Process method.

```
class SmartMarkerCallBack : ISmartMarkerCallBack
{
    Workbook workbook;
    internal SmartMarkerCallBack(Workbook workbook)
    {
        this.workbook = workbook;
    }
    public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
    {
        Console.WriteLine("Processing Cell : " + workbook.Worksheets[sheetIndex].Name + "!" + CellsHelper.CellIndexToName(rowIndex, colIndex));
        Console.WriteLine("Processing Marker : " + tableName + "." + columnName);
    }
} 
```

Rest of the process includes loading the designer spreadsheet containing the Smart Markers with an instance of WorkbookDesigner or creating a new designer spreadsheet from scratch and process it by setting the data source. However, in order to enable the notifications, it is necessary to set the WorkbookDesigner.CallBack property before calling the WorkbookDesigner.Process method as demonstrated below.

```
//Creating a DataTable that will serve as data source for designer spreadsheet
DataTable table = new DataTable("OppLineItems");
table.Columns.Add("PRODUCT_FAMILY");
table.Columns.Add("OPPORTUNITY_LINEITEM_PRODUCTNAME");
table.Rows.Add(new object[] { "MMM", "P1" });
table.Rows.Add(new object[] { "MMM", "P2" });
table.Rows.Add(new object[] { "DDD", "P1" });
table.Rows.Add(new object[] { "DDD", "P2" });
table.Rows.Add(new object[] { "AAA", "P1" });

//Loading the designer spreadsheet in an instance of Workbook
Workbook workbook = new Workbook(infileName);
//Loading the instance of Workbook in an instance of WorkbookDesigner
WorkbookDesigner designer = new WorkbookDesigner(workbook);
//Set the WorkbookDesigner.CallBack property to an instance of newly created class
designer.CallBack = new SmartMarkerCallBack(workbook);
//Set the data source 
designer.SetDataSource(table);
//Process the Smart Markers in the designer spreadsheet
designer.Process(false);
//Save the result
workbook.Save(outfileName); 
```

## Directly Render Chart to PDF

The Aspose.Cells for .NET 8.6.2 has introduced the Chart.ToPdf method in order to simplify the task of rendering charts in PDF format. Previous solution was to copy the required chart onto a new Worksheet then render the worksheet to PDF while specifying the area containing the chart shape. This solution was prone to error due to the number of statements to accomplish the same goal that can now be achieved in a single statement. The Chart.ToPdf method currently accepts a parameter of type string as file path location to store the resultant PDF directly onto the disk.

The following sample code explains the usage of Chart.ToPdf method to render a Chart in PDF format.

```
string filePath = @"F:\Downloads\source.xlsx";

//Load Excel file containing charts
Workbook workbook = new Workbook(filePath);

//Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];

//Access first chart inside the worksheet
Chart chart = worksheet.Charts[0];

//Save the chart into pdf format
chart.ToPdf("chart.pdf"); 
```

## Remove Unused Styles from Workbook's Style Pool

It is fairly possible that a spreadsheet may contain styles that are not in use. Such scenario may easily occur when user copies cells from another workbook because in this case some styles are copied too. Due to the reason that styles are shared for many objects such as cells, rows, columns and so on, when one cell's content (including style) is replaced by the copied one, the Aspose.Cells APIs do not remove the old style from the style pool. Imagine if the user does the copy operation repeatedly, there will be more and more styles in the style pool. Such unused styles can now be removed from the object of the Workbook while using the newly exposed RemoveUnusedStyles method. However, the aforementioned method could impose performance plenty because it has to check all objects to make sure that one style is not being used by any object, so we recommend to use this method with great caution.

Following is the simple usage scenario to remove unused styles.

```
//Load spreadsheet
Workbook workbook = new Workbook(inputFilePath);

//Remove all unused styles from the template
workbook.RemoveUnusedStyles(); 
```

## Other Enhancements & Fixes

The most notable enhancements in this release are as follow:

*   Exposed Cells.Style property that can be used to get/set the default style for a particular Worksheet.
*   Exposed two new events for the Aspose.Cells.GridWeb component, namely, AjaxCallFinished & CellModifiedOnAjax.
*   Provided support for generic List as nested objects in Smart Markers.

We have handled a few exceptions regarding reading/writing Excel file formats and rendering images in Sheet to Image conversions.

In this release, several important issues have been addressed. For example, issues around reading/ writing Microsoft Excel file formats, manipulating Pivot Tables, applying conditional formatting, rendering to HTML file format, formatting rows and columns, manipulating OLE Objects in the template files, setting data validation, manipulating and rendering shapes, applying Page Setup options, rendering images from Excel worksheets, manipulating charts, rendering images files from charts and exporting Excel workbooks to PDF format have been resolved. We have further improved the Aspose.Cells formula calculation engine and fixed some issues in this regard.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 8.6.2, please visit the [download page][2].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png "Aspose.Cells for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.cells-for-.net/entry670670.aspx




