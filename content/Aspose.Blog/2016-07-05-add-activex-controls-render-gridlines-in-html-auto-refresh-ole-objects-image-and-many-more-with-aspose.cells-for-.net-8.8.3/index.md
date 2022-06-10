---
title: 'Add ActiveX Controls, Render GridLines in HTML, Auto Refresh OLE Object''s Image and many more with Aspose.Cells for .NET 8.8.3'
date: Tue, 05 Jul 2016 10:53:30 +0000
draft: false
url: /2016/07/05/add-activex-controls-render-gridlines-in-html-auto-refresh-ole-objects-image-and-many-more-with-aspose.cells-for-.net-8.8.3/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for .NET logo][1]](http://www.aspose.com/.net/excel-component.aspx "Aspose.Cells for .NET API")We are pleased to announce our next version of [Aspose.Cells for .NET v8.8.3][2]. This release includes many valuable features, other enhancements and critical bug fixes. It also improves the overall stability and usability of the APIs. Please see the release notes in order to know what is new and what has been changed/fixed with this version of Aspose.Cells for .NET. If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you to check the complete Public API Changes section to know what APIs are changed so far. We have highlighted some important features and other enhancements here.

## Support for ActiveX Controls

Aspose.Cells APIs have provided the ability to add & manipulate the ActiveX Controls in spreadsheets. Aspose.Cells for .NET API has exposed a number of useful classes, enumerations and methods to fully support the ActiveX Controls. The most worth mentioning addition to the public API is the ShapeCollection.AddActiveXControl method which allows to add an ActiveX Control to the collection of shapes by accepting 7 parameters to specify the control type, location to place the control and size of the control. The control type can be specified using the ControlType enumeration with following possible values.

*   ControlType.CheckBox
*   ControlType.ComboBox
*   ControlType.CommandButton
*   ControlType.Image
*   ControlType.Label
*   ControlType.ListBox
*   ControlType.RadioButton
*   ControlType.ScrollBar
*   ControlType.SpinButton
*   ControlType.TextBox
*   ControlType.ToggleButton
*   ControlType.Unknown

Below provided code snippet demonstrates the simple usage scenario of newly exposed ShapeCollection.AddActiveXControl method to add an ActiveX Control of type Toggle Button. Please check the detailed article on Adding ActiveX Controls to Worksheets if you wish to get more in-depth understanding of the aforementioned feature.

```
// Create an instance of Workbook
var book = new Workbook();

// Access first worksheet from the collection
var sheet = book.Worksheets[0];

// Add Toggle Button ActiveX Control to the ShapeCollection at specified location
var shape = sheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 4, 0, 4, 0, 100, 30);

// Access the ActiveX Control object and set its linked cell property
ActiveXControl control = shape.ActiveXControl;
control.LinkedCell = "A1";

// Save the result on disc
book.Save(dir + "output.xlsx", SaveFormat.Xlsx);
```

## Render Grid Lines to HTML

Aspose.Cells APIs provide the ability to export spreadsheet contents in HTML format as per the standards opted by Excel application. If a spreadsheet is converted to HTML using Excel application, it does not render the grid lines. Aspose.Cells APIs behave in the same way using its default settings, however, with this release of the API, the developers can now choose to render the grid lines as well. Aspose.Cells for Java API has exposed the HtmlSaveOptions.ExportGridLines property with default value of false. If the said property is set to true, the API renders the grid lines for the available data range in HTML format.

Below provided code snippet demonstrates the simple usage scenario of newly exposed HtmlSaveOptions.ExportGridLines to render the grid lines to HTML format. In order to get a more detailed understanding of this feature, please check the article on Rendering Grid Lines to HTML.

```
//Create a workbook
Workbook wb = new Workbook();

//Access first worksheet
Worksheet ws = wb.Worksheets[0];

//Fill worksheet with some integer values
for (int r = 0; r < 10; r++ )
{
    for(int c=0; c<10; c++)
    {
        ws.Cells[r, c].PutValue(r*1);
    }
}

//Save your workbook in HTML format and export gridlines
HtmlSaveOptions opts = new HtmlSaveOptions();
opts.ExportGridLines = true;
wb.Save("D:\\Downloads\\output.html", opts);
```

## Auto Refresh OleObject's Image

Aspose.Cells for .NET 8.8.3 has exposed the OleObject.AutoLoad property which allows to refresh the OleObject's image if the contents/data of the underlying object has been changed. The aforementioned property when set to true, forces the Excel application to refresh the OleObject's image when resultant spreadsheet is loaded in Excel interface.

Below provided code snippet demonstrates the simple usage scenario of newly exposed OleObject.AutoLoad property. In order to get a more detailed understanding of this feature, please check the article on Automatically Refresh OleObect's Image.

```
//Create workbook object from your sample excel file
Workbook wb = new Workbook("sample.xlsx");

//Access first worksheet
Worksheet sheet = wb.Worksheets[0];

//Set auto load property of first ole object to true
sheet.OleObjects[0].AutoLoad = true;

//Save the workbook in xlsx format
wb.Save("output.xlsx", SaveFormat.Xlsx);
```

## Add Comments for ListObjects

Aspose.Cells APIs now allow to get and set the comments for an instance of ListObject. In order to provide the aforementioned feature, the Aspose.Cells APIs have exposed the ListObject.Comment property with the release of 8.8.3.

Here is a simple usage scenario of newly exposed ListObject.Comment property. In order to get detailed understanding of this feature, please check the article on Adding Comments for ListObjects.

```
//Open the template file.
Workbook workbook = new Workbook("source.xlsx");

//Access first worksheet.
Worksheet worksheet = workbook.Worksheets[0];

//Access first list object or table.
ListObject lstObj = worksheet.ListObjects[0];

//Set the comment of the list object
lstObj.Comment = "This is Aspose.Cells comment.";

//Save the workbook in xlsx format
workbook.Save("output.xlsx", SaveFormat.Xlsx);
```

## Other Enhancements and Fixes

The most notable enhancements in this release are as follow:

*   Refresh & recalculate the Pivot Tables having calculated items.
*   Specify text spacing for shapes using ShapeFont.Spacing property.
*   Load spreadsheets without importing charts.
*   Support to parse inner DIV tags while importing HTML.
*   Hide & show legend entry's text.
*   Load spreadsheet with specific paper size.
*   Set line spacing & text alignment for paragraphs in shapes.
*   Specify the path where GridWeb stores temporary session files.
*   Using client side functions to select a range or to get the selected range in a GridWeb using JavaScript.
*   Copy and Paste Rows in GridDesktop within the Control and between the Control and Excel.

We have also handled a few exceptions regarding parsing and saving Excel and HTML files.

In this release, several important issues have been addressed. For example, issues around reading and writing Microsoft Excel file formats, manipulating shapes, copying Rows/Columns, manipulating PivotTables, converting spreadsheets to HTML files and vice versa, manipulating and rendering charts and shapes, rendering images from Excel worksheets, rendering images files from charts and exporting Excel workbooks to PDF format have been resolved.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][3].
*   [Aspose.Cells for .NET Download Section][4].
*   Aspose.Cells for .NET Documentation – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][5] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][6] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][7] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png "Aspose.Cells for .NET logo"
[2]: http://www.aspose.com/downloads/cells/net/new-releases/aspose.cells-for-.net-8.8.3/
[3]: http://www.aspose.com/.net/excel-component.aspx
[4]: http://www.aspose.com/downloads/cells/net
[5]: http://www.aspose.com/api/net/cells
[6]: https://forum.aspose.com/
[7]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




