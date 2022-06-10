---
title: 'Support for ActiveX Controls, Render Grid Lines in HTML, Auto Refresh OleObject''s Image and much more with Aspose.Cells for Java 8.8.3'
date: Tue, 05 Jul 2016 11:20:07 +0000
draft: false
url: /2016/07/05/support-for-activex-controls-render-grid-lines-in-html-auto-refresh-oleobjects-image-and-much-more-with-aspose.cells-for-java-8.8.3/
author: Babar Raza
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for Java][1]](http://www.aspose.com/java/excel-component.aspx "Aspose.Cells for Java - Excel Java APIs")We are pleased to announce the release of [Aspose.Cells for Java 8.8.3][2]. This release includes many new features and enhancements along with some critical bug fixes that further improve the overall stability and usability of the API. Please check the detailed release notes in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Java. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the Public API Changes section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Support for ActiveX Controls

Aspose.Cells APIs have provided the ability to add & manipulate the ActiveX Controls in spreadsheets. Aspose.Cells for Java API has exposed a number of useful classes, enumerations and methods to fully support the ActiveX Controls. The most worth mentioning addition to the public API is the ShapeCollection.addActiveXControl method which allows to add an ActiveX Control to the collection of shapes by accepting 7 parameters to specify the control type, location to place the control and size of the control. The control type can be specified using the ControlType enumeration with following possible values.

*   ControlType.CHECK\_BOX
*   ControlType.COMBO\_BOX
*   ControlType.COMMAND\_BUTTON
*   ControlType.IMAGE
*   ControlType.LABEL
*   ControlType.LIST\_BOX
*   ControlType.RADIO\_BUTTON
*   ControlType.SCROLL\_BAR
*   ControlType.SPIN\_BUTTON
*   ControlType.TEXT\_BOX
*   ControlType.TOGGLE\_BUTTON
*   ControlType.UNKNOWN

Below provided code snippet demonstrates the simple usage scenario of newly exposed ShapeCollection.addActiveXControl method to add an ActiveX Control of type Toggle Button. Please check the detailed article on Adding ActiveX Controls to Worksheets if you wish to get more in-depth understanding of the aforementioned feature.

```
//Create an instance of Workbook
Workbook book = new Workbook();

//Access first worksheet from the collection
Worksheet sheet = book.getWorksheets().get(0);

//Add Toggle Button ActiveX Control to the ShapeCollection at specified location
Shape shape = sheet.getShapes().addActiveXControl(ControlType.TOGGLE_BUTTON, 4, 0, 4, 0, 100, 30);

//Access the ActiveX Control object and set its linked cell property
ActiveXControl control = shape.getActiveXControl();
control.setLinkedCell("A1");

//Save the result on disc
book.save(dir + "output.xlsx", SaveFormat.XLSX);
```

## Render Grid Lines to HTML

Aspose.Cells APIs provide the ability to export spreadsheet contents in HTML format as per the standards opted by Excel application. If a spreadsheet is converted to HTML using Excel application, it does not render the grid lines. Aspose.Cells APIs behave in the same way using its default settings, however, with this release of the API, the developers can now choose to render the grid lines as well. Aspose.Cells for Java API has exposed the HtmlSaveOptions.ExportGridLines property with default value of false. If the said property is set to true, the API renders the grid lines for the available data range in HTML format.

Below provided code snippet demonstrates the simple usage scenario of newly exposed HtmlSaveOptions.ExportGridLines to render the grid lines to HTML format. In order to get a more detailed understanding of this feature, please check the article on Rendering Grid Lines to HTML.

```
//Create an instance of Workbook and load existing spreadsheet
Workbook book = new Workbook(dir + "input.xlsx");

//Create an instance of HtmlSaveOptions
HtmlSaveOptions options = new HtmlSaveOptions();
//Set ExportGridLines to true
options.setExportGridLines(true);

//Save the result in HTML format
book.save(dir + "output.html", options);
```

## Auto Refresh OleObject's Image

Aspose.Cells for Java 8.8.3 has exposed the OleObject.AutoLoad property which allows to refresh the OleObject's image if the contents/data of the underlying object has been changed. The aforementioned property when set to true, forces the Excel application to refresh the OleObject's image when resultant spreadsheet is loaded in Excel interface.

Below provided code snippet demonstrates the simple usage scenario of newly exposed OleObject.AutoLoad property. In order to get a more detailed understanding of this feature, please check the article on Automatically Refresh OleObect's Image.

```
//Create an instance of Workbook and load an existing spreadsheet
Workbook book = new Workbook(dir + "input.xlsx");

//Access first worksheet from the collection
Worksheet sheet = book.getWorksheets().get(0);

//Access OleObjectCollection from first worksheet
OleObjectCollection oleObjects = sheet.getOleObjects();

//Access a OleObject from the collection
OleObject oleObject = oleObjects.get(0);

//Set AutoLoad to true
oleObject.setAutoLoad(true);
```

## Add Comments for ListObjects

Aspose.Cells APIs now allow to get and set the comments for an instance of ListObject. In order to provide the aforementioned feature, the Aspose.Cells APIs have exposed the ListObject.Comment property with the release of 8.8.3.

Here is a simple usage scenario of newly exposed ListObject.Comment property. In order to get detailed understanding of this feature, please check the article on Adding Comments for ListObjects.

```
//Create an instance of Workbook and load existing spreadsheet
Workbook book = new Workbook(dir + "input.xlsx");

//Access first worksheet from the collection
Worksheet sheet = book.getWorksheets().get(0);

//Access first ListObject from the collection of ListObjects
ListObject listObject = sheet.getListObjects().get(0);

//Set comments for the ListObject
listObject.setComment("Comments");

//Save the result on disc
book.save(dir + "output.xlsx");
```

## Other Enhancements & Improvements

The most notable enhancements in this release are as follow:

*   Refresh & recalculate the Pivot Tables having calculated items.
*   Specify text spacing for shapes using ShapeFont.Spacing property.
*   Load spreadsheets without importing charts.
*   Support to parse inner DIV tags while importing HTML.
*   Hide & show legend entry's text.
*   Load spreadsheet with specific paper size.
*   Set line spacing & text alignment for paragraphs in shapes.

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
[2]: http://www.aspose.com/downloads/cells/java/new-releases/aspose.cells-for-java-8.8.3/
[3]: http://www.aspose.com/java/excel-component.aspx
[4]: http://www.aspose.com/community/files/72/java-components/aspose.cells-for-java/default.aspx
[5]: http://www.aspose.com/api/java/cells/com.aspose.cells/index
[6]: https://forum.aspose.com/
[7]: https://blog.aspose.com/
[8]: https://github.com/asposecells/Aspose_Cells_Java




