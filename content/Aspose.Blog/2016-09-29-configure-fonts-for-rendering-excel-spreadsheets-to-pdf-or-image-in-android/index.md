---
title: 'Configure Fonts for Rendering Excel Spreadsheets in Android'
date: Thu, 29 Sep 2016 05:28:36 +0000
draft: false
url: /2016/09/29/configure-fonts-for-rendering-excel-spreadsheets-to-pdf-or-image-in-android/
author: Babar Raza
summary: ''
tags: ['ActiveX controls', 'Create Chart', 'Dynamic Creation of Spreadsheets', 'Excel APIs', 'Excel Android APIs', 'Excel Chart to Image', 'Excel Charts', 'Excel Formulas', 'Excel Table', 'Excel to HTML', 'Objects', 'PDF', 'Recursive Calculation', 'Spreadsheet Creation', 'shapes']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Android_100.png" alt="Aspose.Cells for Android logo">}}


We are pleased to announce the release of [Aspose.Cells for Android 9.0.0][1]. This release includes a number of new features, enhancements, and bug fixes that further improve the overall stability and usability of the API. Please check the release notes in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Android. If you are planning to upgrade the API from any previous version, we strongly suggest you check the Public API Changes section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Configure Fonts for Rendering Spreadsheets

Aspose.Cells for Android API has exposed a number of new classes as well as an enumeration to configure font sources for rendering spreadsheets to image formats and PDF. The most important class is the FontConfigs which has many useful factory methods to either set the font sources or set the font substitution along with some inspection APIs to retrieve the list of specified font sources as well as font substitutions.

### Set Font Sources

Aspose.Cells APIs search the operating system's default font directory for the required fonts. In case the required fonts are not available in the system's font directory then the APIs search through the custom (user-defined) directories. The FontConfigs class has exposed a number of ways to set custom font directories & files as detailed below.

*   FontConfigs.setFontFolder method is useful if there is only one folder to be set.
*   FontConfigs.setFontFolders method is useful when the font files reside in multiple folders and you wish to set all folders separately rather than combining all font files in a single folder.
*   FontConfigs.setFontSources method is useful when you wish to load fonts from multiple folders or font files or font data from an array of bytes.

Here is a simple usage scenario of the aforementioned methods. Please note, in case more than one method have been used to specify the font sources then only the last settings will take effect.

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-SetCustomFontFolders-SetCustomFontFolders.java" >}}

### Substitute Fonts

Aspose.Cells APIs also provide the ability to set user-defined font substitutions for rendering purposes. This mechanism is helpful when a required font is not available on the machine where conversion has to take place. You can provide a list of font names as an alternative to the originally required font. In order to achieve this, the Aspose.Cells APIs have exposed the FontConfigs.setFontSubstitutes method which accepts 2 parameters. The first parameter is of type String, which should be the name of font which needs to be substituted. The second parameter is an array of type String. You can provide a list of font names as a substitution to the original font (specified in the first parameter).

Here is a simple usage scenario of FontConfigs.setFontSubstitutes method.

```
//Substituting the Arial font with Times New Roman & Calibri
FontConfigs.setFontSubstitutes("Arial", new String[] { "Times New Roman", "Calibri" });
```

### Inspect Configured Font Sources & Substitutions

The Aspose.Cells APIs have also provided means to gather information on what sources and substitutions have been set.

*   FontConfigs.getFontSources method returns an array of type FontSourceBase containing the list of specified font sources. In case, no sources have been set, the FontConfigs.getFontSources method will return an empty array.
*   FontConfigs.getFontSubstitutes method accepts a parameter of type String allowing to specify the font name for which a substitution has been set. In case, no substitution has been set for the specified font name then the FontConfigs.getFontSubstitutes method will return null.

Please check the detailed article on [Configurable Font Sources][2] for more in-depth knowledge of newly exposed APIs.

## Recursive Calculation of Formulas

Aspose.Cells for Android 9.0.0 has exposed the Boolean type CalculationOptions.Recursive property. Setting the CalculationOptions.Recursive property to true and passing the object to calculateFormula method directs the Aspose.Cells APIs to calculate the dependent cells recursively when calculating cells which depend on other cells.

Below provided code snippet demonstrates the simple usage scenario of newly exposed CalculationOptions.Recursive property. In order to get more details of possible usage scenarios, please check the detailed article on [Optimizing Formula Calculation Time][3].

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-DecreaseCalculationTime-DecreaseCalculationTime.java" >}}

## Set Class Identifier for OleObjects

Aspose.Cells for Android 9.0.0 has exposed the OleObject.ClassIdentifier property which can be used to retrieve or set the class identifier for an OleObject. Please note, the class identifier decides which application is required to load the embedded resource/OleObject and how. for instance, a PPT (presentation) file can be embedded in a spreadsheet with 2 different views, that is; presentation view or slide view, whereas both views have different class identifier values.

Below provided code snippet demonstrates the simple usage scenario of newly exposed OleObject.ClassIdentifier property. In order to get more details of possible usage scenarios, please check the detailed article on [Class Identifier for OleObjects][4].

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-GetSettheClassIdentifier-GetSettheClassIdentifier.java" >}}

## Control Chart's Data Source while Copying Rows

Aspose.Cells for Android API has exposed the Boolean type CopyOptions.ReferToDestinationSheet property along with the an overload of Cells.copyRows method in order to facilitate the copy rows operation when rows to be copied also contains a chart and its data source. You can make use of these new APIs to point the chart's data source to the source or destination worksheets.

Below provided code snippet demonstrates the simple usage scenario whereas a detailed article can be reviewed at [Control the Data Source of Chart while Copying Rows][5].

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-ChangeDataSource-ChangeDataSource.java" >}}

## Implement IFilePathProvider Interface

Aspose.Cells for Android 9.0.0 allows to get/set the IFilePathProvider for exporting worksheets to separate HTML files. These new APIs are helpful in scenarios where hyperlinks in one worksheet point to a location in another worksheet, where the application requirement is to render each worksheet to separate HTML file. Implementing the IFilePathProvider allows to keep the aforementioned hyperlinks intact regardless of the fact that they are pointing to a location in a separate resultant HTML file.

Following is the simple usage scenario of HtmlSaveOptions.FilePathProvider property. In order to get more in-depth knowledge of these APIs, please check the detailed article on [Implementing IFilePathProvider Interface][6].

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-FilePathProvider-FilePathProvider.java" >}}

## Control the Appearance of Shape's Textual Contents

Aspose.Cells for Android API has exposed the Shape.TextOptions property can be used to control all aspects of the shape's textual contents such as font style, color, font-weight, and so on.

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

Aspose.Cells for Android 9.0.0 has fixed a few critical bugs as well as enhanced its core for more stability. A few of the worth mentioning enhancements are as follows.

*   This release has exposed the ListObject.Comment property to [set the comments for an Excel Table or ListObject][7].
*   The Aspose.Cells APIs can be used to insert and/or [manipulate existing ActiveX controls][8]. One such example in an ActiveX ComboBox which can now be created as well as manipulated with Aspose.Cells for Android APIs.
*   Aspose.Cells for Android API has exposed the ChartPoint.isInSecondaryPlot property with this release. Boolean type property can be used to [detect if a ChartPoint resides on secondary plot or not][9].
*   Aspose.Cells for Android APIs provide support for creating new Excel charts as well manipulating existing ones. With this release, you can now [hide the legend entry's text by setting the fill color to none][10].
*   Aspose.Cells for Android has provided the PivotTable.IsExcel2003Compatible property which can be used to [check if the PivotTable is compatible for Excel 2003 for refreshing][11]. If true, a string must be less than or equal to 255 characters however, if the string is greater than 255 characters, it will be truncated.
*   Another addition to the public API is the HTMLLoadOptions.SupportDivTag which allows to [handle the nested DIV tags while loading HTML in Aspose.Cells object model][12].

## Public API Changes

Aspose.Cells for Android 9.0.0 has made a few changes to the publicly exposed APIs in order to keep the API usage simple. Some of the changes are listed as follows.

*   The Worksheet.SetBackground method has been marked obsoleted whereas the alternative approach has been exposed via Worksheet.BackgroundImage property.
*   A few methods such as Worksheet.CopyConditionalFormatting & Workbook.CheckWriteProtectedPassword have obsoleted some releases back. Now they have been completely removed from the public API.
*   The Workbook.RemoveDigitallySign method has been renamed to Workbook.RemoveDigitalSignature.
*   The factory methods such as CellsHelper.setFontDir & setFontDirs have been marked obsoleted whereas the alternative approach has been exposed via FontConfigs class as detailed above.
*   A few of the properties from Shape class has been marked obsolete whereas alternative properties have been exposed. For instance, the Shape.FillFormat & Shape.LineFormat properties have been replaced by Shape.Fill & Shape.Line properties respectively.
*   The ShapeFont class has been replaced by the TextOptions class whereas the FontSetting.ShapeFont property has been replaced by the FontSetting.TextOptions.




[1]: https://downloads.aspose.com/cells/androidjava
[2]: https://docs.aspose.com/display/cellsjava/Configuring+Fonts+for+Rendering+Spreadsheets
[3]: https://docs.aspose.com/display/cellsjava/Decrease+the+Calculation+Time+of+Cell.Calculate+method
[4]: https://docs.aspose.com/display/cellsjava/Get+or+Set+the+Class+Identifier+of+the+Embedded+OLE+Object
[5]: https://docs.aspose.com/display/cellsjava/Change+Data+Source+of+the+Chart+to+Destination+Worksheet+while+Copying+Rows+or+Range
[6]: https://docs.aspose.com/display/cellsjava/Provide+exported+worksheet+html+file+path+via+IFilePathProvider+interface
[7]: https://docs.aspose.com/display/cellsjava/Set+the+Comment+of+Table+or+List+Object
[8]: http://docs.aspose.com/display/cellsjava/Update+ActiveX+ComboBox+Control
[9]: http://docs.aspose.com/display/cellsjava/Find+if+Data+Points+are+in+the+Second+Pie+or+Bar+on+a+Pie+of+Pie+or+Bar+of+Pie+Chart
[10]: http://docs.aspose.com/display/cellsjava/Set+text+of+chart+legend+entry+fill+to+none+using+Aspose.Cells
[11]: http://docs.aspose.com/display/cellsjava/Specify+whether+the+PivotTable+is+compatible+for+Excel2003+while+refreshing+PivotTable
[12]: http://docs.aspose.com/display/cellsjava/Support+the+layout+of+DIV+tags+while+loading+html+to+excel+workbook




