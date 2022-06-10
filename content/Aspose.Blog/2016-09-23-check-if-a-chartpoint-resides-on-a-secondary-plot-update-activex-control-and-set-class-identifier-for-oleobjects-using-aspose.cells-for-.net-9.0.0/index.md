---
title: 'Check if a ChartPoint Resides on a Secondary Plot, Update ActiveX Control and Set Class Identifier for OleObjects using Aspose.Cells for .NET 9.0.0'
date: Fri, 23 Sep 2016 09:26:49 +0000
draft: false
url: /2016/09/23/check-if-a-chartpoint-resides-on-a-secondary-plot-update-activex-control-and-set-class-identifier-for-oleobjects-using-aspose.cells-for-.net-9.0.0/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for .NET logo][1]](http://www.aspose.com/.net/excel-component.aspx "Aspose.Cells for .NET API")We are pleased to announce our next version of [Aspose.Cells for .NET v9.0.0][2]. This release includes some new features and other enhancements with critical bug fixes. Please see the release notes in order to know what is new and what has been changed/fixed with this version of Aspose.Cells for .NET. If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you to check the complete Public API Changes section to know what APIs are changed so far. We have highlighted some important features and other enhancements here.

## Check If a ChartPoint Resides on a Secondary Plot

Aspose.Cells for .NET API has exposed the ChartPoint.IsInSecondaryPlot property with this release. Boolean type property can be used to detect if a ChartPoint resides on secondary plot or not.

Here is a simple usage scenario of aforementioned property, whereas a detailed article can be viewed on Detecting if a ChartPoint Resides on Secondary Plot.

```
// Load an existing spreadsheet containing a Pie chart
var book = new Workbook(dir + "PieBar.xlsx");

// Load the Worksheet at 0 index
var sheet = book.Worksheets[0];

// Load the first chart from the collection
var chart = sheet.Charts[0];

// Calculate the chart before accessing its properties
chart.Calculate();

// Accessing chart's first series
var series = chart.NSeries[0];

// Loop over the ChartPoint collection
foreach (ChartPoint point in series.Points)
{
    // Detect if ChartPoint resides on secondary plot
    Console.WriteLine(point.IsInSecondaryPlot);
}
```

## Update ActiveX ComboBox

The Aspose.Cells APIs can be used to insert and/or manipulate existing ActiveX controls. One such example in an ActiveX ComboBox which can now be created as well as manipulated with Aspose.Cells for .NET APIs.

Please check the detailed article on Updating ActiveX ComboBox Control for more in-depth knowledge of this feature.

```
//Create a workbook
Workbook wb = new Workbook("sample.xlsx");

//Access first shape from first worksheet
Shape shape = wb.Worksheets[0].Shapes[0];

//Access ActiveX ComboBox Control and update its value
if (shape.ActiveXControl != null)
{
    //Access Shape ActiveX Control
    ActiveXControl c = shape.ActiveXControl;

    //Check if ActiveX Control is ComboBox Control
    if (c.Type == ControlType.ComboBox)
    {
        //Type cast ActiveXControl into ComboBoxActiveXControl and change its value
        ComboBoxActiveXControl comboBoxActiveX = (ComboBoxActiveXControl)c;
        comboBoxActiveX.Value = "This is combo box control.";
    }
}

//Save the workbook
wb.Save("output.xlsx");
```

## Set Class Identifier for OleObjects

Aspose.Cells for .NET 9.0.0 has exposed the OleObject.ClassIdentifier property which can be used to retrieve or set the class identifier for an OleObject. Please note, the class identifier decides which application is required to load the embedded resource/OleObject and how. for instance, a PPT file can be embedded in a spreadsheet with 2 different views, that is; presentation view or slide view, whereas both views have different class identifier values.

Below provided code snippet demonstrates the simple usage scenario of newly exposed OleObject.ClassIdentifier property. In order to get more details of possible usage scenarios, please check the detailed article on Class Identifier for OleObjects.

```
// Load a spreadsheet containing a presentation as OleObject
var book = new Workbook(dir + "embeddedPresentation.xls");

// Initialize variables to store properties of OleObject
int upperLeftRow = 0;
int upperLeftColumn = 0;
int height = 0;
int width = 0;
byte[] imageData = null;
int x = 0;
int y = 0;
byte[] objData = null;
string progID = "";
FileFormatType fileFormatType = FileFormatType.Unknown;
string sourceFullName = "";
bool isDisplayAsIcon = false;
byte[] classId = null;

// Get the first worksheet from the collection
var sheet = book.Worksheets[0];

// Get the first OleObject from the collection
var frame = sheet.OleObjects[0];

// Store the properties in variables
upperLeftRow = frame.UpperLeftRow;
upperLeftColumn = frame.UpperLeftColumn;
height = frame.Height;
width = frame.Width;
imageData = frame.ImageData;
x = frame.X;
y = frame.Y;
objData = frame.ObjectData;
progID = frame.ProgID;
fileFormatType = frame.FileFormatType;
sourceFullName = frame.ObjectSourceFullName;
isDisplayAsIcon = frame.DisplayAsIcon;
classId = frame.ClassIdentifier;

// Initialize a new Workbook instance
book = new Workbook();

// Access first worksheet from the collection
sheet = book.Worksheets[0];

// Insert the OleObject to the worksheet
int oleNumber = sheet.OleObjects.Add(upperLeftRow, upperLeftColumn, height, width, imageData);

// Access newly inserted OleObject
var embeddedObject = sheet.OleObjects[oleNumber];

// Assign previously stored properties to new OleObject
embeddedObject.X = x;
embeddedObject.Y = y;
embeddedObject.ObjectData = objData;
embeddedObject.ProgID = progID;
embeddedObject.FileFormatType = fileFormatType;
embeddedObject.DisplayAsIcon = isDisplayAsIcon;
embeddedObject.ObjectSourceFullName = sourceFullName;
embeddedObject.IsAutoSize = false;
if (classId != null)
{
    embeddedObject.ClassIdentifier = classId;
}

// Save the resultant spreadsheet
book.Save(dir  + "output.xls"); 
```

## Control the Appearance of Shape's Textual Contents

Aspose.Cells for .NET API has exposed the Shape.TextOptions property which can be used to control all aspects of the shape's textual contents such as font style, color, font weight and so on.

Below provided code snippet demonstrates the simple usage scenario of Shape.TextOptions property.

```
// Initialize an instance of Workbook
var book = new Workbook();

// Get the default Worksheet from the Workbook
var sheet = book.Worksheets[0];

// Add a TextBox to the collection
var textboxIndex = sheet.TextBoxes.Add(2, 1, 160, 200);

// Get the TextBox object
var textbox = sheet.TextBoxes[textboxIndex];

// Add text to the TextBox
textbox.Text = "Hello Aspose!";

// Format the textual contents
textbox.TextOptions.Color = System.Drawing.Color.Red;
textbox.TextOptions.IsItalic = true;
```

## Other Enhancements and Fixes

Aspose.Cells for .NET 9.0.0 has fixed a few critical bugs as well as enhanced its core for more stability. A few of the worth mentioning enhancements are as follow.

*   Load the Workbook with specific System Culture Info.
*   Use Aspose.Cells.GridDesktop control in WPF Application.
*   Enhanced the Aspose.Cells' Calculation Engine for performance considerations.
*   Improved HTML import engine for cell borders as well as cell text alignment.
*   Handled a few exceptions such as NullPointerException and "Invalid text of the defined name." for certain scenarios.

In this release, several important issues have been addressed. For example, issues around reading and writing Microsoft Excel file formats, rendering to HTML file format, rendering images from Excel worksheets, rendering images files from charts and exporting Excel workbooks to PDF format have been resolved.

## Public API Changes

Aspose.Cells for .NET 9.0.0 has made a few changes to the publicly exposed APIs in order to keep the API usage simple. Some of the changes are listed as follow.

*   The Worksheet.SetBackground method has been marked obsoleted whereas the alternative approach has been exposed via Worksheet.BackgroundImage property.
*   A few methods such as Worksheet.CopyConditionalFormatting & Workbook.CheckWriteProtectedPassword were obsoleted some releases back. Now they have been completely removed from the public API.
*   The Workbook.RemoveDigitallySign method has been renamed to Workbook.RemoveDigitalSignature.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][3].
*   [Aspose.Cells for .NET Download Section][4].
*   Aspose.Cells for .NET Documentation – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][5] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][6] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][7] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png "Aspose.Cells for .NET logo"
[2]: http://www.aspose.com/downloads/cells/net/new-releases/aspose.cells-for-.net-9.0.0/
[3]: http://www.aspose.com/.net/excel-component.aspx
[4]: http://www.aspose.com/downloads/cells/net
[5]: http://www.aspose.com/api/net/cells
[6]: https://forum.aspose.com/
[7]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




