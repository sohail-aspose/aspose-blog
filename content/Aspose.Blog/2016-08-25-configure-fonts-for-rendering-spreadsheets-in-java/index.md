---
title: 'Configure Fonts for Rendering Spreadsheets in Java'
date: Thu, 25 Aug 2016 12:48:34 +0000
draft: false
url: /2016/08/25/configure-fonts-for-rendering-spreadsheets-in-java/
author: Babar Raza
summary: ''
tags: ['Copy Ranges', 'Copy Rows', 'Excel Formulas', 'Excel Java APIs', 'Excel to HTML', 'Font Sources', 'Font Substitution', 'Formula Calculation', 'Manipulate Spreadsheets', 'Spreadsheet to HTML', 'TrueType Fonts']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We are pleased to announce the release of [Aspose.Cells for Java 8.9.2][1]. This release includes many new features and enhancements along with some critical bug fixes that further improve the overall stability of the API. Please check the detailed release notes in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Java. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the Public API Changes section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Configure Fonts for Rendering Spreadsheets

Aspose.Cells for Java API has exposed a number of new classes as well as an enumeration to configure font sources for rendering spreadsheets to image formats and PDF. Most important class is the FontConfigs which has many useful factory methods to either set the font sources or set the font substitution along with some inspection APIs to retrieve the list of specified font sources as well as font substitutions.

### Set Font Sources

Aspose.Cells APIs search the operating system's default font directory for the required fonts. In case the required fonts are not available in the system's font directory then the APIs search through the custom (user defined) directories. The FontConfigs class has exposed a number of ways to set custom font directories & files as detailed below.

*   FontConfigs.setFontFolder method is useful if there is only one folder to be set.
*   FontConfigs.setFontFolders method is useful when the font files reside in multiple folders and you wish to set all folders separately rather than combining all font files in a single folder.
*   FontConfigs.setFontSources method is useful when you wish to load fonts from multiple folders or font files or font data from an array of bytes.

Here is a simple usage scenario of aforementioned methods. Please note, in case more than one methods have been used to specify the font sources then only the last settings will take effect.

```
//Defining string variables to store paths to font folders & font file
String fontFolder1 = "D:/Arial";
String fontFolder2 = "D:/Calibri";
String fontFile = "D:/Arial/arial.ttf";

//Setting first font folder with setFontFolder method
//Second parameter directs the API to search the sub folders for font files
FontConfigs.setFontFolder(fontFolder1, true);

//Setting both font folders with setFontFolders method
//Second parameter prohibits the API to search the sub folders for font files
FontConfigs.setFontFolders(new String[] { fontFolder1, fontFolder2 }, false);

//Defining FolderFontSource
FolderFontSource sourceFolder = new FolderFontSource(fontFolder1, false);

//Defining FileFontSource
FileFontSource sourceFile = new FileFontSource(fontFile);

//Defining MemoryFontSource
byte[] bytes = Files.readAllBytes(new File(fontFile).toPath());
MemoryFontSource sourceMemory = new MemoryFontSource(bytes);

//Setting font sources
FontConfigs.setFontSources(new FontSourceBase[] { sourceFolder, sourceFile, sourceMemory});
```

### Substitute Fonts

Aspose.Cells APIs also provide the ability to set user defined font substitutions for rendering purposes. This mechanism is helpful when a required font is not available on the machine where conversion has to take place. You can provide a list of font names as alternative to the originally required font. In order to achieve this, the Aspose.Cells APIs have exposed the FontConfigs.setFontSubstitutes method which accepts 2 parameters. The first parameter is of type String, which should be the name of font which needs to be substituted. The second parameter is an array of type String. You can provide a list of font names as substitution to original font (specified in the first parameter).

Here is a simple usage scenario of FontConfigs.setFontSubstitutes method.

```
//Substituting the Arial font with Times New Roman & Calibri
FontConfigs.setFontSubstitutes("Arial", new String[] { "Times New Roman", "Calibri" });
```

### Inspect Configured Font Sources & Substitutions

The Aspose.Cells APIs have also provided means to gather information on what sources and substitutions have been set.

*   FontConfigs.getFontSources method returns an array of type FontSourceBase containing the list of specified font sources. In case, no sources have been set, the FontConfigs.getFontSources method will return an empty array.
*   FontConfigs.getFontSubstitutes method accepts a parameter of type String allowing to specify the font name for which a substitution has been set. In case, no substitution has been set for the specified font name then the FontConfigs.getFontSubstitutes method will return null.

Please check the detailed article on Configurable Font Sources for more in-depth knowledge of newly exposed APIs.

## Recursive Calculation of Formulas

Aspose.Cells for Java 8.9.2 has exposed the Boolean type CalculationOptions.Recursive property. Setting the CalculationOptions.Recursive property to true and passing the object to calculateFormula method directs the Aspose.Cells APIs to calculate the dependent cells recursively when calculating cells which depends on other cells.

Below provided code snippet demonstrates the simple usage scenario of newly exposed CalculationOptions.Recursive property. In order to get more details of possible usage scenarios, please check the detailed article on Optimizing Formula Calculation Time.

```
//Load a sample spreadsheet in an instance of Workbook
Workbook book = new Workbook(dir + "sample.xlsx");

//Initialize CalculationOptions & set Recursive property to true
CalculationOptions options = new CalculationOptions();
options.setRecursive(true);

//Recalculate formulas
book.calculateFormula(options);
```

## Control Chart's Data Source while Copying Rows

Aspose.Cells for Java API has exposed the Boolean type CopyOptions.ReferToDestinationSheet property along with the an overload of Cells.copyRows method in order to facilitate the copy rows operation when rows to be copied also contains a chart and its data source. You can make use of these new APIs to point the chart's data source to the source or destination worksheets.

Below provided code snippet demonstrates the simple usage scenario whereas a detailed article can be reviewed at Control the Data Source of Chart while Copying Rows.

```
//Load a sample spreadsheet in an instance of Workbook
Workbook book = new Workbook(dir + "sample.xlsx");

//Access the worksheet containing the chart & its data source
Worksheet source = book.getWorksheets().get(0);

//Add a new worksheet to the collection
Worksheet destination = book.getWorksheets().get(book.getWorksheets().add());

//Initialize CopyOptions and set its ReferToDestinationSheet property to true
CopyOptions options = new CopyOptions();
options.setReferToDestinationSheet(true);

//Copy the rows
destination.getCells().copyRows(source.getCells(), 0, 0, source.getCells().getMaxDisplayRange().getRowCount(), options);

//Save the result on disc
book.save(dir + "output.xlsx");
```

## Implement IFilePathProvider Interface

Aspose.Cells for Java 8.9.2 allows to get/set the IFilePathProvider for exporting worksheets to separate HTML files. These new APIs are helpful in scenarios where hyperlinks in one worksheet points to a location in another worksheet, where application requirement is to render each worksheet to separate HTML file. Implementing the IFilePathProvider allows to keep the aforementioned hyperlinks intact regardless of the fact that they are pointing to a location in a separate resultant HTML file.

Following is the simple usage scenario of HtmlSaveOptions.FilePathProvider property. In order to get more in-depth knowledge of these APIs, please check the detailed article on Implementing IFilePathProvider Interface.

```
//Load a spreadsheet in an instance of Workbook
Workbook book = new Workbook(dir + "sample.xlsx");

//Save each Worksheet to separate  HTML file
for (int i = 0; i < book.getWorksheets().getCount(); i++)
{
	book.getWorksheets().setActiveSheetIndex(i);

	//Create an instance of HtmlSaveOptions & set FilePathProvider property
	HtmlSaveOptions options = new HtmlSaveOptions();
	options.setExportActiveWorksheetOnly(true);
	options.setFilePathProvider(new IFilePathProvider() 
	{ 
		public String getFullName(String sheetName)
		{
		    if ("Sheet2".equals(sheetName))
		    {
		        return "sheet1.html";
		    }
		    else if ("Sheet3".equals(sheetName))
		    {
		        return "sheet2.html";
		    }

		    return "";
		}
	});

	 //Write HTML file to disc
	 book.save(dir + "sheet"+ i +".html", options);
}
```

## Other Enhancements & Fixes

Aspose.Cells for Java 8.9.2 has fixed a few critical bugs as well as enhanced its core for more stability. A few of the worth mentioning enhancements are as follow.

*   Enhanced HTML rendering engine for shapes such as TextBoxes.
*   Improved PDF rendering engine for charts as well as cell text alignment.
*   Tweaked Aspose.Cells' formula calculation engine to match the results with Excel application.
*   Handled a few exceptions such as IndexOutOfBoundsException, NumberFormatException & OutOfMemoryError for certain scenarios.

## Public API Changes

Aspose.Cells for Java 8.9.2 has made a few changes to the publicly exposed APIs in order to keep the API usage simple. Some of the changes are listed as follow.

*   The factory methods such as CellsHelper.setFontDir & setFontDirs have been marked obsoleted whereas the alternative approach has been exposed via FontConfigs class as detailed above.
*   A few of the properties from Shape class has been marked obsoleted whereas alternative properties have been exposed. For instance, the Shape.FillFormat & Shape.LineFormat properties have been replaced by Shape.Fill & Shape.Line properties respectively.
*   The ShapeFont class has been replaced by the TextOptions class whereas the FontSetting.ShapeFont property has been replaced by the FontSetting.TextOptions.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][2].
*   [Aspose.Cells for Java Download Section][3].
*   [Aspose.Cells for Java Documentation][4] – up-to-date documentation containing Programmer's Guide, Knowledge Base, and much more.
*   [Aspose.Cells for Java API Reference Guide][5] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][6] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][7] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Java Examples][8] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://products.aspose.com/cells/java
[2]: https://products.aspose.com/cells/java
[3]: https://downloads.aspose.com/cells/java
[4]: https://docs.aspose.com/cells/java
[5]: https://apireference.aspose.com/cells/java
[6]: https://forum.aspose.com/
[7]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/
[8]: https://github.com/asposecells/Aspose_Cells_Java




