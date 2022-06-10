---
title: 'Manipulate Document Properties Without Creating an Instance of Workbook, Assign Macros to Controls and Restrict the API to Generate Frame Scripts for HTML Conversion with Aspose.Cells for .NET 8.6.0'
date: Tue, 29 Sep 2015 18:42:59 +0000
draft: false
url: /2015/09/29/manipulate-document-properties-without-creating-an-instance-of-workbook-assign-macros-to-controls-and-restrict-the-api-to-generate-frame-scripts-for-html-conversion-with-aspose.cells-for-.net-8.6.0/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for .NET logo][1]](https://www.aspose.com/ "Aspose.Cells for .NET API")Aspose.Cells for .NET 8.6.0 has been released. This release contains some useful enhancements along with critical bug fixes. If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you to check the complete Public API Changes section to know what has been changed in the API so far. We have provided a few important features in this month’s release.

## Manipulate Document Properties with WorkbookMetadata

Aspose.Cells for .NET APIs have exposed the Aspose.Cells.Metadata.WorkbookMetadata class that is light weight as compared to Workbook class and allows to load the spreadsheet in order to manipulate the document properties in a simpler & more efficient way. In addition to the aforesaid class, the Aspose.Cells for .NET 8.6.0 has also exposed the MetadataOptions class and MetadataType enumeration that can be used to specify the type of properties to be updated.

Following code snippet demonstrates how to use the newly exposed WorkbookMetadata & MetadataOptions classes to add a custom property to the spreadsheet while using Aspose.Cells for .NET API.

```
// Open Workbook metadata
MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
WorkbookMetadata meta = new WorkbookMetadata("Sample1.xlsx", options);

// Set some properties
meta.CustomDocumentProperties.Add("test", "test");

// Save the metadata info
meta.Save("Sample2.xlsx"); 
```

## Assign Macros to Shapes

Aspose.Cells for .NET now provides the Shape.MarcoName property to assign the macros to any control in the spreadsheet. This property is useful in scenarios where application requirement is to add modules and assign them to the controls for user interaction.

The following sample code explains the usage of Shape.MarcoName property to assign a simple newly added module to a button's click event.

```
Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook();
Aspose.Cells.Worksheet sheet = workbook.Worksheets[0];

int moduleIdx = workbook.VbaProject.Modules.Add(sheet);
Aspose.Cells.Vba.VbaModule module = workbook.VbaProject.Modules[moduleIdx];
module.Codes =
    "Sub ShowMessage()" + "\r\n" +
    "    MsgBox \"Welcome to Aspose!\"" + "\r\n" +
    "End Sub";

Aspose.Cells.Drawing.Button button = sheet.Shapes.AddButton(2, 0, 2, 0, 28, 80);
button.Placement = Aspose.Cells.Drawing.PlacementType.FreeFloating;
button.Font.Name = "Tahoma";
button.Font.IsBold = true;
button.Font.Color = System.Drawing.Color.Blue;
button.Text = "Aspose";

button.MacroName = sheet.Name + ".ShowMessage";

workbook.Save("Output.xlsm"); 
```

## Disable the Generation of Frame & Document Property Scripts for HTML Conversion

Aspose.Cells for .NET 8.6.0 has exposed the HtmlSaveOptions.ExportFrameScriptsAndProperties property that can be used to control the generation of scripts such as Frames & Document Properties while exporting the spreadsheets in HTML format. The aforesaid boolean type property has the default value of true, that means; the resultant HTML will contain the scripts related to the frames as per standards of Excel application. Moreover, the resultant HTML code will contain the conditional comments that detects the browser type and handles the layout accordingly. However, setting this property to false will direct the Aspose.Cells APIs not to generate the frame scripts and conditional comments. In this case the resultant HTML can be viewed in any browser but it cannot be imported back while using Aspose.Cells APIs.

## Other Enhancements and Fixes

In the new version, we have also provided a few enhancements:

e.g

*   Exposed OoxmlSaveOptions.UpdateZoom property that can be used to update the PageSetup.Zoom if PageSetup.FitToPagesWide and/or PageSetup.FitToPagesTall properties have been used to control the Worksheet scaling.
*   Supported - you may use Aspose.Cells for .NET to run it in the Medium Trust environment.

We have handled some exceptions when reading/writing Excel spreadsheets, rendering Excel spreadsheets to PDF file format, refreshing Pivot tables and rendering Excel files to HTML file format.

In this release, several important issues have been addressed. For example, issues around reading/ writing Microsoft Excel file formats, manipulating Pivot Tables, copying ranges, embedding Ole objects, combining workbooks, manipulating shapes, applying PageSetup options, rendering images from Excel worksheets, manipulating charts, rendering images files from charts and exporting Excel workbooks to PDF format have been resolved. We have further improved the Aspose.Cells formula calculation engine and fixed a few issues in this regard.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 8.6.0, please visit the [download page][2].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png "Aspose.Cells for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.cells-for-.net/entry657337.aspx




