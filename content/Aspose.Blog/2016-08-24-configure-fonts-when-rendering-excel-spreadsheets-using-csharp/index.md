---
title: 'Configure Fonts when Rendering Excel Spreadsheets using C#'
date: Wed, 24 Aug 2016 19:31:44 +0000
draft: false
url: /2016/08/24/configure-fonts-when-rendering-excel-spreadsheets-using-csharp/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce our next version of [Aspose.Cells for .NET v8.9.2][1]. This release includes several new features and other enhancements with critical bug fixes. Please see the release notes in order to know what is new and what has been changed/fixed with this version of Aspose.Cells for .NET. If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you to check the complete Public API Changes section to know what APIs are changed so far. We have highlighted some important features and other enhancements here.

## Configure Fonts for Rendering Spreadsheets

Aspose.Cells API has exposed a number of new classes as well as an enumeration to configure font sources for rendering spreadsheets to image formats and PDF. Most important class is the FontConfigs which has many useful factory methods to either set the font sources or set the font substitution along with some inspection APIs to retrieve the list of specified font sources as well as font substitutions.

### Set Font Sources

Aspose.Cells APIs search the operating system's default font directory for the required fonts. In case the required fonts are not available in the system's font directory then the APIs search through the custom (user defined) directories. The FontConfigs class has exposed a number of ways to set custom font directories & files as detailed below.

*   FontConfigs.SetFontFolder method is useful if there is only one folder to be set.
*   FontConfigs.SetFontFolders method is useful when the font files reside in multiple folders and you wish to set all folders separately rather than combining all font files in a single folder.
*   FontConfigs.SetFontSources method is useful when you wish to load fonts from multiple folders or font files or font data from an array of bytes.

Here is a simple usage scenario of aforementioned methods. Please note, in case more than one methods have been used to specify the font sources then only the last settings will take effect.

```
//Defining string variables to store paths to font folders & font file
// Defining string variables to store paths to font folders & font file
string fontFolder1 = "D:/Arial";
string fontFolder2 = "D:/Calibri";
string fontFile = "D:/Arial/arial.ttf";

// Setting first font folder with SetFontFolder method
// Second parameter directs the API to search the subfolders for font files
FontConfigs.SetFontFolder(fontFolder1, true);

// Setting both font folders with SetFontFolders method
// Second parameter prohibits the API to search the subfolders for font files
FontConfigs.SetFontFolders(new string[] { fontFolder1, fontFolder2 }, false);

// Defining FolderFontSource
FolderFontSource sourceFolder = new FolderFontSource(fontFolder1, false);

// Defining FileFontSource
FileFontSource sourceFile = new FileFontSource(fontFile);

// Defining MemoryFontSource
MemoryFontSource sourceMemory = new MemoryFontSource(System.IO.File.ReadAllBytes(fontFile));

//Setting font sources
FontConfigs.SetFontSources(new FontSourceBase[] { sourceFolder, sourceFile, sourceMemory});
```

### Substitute Fonts

Aspose.Cells APIs also provide the ability to set user defined font substitutions for rendering purposes. This mechanism is helpful when a required font is not available on the machine where conversion has to take place. You can provide a list of font names as alternative to the originally required font. In order to achieve this, the Aspose.Cells APIs have exposed the FontConfigs.SetFontSubstitutes method which accepts 2 parameters. The first parameter is of type string, which should be the name of font which needs to be substituted. The second parameter is an array of type string. You can provide a list of font names as substitution to original font (specified in the first parameter).

Here is a simple usage scenario of FontConfigs.SetFontSubstitutes method.

```
// Substituting the Arial font with Times New Roman & Calibri
FontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman", "Calibri" });
```

### Inspect Configured Font Sources & Substitutions

The Aspose.Cells APIs have also provided means to gather information on what sources and substitutions have been set.

*   FontConfigs.GetFontSources method returns an array of type FontSourceBase containing the list of specified font sources. In case, no sources have been set, the FontConfigs.GetFontSources method will return an empty array.
*   FontConfigs.GetFontSubstitutes method accepts a parameter of type string allowing to specify the font name for which a substitution has been set. In case, no substitution has been set for the specified font name then the FontConfigs.GetFontSubstitutes method will return null.

Please check the detailed article on Configurable Font Sources for more in-depth knowledge of newly exposed APIs.

## Recursive Calculation of Formulas

Aspose.Cells for .NET 8.9.2 has exposed the Boolean type CalculationOptions.Recursive property. Setting the CalculationOptions.Recursive option to true and passing the object to CalculateFormula method directs the Aspose.Cells APIs to calculate the dependent cells recursively when calculating cells which depends on other cells.

Below provided code snippet demonstrates the simple usage scenario of newly exposed CalculationOptions.Recursive property. In order to get more details of possible usage scenarios, please check the detailed article on Optimizing Formula Calculation Time.

```
// Load a sample spreadsheet in an instance of Workbook
var book = new Workbook(dir + "sample.xlsx");

// Initialize CalculationOptions & set Recursive property to true
var options = new CalculationOptions();
options.Recursive = true;

// Recalculate formulas
book.CalculateFormula(options);
```

## Control Chart's Data Source while Copying Rows

Aspose.Cells for .NET API has exposed the Boolean type CopyOptions.ReferToDestinationSheet property along with the an overload of Cells.CopyRows method in order to facilitate the copy rows operation when rows to be copied also contains a chart and its data source. You can make use of these new APIs to point the chart's data source to the source or destination worksheets.

Below provided code snippet demonstrates the simple usage scenario whereas a detailed article can be reviewed at Control the Data Source of Chart while Copying Rows.

```
// Load a sample spreadsheet in an instance of Workbook
var book = new Workbook(dir + "sample.xlsx");

// Access the worksheet containing the chart & its data source
var source = book.Worksheets[0];

// Add a new worksheet to the collection
var destination = book.Worksheets[book.Worksheets.Add()];

// Initialize CopyOptions and set its ReferToDestinationSheet property to true
CopyOptions options = new CopyOptions();
options.ReferToDestinationSheet = true;

// Copy the rows
destination.Cells.CopyRows(source.Cells, 0, 0, source.Cells.MaxDisplayRange.RowCount, options);

// Save the result on disc
book.Save(dir + "output.xlsx");
```

## Implement IFilePathProvider Interface

Aspose.Cells for .NET 8.9.2 allows to get/set the IFilePathProvider for exporting worksheets to separate HTML files. These new APIs are helpful in scenarios where hyperlinks in one worksheet points to a location in another worksheet, where application requirement is to render each worksheet to separate HTML file. Implementing the IFilePathProvider allows to keep the aforementioned hyperlinks intact regardless of the fact that they are pointing to a location in a separate resultant HTML file.

In order to get more in-depth knowledge of these APIs, please check the detailed article on Implementing IFilePathProvider Interface.

## Important Public API Changes

Aspose.Cells for .NET 8.9.2 has made a few changes to the publicly exposed APIs in order to keep the API usage simple. Some of the changes are listed as follow.

*   The factory attributes such as, CellsHelper.FontDir & FontDirs have been marked obsoleted whereas the alternative approach has been exposed via FontConfigs class as detailed above.
*   A few of the properties from Shape class has been marked obsoleted whereas alternative properties have been exposed. For instance, the Shape.FillFormat & Shape.LineFormat properties have been replaced by Shape.Fill & Shape.Line properties respectively.
*   The ShapeFont class has been replaced by the TextOptions class whereas the FontSetting.ShapeFont property has been replaced by the FontSetting.TextOptions.

## Other Enhancements and Fixes

Aspose.Cells has fixed a few critical bugs as well as enhanced its core for more stability. A few of the worth mentioning enhancements are as follow.

*   Enter Cell Data of GridWeb Worksheet in Percentage Format.
*   Enhanced HTML rendering engine.
*   Improved PDF rendering engine for charts, shapes as well as style/formatting including cell's text alignment.
*   Tweaked Aspose.Cells' formula calculation engine to match the results with Excel application.

We have handled a few exceptions regarding reading and writing Excel and HTML file formats.

In this release, several important issues have been addressed. For example, issues around reading and writing Microsoft Excel file formats, rendering images from Excel worksheets, rendering images files from charts and exporting Excel workbooks to PDF format have been resolved.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][2].
*   [Aspose.Cells for .NET Download Section][3].
*   Aspose.Cells for .NET Documentation – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][4] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][5] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][6] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://www.aspose.com/downloads/cells/net/new-releases/aspose.cells-for-.net-8.9.2/
[2]: http://www.aspose.com/.net/excel-component.aspx
[3]: http://www.aspose.com/downloads/cells/net
[4]: http://www.aspose.com/api/net/cells
[5]: https://forum.aspose.com/
[6]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




