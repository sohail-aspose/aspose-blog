---
title: 'Modify SQL Database Connection Settings, Apply Rich Text to Custom Data Label of Chart Point, Render Comments and Set Desired Image Dimensions with Aspose.Cells for .NET 8.4.1'
date: Tue, 21 Apr 2015 12:52:47 +0000
draft: false
url: /2015/04/21/modify-sql-database-connection-settings-apply-rich-text-to-custom-data-label-of-chart-point-render-comments-and-set-desired-image-dimensions-with-aspose.cells-for-.net-8.4.1/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for .NET logo][1]](https://www.aspose.com/ "Aspose.Cells for .NET API")Aspose.Cells for .NET 8.4.1 has been released. This release contains many useful features, fixes and other enhancements. If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you to check the complete Public API Changes section to know what has been changed in the API so far. We have provided a few of the worth mentioning features in this month’s release.

## Modify SQL Database Connection Settings

Microsoft Excel application allows to create the database connection so that the data could be bound/ fetched and loaded in the spreadsheets to refresh Pivot Tables, Charts or just the worksheet. The external data source is connected to the workbook through a data connection, which is a set of information that describes how to locate, log in, query, and access the external data source.

Aspose.Cells for .NET API does not allow to create a database connection yet, however, some revisions back, the API had exposed the ExternalConnection class that contains the method & properties that could be used to review the database connection details stored in a spreadsheet. Most of the properties associated with ExternalConnection class were read-only until the release of Aspose.Cells for .NET 8.4.1. With this release, the API has provided the support to manipulate the database connection settings. Please check the detailed article on Modify Existing Database Connection Settings.

## Set Desired Image Dimensions for Spreadsheet & Chart Export

Another worth mentioning feature is the support for setting desired image dimensions while exporting spreadsheets & charts to image formats. Aspose.Cells for .NET 8.4.1 has exposed the ImageOrPrintOptions.SetDesiredSize method to set the dimensions of the resultant image while exporting spreadsheets & charts to images. The SetDesiredSize method accepts two integer type parameters, where first is the desired width and second parameter is the desired height.

The following code snippet shows how to set the desired dimensions while exporting Worksheet to PNG. Please note, similar mechanism can also be used to set the image dimensions while converting Charts to image formats.

```
 string filePath = @"F:\Downloads\source.xlsx";

//Create workbook object from source file
Workbook workbook = new Workbook(filePath);

//Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];

//Set image or print options
//We want one page per sheet
//The image format is in png
//And desired dimensions are 400x400
ImageOrPrintOptions opts = new ImageOrPrintOptions();
opts.OnePagePerSheet = true;
opts.ImageFormat = ImageFormat.Png;
opts.SetDesiredSize(400, 400);

//Render sheet into image
SheetRender sr = new SheetRender(worksheet, opts);
sr.ToImage(0, "output.png"); 
```

## Render Cell Comments in PDF

Microsoft Excel has predefined settings to render comments while printing the spreadsheet or saving them in PDF format. Aspose.Cells APIs have borrowed this concept from Microsoft Excel and have exposed the PageSetup.PrintComments property & PrintCommentsType enumeration to facilitate the rendering of comments while converting spreadsheets to PDF format. The PrintCommentsType enumeration has the following constants that behave similarly as of Microsoft Excel application.

*   PrintNoComments: Comments are not to be rendered.
*   PrintInPlace: Comments are to be rendered where they are placed.
*   PrintSheetEnd: Comments are to be rendered at the end of worksheet.

## Format Sub-String of DataLabels' Text

The API has recently exposed the DataLabels.Characters method to retrieve an instance of FontSetting class that corresponds to the sub-string of ChartPoint.DataLabels. In turn, the instance of FontSetting class can be used to format the sub-string of the Data Labels with different font settings & color.

The following code snippet shows how to use the DataLabels.Characters method.

```
 string filePath = @"F:\Downloads\source.xlsx";

//Create a workbook from source Excel file
Workbook workbook = new Workbook(filePath);

//Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];

//Access the first chart inside the sheet
Chart chart = worksheet.Charts[0];

//Access the data label of first series first point
DataLabels dlbls = chart.NSeries[0].Points[0].DataLabels;

//Set data label text
dlbls.Text = "Rich Text Label";

//Set the font setting of the first 10 characters
FontSetting fntSetting =  dlbls.Characters(0, 10);
fntSetting.Font.Color = Color.Red;
fntSetting.Font.IsBold = true;

//Save the workbook
workbook.Save("output.xlsx"); 
```

## Determine if Workbook is Licensed

Aspose.Cells for .NET 8.4.1 has exposed the Workbook.IsLicensed attribute which could be of great help in determining if the license file/key has been successfully loaded or not. If you access this property before setting the license, it will return false otherwise true for properly set valid license.

The following sample code demonstrates the usage of Workbook.IsLicensed property.

```
 //Create Workbook object
Workbook workbook = new Workbook();

//Check if the license is loaded or not
if (!workbook.IsLicensed)
{
	//Set license
	License license = new License();
	lic.SetLicense(licPath);
}
else
{
        //do process
} 
```

## Other Enhancements and Fixes

In the new version, we have also provided the following new enhancements:

*   Provided support for bullets while using Cell.HtmlString attribute.
*   Export Chart to SVG with viewBox attribute.

We have fixed a few exceptions that occurred while reading and writing Microsoft Excel file formats, loading an MHTML file format, refreshing Chart's cache and performing Auto-Fit operations.

In this release, several important issues have been addressed. For example, issues around writing Microsoft Excel file formats, applying formatting to the cells, copying rows, manipulating PivotTables, using PageSetup options, rendering HTML file format, manipulating shapes, rendering images from Excel worksheets, manipulating charts with formatting, rendering images files from charts and exporting Excel workbooks to PDF format have been resolved. We have also enhanced the Aspose.Cells formula calculation engine further and fixed a few relevant issues in this release.

We have supported moving worksheets within a workbook in the desktop based Grid control provided by Aspose.Cells for .NET. We also figured out issues around rendering shapes, copying/ pasting rows in the web based Grid control by Aspose.Cells for .NET.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 8.4.1, please visit the [download page][2].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png "Aspose.Cells for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.cells-for-.net/entry621506.aspx




