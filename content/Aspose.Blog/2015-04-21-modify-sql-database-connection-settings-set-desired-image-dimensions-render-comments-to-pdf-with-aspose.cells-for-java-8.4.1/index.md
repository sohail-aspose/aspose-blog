---
title: 'Modify SQL Database Connection Settings, Set Desired Image Dimensions, Render Comments To PDF with Aspose.Cells for Java 8.4.1'
date: Tue, 21 Apr 2015 13:45:17 +0000
draft: false
url: /2015/04/21/modify-sql-database-connection-settings-set-desired-image-dimensions-render-comments-to-pdf-with-aspose.cells-for-java-8.4.1/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for Java][1]](http://www.aspose.com/java/excel-component.aspx "Aspose.Cells for Java - Excel Java APIs")

We are pleased to announce the monthly release of Aspose.Cells for Java, version 8.4.1. This release contains many useful features & enhancements that you may start exploring immediately, however, before you head to the [download section][2] here is a look at just a few of the worth mentioning features in this month’s release. For a full list of bug fixes and improvements please refer to the download page in the link above. In case you are planning to upgrade the API from any previous revision, we strongly suggest you to go through the Public API Changes section first to know what has been changed since your current version of the API.

## Code Baseline Moved to Java 6

Starting with this release, Aspose.Cells for Java has dropped the support for Java versions prior to v6 and has moved its codebase to Java 6 (Java 7 and 8 are also supported). Reason being, Sun/Oracle has discontinued the support for all JDK revisions prior to 1.6. Now the Aspose.Cells for Java package contains a single Jar that works well with Java 6, 7 & 8.

## Modify SQL Database Connection Settings

Microsoft Excel application allows to create the database connection so that the data could be fetched and loaded in the spreadsheets to refresh Pivot Tables, Charts or just the worksheet. The external data source is connected to the workbook through a data connection, which is a set of information that describes how to locate, log in, query, and access the external data source.

Aspose.Cells for Java API does not allow to create a database connection yet, however, some revisions back, the API had exposed the ExternalConnection class that contains the method & properties that could be used to inspect the database connection details stored in a spreadsheet. Most of the properties associated with ExternalConnection class were read-only until the release of Aspose.Cells for Java 8.4.1. With this release, the API has provided the support to manipulate the database connection settings. Please check the detailed article on Modify Existing Database Connection Settings.

## Set Desired Image Dimensions for Spreadsheet & Chart Export

Another worth mentioning feature is the support for setting desired image dimensions while exporting spreadsheets & charts to image formats. Aspose.Cells for Java 8.4.1 has exposed the ImageOrPrintOptions.setDesiredSize method to set the dimensions of the resultant image while exporting spreadsheets & charts to images. The setDesiredSize method accepts two integer type parameters, where first is the desired width and second parameter is the desired height.

The following code snippet shows how to set the desired dimensions while exporting Worksheet to PNG. Please note, similar mechanism can also be used to set the image dimensions while converting Charts to image formats.

```
 //Create an instance of Workbook & load an existing spreadsheet
com.aspose.cells.Workbook workbook = new com.aspose.cells.Workbook(input);

//Access first worksheet
com.aspose.cells.Worksheet worksheet = workbook.getWorksheets().get(0);

//Create an instance of ImageOrPrintOptions
com.aspose.cells.ImageOrPrintOptions options = new com.aspose.cells.ImageOrPrintOptions();

//Set resultant image format
options.setImageFormat(com.aspose.cells.ImageFormat.getPng());

//Set desired dimensions as 400x400
options.setDesiredSize(400, 400);

//Render worksheet to image
com.aspose.cells.SheetRender renderer = new com.aspose.cells.SheetRender(worksheet, options);
renderer.toImage(0, "output.png"); 
```

## Render Cell Comments in PDF

Microsoft Excel has predefined settings to render comments while printing the spreadsheet or saving them in PDF format. Aspose.Cells APIs have borrowed this concept from Microsoft Excel and have exposed the PageSetup.PrintComments property & PrintCommentsType enumeration to facilitate the rendering of comments while converting spreadsheets to PDF format. The PrintCommentsType enumeration has the following constants that behave similarly as of Microsoft Excel application.

*   PRINT\_NO\_COMMENTS: Comments are not to be rendered.
*   PRINT\_IN\_PLACE: Comments are to be rendered where they are placed.
*   PRINT\_SHEET\_END: Comments are to be rendered at the end of worksheet.

## Format Sub-String of DataLabels' Text

The API has recently exposed the DataLabels.characters method to retrieve an instance of FontSetting class that corresponds to the sub-string of a ChartPoints.DataLabels. In turn, the instance of FontSetting class can be used to format the sub-string of the Data Labels with different font settings & color.

The following code snippet shows how to use the DataLabels.characters method.

```
 //Create a workbook from source Excel file
com.aspose.cells.Workbook workbook = new com.aspose.cells.Workbook(input);

//Access first worksheet
com.aspose.cells.Worksheet worksheet = workbook.getWorksheets().get(0);

//Access the first chart inside the sheet
com.aspose.cells.Chart chart = worksheet.getCharts().get(0);

//Access the data label of first series first point
com.aspose.cells.DataLabels labels = chart.getNSeries().get(0).getPoints().get(0).getDataLabels();

//Set data label text
labels.setText("Rich Text Label");

//Set the font setting of the first 10 characters
com.aspose.cells.FontSetting settings = labels.characters(0, 10);
settings.getFont().setColor(com.aspose.cells.Color.getRed());
settings.getFont().setBold(true);

//Save the workbook
workbook.save(output); 
```

## Determine if Workbook is Licensed

Aspose.Cells for Java 8.4.1 has exposed the Workbook.isLicensed which could be of great help in determining if the license has been successfully loaded or not. If you access this property before setting the license, it will return false and true for a properly set valid license.

The following sample code demonstrates the usage of Workbook.isLicensed property.

```
 //Create Workbook object
com.aspose.cells.Workbook workbook = new com.aspose.cells.Workbook();

//Check if the license is loaded or not
if (!workbook.isLicensed())
{
	//Set license
	com.aspose.cells.License license = new com.aspose.cells.License();
	lic.SetLicense(licPath);
}
else
{
        //do process
} 
```

## Other Enhancements & Fixes

Aspose.Cells for Java 8.4.1 has fixed a number of issues and enhanced the core to accommodate many customer requested features. Following are a few worth mentioning enhancements & fixes.

*   Enhanced the ImageOrPrintOptions to facilitate the users who wish to render in SVG format with viewBox attribute.
*   Provided support for bullets while using Cell.setHtmlString method or SmartMarkers.
*   Provided support for setting different borders through web operation for Aspose.Cells.GridWeb component.
*   Improved the navigation with arrow keys in the Aspose.Cells.GridWeb component.
*   Improved the import of spreadsheets in the Aspose.Cells.GridWeb component that contain conditional formatting rules.
*   Improved the Chart2Image feature for missing & overlapping legend entries and grid lines.
*   Addressed a few exceptions related to the loading of spreadsheets with Aspose.Cells for Java API.

Please visit the documentation for details, and if you still have any questions, we always welcome inquiries on [Aspose.Cells Support Forum][3].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Cells-for-Java_100.png "Aspose.Cells for Java"
[2]: http://www.aspose.com/community/files/72/java-components/aspose.cells-for-java/entry621853.aspx "Download Aspose.Cells for Java 8.4.1"
[3]: https://forum.aspose.com/




