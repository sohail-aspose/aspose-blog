---
title: 'Set Link Target Type for HTML Conversion, Ignore Hidden Columns while Exporting Worksheet Data to DataTable and Detect If VbaProject is Signed with Aspose.Cells for .NET 8.6.1'
date: Mon, 02 Nov 2015 08:43:17 +0000
draft: false
url: /2015/11/02/set-link-target-type-for-html-conversion-ignore-hidden-columns-while-exporting-worksheet-data-to-datatable-and-detect-if-vbaproject-is-signed-with-aspose.cells-for-.net-8.6.1-2/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for .NET logo][1]](https://www.aspose.com/ "Aspose.Cells for .NET API")Aspose.Cells for .NET 8.6.1 has been released. This release contains some useful features and other enhancements along with critical bug fixes. If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you to check the complete Public API Changes section to know what has been changed in the API so far. We have provided a few important features in this month’s release.

## Set Link Target Type for HTML Conversion

Aspose.Cells APIs are capable of converting all supported spreadsheet formats to HTML with highest fidelity. The conversion process is efficient as well as configurable, i.e., users can customize the HTML generation process as per their application requirement. Aspose.Cells APIs have exposed the HtmlSaveOptions class that is mainly responsible for the conversion process and provides a vast array of features to influence the HTML generation.

This release of Aspose.Cells for Java API has exposed an enumeration namely HtmlLinkTargetType along with a new property HtmlSaveOptions.LinkTargetType that together allows to set the target type for the links in spreadsheet while conversion to HTML format. The possible values of the HtmlLinkTargetType enumeration are as follow where the default value is Self.

*   HtmlLinkTargetType.Blank: Opens the linked document/page in a new window or tab.
*   HtmlLinkTargetType.Parent: Opens the linked document/page in parent frame.
*   HtmlLinkTargetType.Self: Opens the linked document/page in the same frame where the link was clinked.
*   HtmlLinkTargetType.Top: Opens the linked document/page in the full body of the window.

Here is the simplest usage scenario of newly exposed APIs to set the link target type.

```
//Load a spreadsheet
Workbook workbook = new Workbook(inputFilePath);

HtmlSaveOptions opts = new HtmlSaveOptions();
opts.LinkTargetType = HtmlLinkTargetType.Self;

//Convert the spreadsheet to HTML with preset HtmlSaveOptions
workbook.Save(outputFilePath, options); 
```

## Ignore Hidden Columns while Exporting Worksheet Data to DataTable

Aspose.Cells for .NET 8.6.1 allows you to just ignore hidden columns while exporting worksheet data to data table. You can achieve it using Aspose.Cells by setting the ExportTableOptions.PlotVisibleColumns to true. By default, its value is false, so you need to set it true to ignore the hidden columns while exporting the data.

## Access & Update Portion of Rich Text

Aspose.Cells for .NET API provides easy to use mechanism to access the format related properties of each character from a cell containing Rich Text. The API has exposed the GetCharacters & SetCharacters methods for the Cell class that allows to access & update the portion of the Rich Text in a cell. The Cell.GetCharacters method returns an array of FontSetting objects where each object represents the styling of an individual character. The Cell.SetCharacters method also accepts an array of FontSetting objects to set the styling for individual characters of a cell.

The following sample code explains the usage of Cell.GetCharacters & Cell.SetCharacters methods to access and manipulate the styling of Rich Text.

```
//Load a spreadsheet
Workbook workbook = new Workbook(inputFilePath);
//Access first worksheet of the workbook
Worksheet worksheet = workbook.Worksheets[0];
//Access the cells containing the Rich Text
Cell cell = worksheet.Cells["A1"];

//Retrieve the array of FontSetting from the cell
FontSetting[] settings = cell.GetCharacters();

//Modify the Font Name for the first FontSetting 
settings[0].Font.Name = "Arial";

//Set the updated FontSetting
cell.SetCharacters(settings); 
```

## Detect If VbaProject is Signed

Aspose.Cells for .NET 8.6.1 has exposed the the VbaProject.IsSigned Boolean property that can be used to test if a VbaProject in a Workbook is signed or not. The Boolean type property returns true if the project is signed.

Following is the simple usage scenario.

```
//Load a spreadsheet
Workbook workbook = new Workbook(inputFilePath);

//Retrieve the VbaProject from the Workbook
VbaProject project = workbook.VbaProject;

//Test if VbaProject is signed
if (project.IsSigned)
{
    Console.WriteLine("VBA Project is Signed");
}
else
{
    Console.WriteLine("VBA Project is not Signed");
} 
```

## Other Enhancements and Fixes

In the new version, we have also provided some other enhancements:

e.g

*   Exposed RangeCollection.Add method that can be used to add Range objects to the collection of ranges for a particular Worksheet.
*   Exposed an overload of the VbaModuleCollection.Remove method that can now accept an instance of Worksheet to remove all the VBA modules associated with the specified Worksheet.
*   Modified Cell.GetFormatConditions method that now returns an array of type FormatConditionCollection.
*   Provided support for WebQuery type of external data source.
*   Add reference to VBA macros project in the workbook.
*   Provided support to load and save SpreasheetML(XML) file in GridDesktop control.

We have handled some exceptions when reading/writing Excel file formats and rendering shapes in Excel to PDF conversions.

In this release, several important issues have been addressed. For example, issues around reading/ writing Microsoft Excel file formats, encrypting Excel spreadsheets, protecting worksheets in the workbook, accessing document properties and Smart Markers, manipulating named ranges, manipulating and rendering shapes, applying PageSetup options, rendering images from Excel worksheets, manipulating charts, rendering images files from charts and exporting Excel workbooks to PDF format have been resolved. We have further improved the Aspose.Cells formula calculation engine and fixed a few issues in this regard.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 8.6.1, please visit the [download page][2].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png "Aspose.Cells for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.cells-for-.net/entry664883.aspx




