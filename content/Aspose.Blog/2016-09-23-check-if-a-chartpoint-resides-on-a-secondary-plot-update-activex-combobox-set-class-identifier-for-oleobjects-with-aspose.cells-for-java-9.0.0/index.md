---
title: 'Check If a ChartPoint Resides on a Secondary Plot, Update ActiveX ComboBox &amp; Set Class Identifier for OleObjects with Aspose.Cells for Java 9.0.0'
date: Fri, 23 Sep 2016 09:50:40 +0000
draft: false
url: /2016/09/23/check-if-a-chartpoint-resides-on-a-secondary-plot-update-activex-combobox-set-class-identifier-for-oleobjects-with-aspose.cells-for-java-9.0.0/
author: Babar Raza
summary: ''
tags: ['ActiveX Control', 'Chart Point', 'Class Identifier', 'ComboBox', 'Embedded Objects', 'Excel APIs', 'Excel Charts', 'Java APIs', 'OleObjects', 'Spreadsheet Creation', 'Spreadsheet Manipulation']
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for Java][1]](http://www.aspose.com/java/excel-component.aspx "Aspose.Cells for Java - Excel Java APIs")We are pleased to announce the release of [Aspose.Cells for Java 9.0.0][2]. This release includes many new features and enhancements along with some critical bug fixes that further improve the overall stability of the API. Please check the detailed release notes in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Java. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the Public API Changes section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Check If a ChartPoint Resides on a Secondary Plot

Aspose.Cells for Java API has exposed the ChartPoint.isInSecondaryPlot property with this release. Boolean type property can be used to detect if a ChartPoint resides on secondary plot or not.

Here is a simple usage scenario of aforementioned property, whereas a detailed article can be viewed on Detecting if a ChartPoint Resides on Secondary Plot.

```
//Load an existing spreadsheet containing a Pie chart
Workbook book = new Workbook(dir + "sample.xlsx");

//Load the Worksheet at 0 index
Worksheet sheet = book.getWorksheets().get(0);

//Load the first chart from the collection
Chart chart = sheet.getCharts().get(0);

//Calculate the chart before accessing its properties
chart.calculate();

//Accessing chart's first series
Series series = chart.getNSeries().get(0);

//Loop over the ChartPoint collection
for(int p = 0 ; p < series.getPoints().getCount(); p++)
{
	ChartPoint point = series.getPoints().get(p);

	//Detect if ChartPoint resides on secondary plot
	System.out.println(point.isInSecondaryPlot());
}
```

## Update ActiveX ComboBox

The Aspose.Cells APIs can be used to insert and/or manipulate existing ActiveX controls. One such example in an ActiveX ComboBox which can now be created as well as manipulated with Aspose.Cells for Java APIs.

Please check the detailed article on Updating ActiveX ComboBox Control for more in-depth knowledge of this feature.

```
//Create an instance of Workbook from a sample spreadsheet
Workbook book = new Workbook(dir + "sample.xlsx");

//Access first shape from first worksheet
Shape shape = book.getWorksheets().get(0).getShapes().get(0);

//Access ActiveX ComboBox and update its value
if (shape.getActiveXControl() != null)
{
    //Access Shape ActiveX Control
    ActiveXControl c = shape.getActiveXControl();

    //Check if ActiveX Control is of type ComboBox
    if (c.getType() == ControlType.COMBO_BOX)
    {
        //Type cast ActiveXControl into ComboBoxActiveXControl and change its value
        ComboBoxActiveXControl comboBoxActiveX = (ComboBoxActiveXControl)c;
        comboBoxActiveX.setValue("This is combo box control.");
    }
}

//Save the result
book.save(dir + "output.xlsx");
```

## Set Class Identifier for OleObjects

Aspose.Cells for Java 9.0.0 has exposed the OleObject.ClassIdentifier property which can be used to retrieve or set the class identifier for an OleObject. Please note, the class identifier decides which application is required to load the embedded resource/OleObject and how. for instance, a PPT file can be embedded in a spreadsheet with 2 different views, that is; presentation view or slide view, whereas both views have different class identifier values.

Below provided code snippet demonstrates the simple usage scenario of newly exposed OleObject.ClassIdentifier property. In order to get more details of possible usage scenarios, please check the detailed article on Class Identifier for OleObjects.

```
//Load a spreadsheet containing a presentation as OleObject
Workbook book = new Workbook(dir + "sample.xls");

//Initialize variables to store properties of OleObject
int upperLeftRow = 0;
int upperLeftColumn = 0;
int height = 0;
int width = 0;
byte[] imageData = null;
int x = 0;
int y = 0;
byte[] objData = null;
String progID = "";
int fileFormatType = 0;
String sourceFullName = "";
Boolean isDisplayAsIcon = false;
byte[] classId = null;

//Get the first worksheet from the collection
Worksheet sheet = book.getWorksheets().get(0);

//Get the first OleObject from the collection
OleObject frame = sheet.getOleObjects().get(0);

//Store the properties in variables
upperLeftRow = frame.getUpperLeftRow();
upperLeftColumn = frame.getUpperLeftColumn();
height = frame.getHeight();
width = frame.getWidth();
imageData = frame.getImageData();
x = frame.getX();
y = frame.getY();
objData = frame.getObjectData();
progID = frame.getProgID();
fileFormatType = frame.getFileFormatType();
sourceFullName = frame.getObjectSourceFullName();
isDisplayAsIcon = frame.getDisplayAsIcon();
classId = frame.getClassIdentifier();

//Initialize a new Workbook instance
book = new Workbook();

//Access first worksheet from the collection
sheet = book.getWorksheets().get(0);

//Insert the OleObject to the worksheet
int oleNumber = sheet.getOleObjects().add(upperLeftRow, upperLeftColumn, height, width, imageData);

//Access newly inserted OleObject
OleObject embeddedObject = sheet.getOleObjects().get(oleNumber);

//Assign previously stored properties to new OleObject
embeddedObject.setX(x);
embeddedObject.setY(y);
embeddedObject.setObjectData(objData);
embeddedObject.setProgID(progID);
embeddedObject.setFileFormatType(fileFormatType);
embeddedObject.setDisplayAsIcon(isDisplayAsIcon);
embeddedObject.setObjectSourceFullName(sourceFullName);
embeddedObject.setAutoSize(false);
if (classId != null)
{
	embeddedObject.setClassIdentifier(classId);
} 
```

## Control the Appearance of Shape's Textual Contents

Aspose.Cells for Java API has exposed the Shape.TextOptions property which can be used to control all aspects of the shape's textual contents such as font style, color, font weight and so on.

Below provided code snippet demonstrates the simple usage scenario of Shape.TextOptions property.

```
//Initialize an instance of Workbook
Workbook book = new Workbook();

//Get the default Worksheet from the Workbook
Worksheet sheet = book.getWorksheets().get(0);

//Add a TextBox to the collection
int textboxIndex = sheet.getTextBoxes().add(2, 1, 160, 200);

//Get the TextBox object
TextBox textbox = sheet.getTextBoxes().get(textboxIndex);

//Add text to the TextBox
textbox.setText("Hello Aspose!");

//Format the textual contents
textbox.getTextOptions().setColor(Color.getRed());
textbox.getTextOptions().setItalic(true);
textbox.getTextOptions().setBold(true);
```

## Other Enhancements & Fixes

Aspose.Cells for Java 9.0.0 has fixed a few critical bugs as well as enhanced its core for more stability. A few of the worth mentioning enhancements are as follow.

*   Enhanced the Aspose.Cells' Calculation Engine for performance considerations.
*   Improved HTML import engine for cell borders as well as cell text alignment.
*   Handled a few exceptions such as NullPointerException, NegativeArraySizeException & ArrayIndexOutOfBoundsException for certain scenarios.

## Public API Changes

Aspose.Cells for Java 9.0.0 has made a few changes to the publicly exposed APIs in order to keep the API usage simple. Some of the changes are listed as follow.

*   The Worksheet.SetBackground method has been marked obsoleted whereas the alternative approach has been exposed via Worksheet.BackgroundImage property.
*   A few methods such as Worksheet.CopyConditionalFormatting & Workbook.CheckWriteProtectedPassword were obsoleted some releases back. Now they have been completely removed from the public API.
*   The Workbook.RemoveDigitallySign method has been renamed to Workbook.RemoveDigitalSignature.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][3].
*   [Aspose.Cells for Java Download Section][4].
*   Aspose.Cells for Java Documentation – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][5] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][6] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][7] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Java Examples][8] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Cells-for-Java_100.png "Aspose.Cells for Java"
[2]: http://www.aspose.com/downloads/cells/java/new-releases/aspose.cells-for-java-9.0.0/
[3]: http://www.aspose.com/java/excel-component.aspx
[4]: http://www.aspose.com/community/files/72/java-components/aspose.cells-for-java/default.aspx
[5]: http://www.aspose.com/api/java/cells/com.aspose.cells/index
[6]: https://forum.aspose.com/
[7]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/
[8]: https://github.com/asposecells/Aspose_Cells_Java




