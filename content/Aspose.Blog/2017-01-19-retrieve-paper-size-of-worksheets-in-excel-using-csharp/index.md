---
title: 'Retrieve Paper Size of Worksheets in Excel using C#'
date: Thu, 19 Jan 2017 10:13:36 +0000
draft: false
url: /2017/01/19/retrieve-paper-size-of-worksheets-in-excel-using-csharp/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce our next version of [Aspose.Cells for .NET v17.1.0][1]. The new release includes some valuable features and other enhancements with critical bug fixes. Please see the release notes in order to know what is new/enhanced and what has been changed/fixed with this version of Aspose.Cells for .NET. If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you to check the complete Public API Changes section to know what APIs are changed so far. We have highlighted some important features and other enhancements here.

## Improved Custom Load Filtering Mechanism

The LoadFilter class allows to customize the loading process as per the properties of the Worksheet. In order to customize the loading process, one has to override the LoadFilter.StartSheet method. Please note, there are just a few properties that can be used for a given worksheet object in this scenario because most of the data and properties have not been loaded yet. The available Worksheet properties are: Name, Index & VisibilityType.

With the release of Aspose.Cells for .NET 17.1.0, the API has added the setter for the LoadFilter.LoadDataFilterOptions property to replace the m\_LoadDataFilterOptions instance variable. Users may change the LoadDataFilterOptions property in their own implementation of LoadFilter class to control the behavior of loading template files.

In order to get more in-depth understanding of the new filtering mechanism, please check the detailed article on Filtering Objects at Load Time.

## Get Paper Size of the Worksheet

Sometimes, application requirement could be to retrieve the worksheet's paper size in the unit of Inches, which can now be achieved using the PageSetup.PaperWidth and PageSetup.PaperHeight properties. The PageSetup.PaperWidth and PageSetup.PaperHeight properties are of type double representing the paper width & height in the unit of inches while considering the page orientation.

The following code snippet tries to explain the usage of PageSetup.PaperWidth and PageSetup.PaperHeight properties. Please review the detailed article if you wish to get more in-depth knowledge on how to get the worksheet's paper size.

```
//Create workbook
Workbook wb = new Workbook();

//Access first worksheet
Worksheet ws = wb.Worksheets[0];

//Set paper size to A2 and print paper width and height in inches
ws.PageSetup.PaperSize = PaperSizeType.PaperA2;
Debug.WriteLine("PaperA2: " + ws.PageSetup.PaperWidth + "x" + ws.PageSetup.PaperHeight);

//Set paper size to A3 and print paper width and height in inches
ws.PageSetup.PaperSize = PaperSizeType.PaperA3;
Debug.WriteLine("PaperA3: " + ws.PageSetup.PaperWidth + "x" + ws.PageSetup.PaperHeight);

//Set paper size to A4 and print paper width and height in inches
ws.PageSetup.PaperSize = PaperSizeType.PaperA4;
Debug.WriteLine("PaperA4: " + ws.PageSetup.PaperWidth + "x" + ws.PageSetup.PaperHeight);

//Set paper size to Letter and print paper width and height in inches
ws.PageSetup.PaperSize = PaperSizeType.PaperLetter;
Debug.WriteLine("PaperLetter: " + ws.PageSetup.PaperWidth + "x" + ws.PageSetup.PaperHeight); 
```

## Specify the Number of Significant Digits

Aspose.Cells APIs store 17 significant digits of double values unlike Excel application which stores only 15 significant digits. You can override this default behavior of Aspose.Cells APIs while using the newly exposed CellsHelper.SignificantDigits property.

The following code snippet enforces the Aspose.Cells APIs to use 15 significant digits while storing double values to the spreadsheet files of type XLSX. Please review the detailed article if you wish to get more in-depth knowledge on how to specify significant digits.

```
//By default, Aspose.Cells stores 17 significant digits unlike
//MS-Excel which stores only 15 significant digits
CellsHelper.SignificantDigits = 15;

//Create workbook
Workbook workbook = new Workbook();

//Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];

//Access cell A1
Cell c = worksheet.Cells["A1"];

//Put double value, only 15 significant digits as specified by
//CellsHelper.SignificantDigits above will be stored in excel file just like MS-Excel does
c.PutValue(1234567890.123451711);

//Save the workbook
workbook.Save("out_SignificantDigits.xlsx"); 
```

## Verify Custom Pattern for the Style Object

Aspose.Cells for .NET 17.1.0 has added the CheckCustomNumberFormat property to the WorkbookSettings class. The CheckCustomNumberFormat is useful in checking if the Style.Custom property has been set properly or not. In case the Style.Custom property has been set improperly, that is; the value does not correspond to valid pattern then the Aspose.Cells for .NET APIs will throw CellsException with appropriate message.

The following code snippet tried to assign an invalid custom format to the Style.Custom property. Since, the code has already set WorkbookSettings.CheckCustomNumberFormat property to true therefore the statement to set the Style.Custom property will cause CellsException.

```
//Create a workbook
Workbook wb = new Workbook();

//Setting this property to true will make Aspose.Cells to throw exception
//when invalid custom number format is assigned to Style.Custom property
wb.Settings.CheckCustomNumberFormat = true;

//Access first worksheet
Worksheet ws = wb.Worksheets[0];

//Access cell A1 and put some number inside it
Cell c = ws.Cells["A1"];
c.PutValue(2347);

//Access cell's style and set its Style.Custom property
Style s = c.GetStyle();
//This line will throw exception if Workbook.Settings.CheckCustomNumberFormat is set to true
s.Custom = "ggg @ fff"; //Invalid custom number format
c.SetStyle(s); 
```

## Other Enhancements and Fixes

Aspose.Cells for .NET 17.1.0 has enhanced its core for more stability as well as fixed a few critical bugs. Moreover, there are numerous minor enhancements in order to improve the overall usage of the API. A few of the worth mentioning enhancements are as follow.

*   Ability to read the color of shape's glow effect.
*   Support for rendering gradient fill for WordArt objects while converting spreadsheets to HTML.
*   Support to load Excel 2016 chart types.
*   Bind Worksheet to a DataSet at Runtime using GridWeb
*   Bind Worksheet to a Customized Collection Object using GridWeb
*   Enhanced HTML parsing engine for inline CSS.
*   Handled NullReferenceException and other exceptions while loading/saving MS Excel files

Furthermore, in this release, we have fixed several other issues. For example, issues around reading/writing MS Excel Excel file formats, rendering wordart and smartart shapes, rendering charts and other shapes, manipulating ListObject/Table, formatting and manipulating Pivot Tables, conditional formatting, rendering to HTML file format, rendering images from Excel worksheets, rendering images files from charts and exporting Excel workbooks to PDF format have been resolved. The formula calculation engine is improved too in the new release.

## Changes to the Public API

This version of Aspose.Cells for .NET has made some changes to the Public APIs. A few of the worth mentioning changes are as follow whereas details can be viewed from the Migration Manual.

*   Several new fields have been added to the ChartType enumeration which represents chart types specific to Excel 2016.
*   A new field Percentage has been added to the DisplayUnitType enumeration that indicates the values on the chart shall be divided by 0.01.
*   The instance variable m\_LoadDataFilterOptions has been removed. It is advised to use the LoadFilter.LoadDataFilterOptions property instead.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][2].
*   [Aspose.Cells for .NET Download Section][3].
*   Aspose.Cells for .NET Documentation – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][4] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][5] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][6] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://products.aspose.com/cells/net
[2]: https://www.aspose.com/products/cells/net
[3]: http://www.aspose.com/downloads/cells/net
[4]: http://www.aspose.com/api/net/cells
[5]: https://forum.aspose.com/
[6]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




