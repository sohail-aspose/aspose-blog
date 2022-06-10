---
title: 'Support for ActiveX Controls in Spreadsheets with Aspose.Cells for Android 8.9.0'
date: Fri, 29 Jul 2016 06:32:32 +0000
draft: false
url: /2016/07/29/support-for-activex-controls-filter-data-type-while-loading-spreadsheets-customize-calculation-engine-with-aspose.cells-for-android-8.9.0/
author: Babar Raza
summary: ''
tags: ['ActiveX controls', 'Android APIs', 'Android APIs for Excel Formats', 'Chart2PDF', 'Filtered Content Loading', 'Manipulate Spreadsheets in Android']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Android_100.png" alt="Aspose.Cells for Android logo">}}


We are pleased to announce the release of [Aspose.Cells for Android 8.9.0][1]. This release includes a number of new features, enhancements and bug fixes that further improve the overall stability and usability of the API. Please check the release notes in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Android. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the Public API Changes section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Work with ActiveX Controls in Spreadsheets

Aspose.Cells APIs have provided the ability to add & manipulate the ActiveX Controls in spreadsheets. Aspose.Cells for Android API has exposed a number of useful classes, enumerations and methods to fully support the ActiveX Controls. The most worth mentioning addition to the public API is the ShapeCollection.addActiveXControl method which allows to add an ActiveX Control to the collection of shapes by accepting 7 parameters to specify the control type, location to place the control and size of the control. The control type can be specified using the ControlType enumeration with following possible values.

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

Below provided code snippet demonstrates the simple usage scenario of newly exposed ShapeCollection.addActiveXControl method to add an ActiveX Control of type Toggle Button. Please check the detailed article on [Adding ActiveX Controls to Worksheets][2] if you wish to get more in-depth understanding of the aforementioned feature.

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-AddActiveXControl-AddActiveXControl.java" >}}

## Filter the Data Type for Loading

As per default behaviour, Aspose.Cells APIs load everything from the template file into its own object model, providing access to every aspect of the spreadsheet. There could be scenarios where the user does not want to load everything but specific objects, such as charts or shapes. This can be achieved using the newly exposed LoadDataFilterOptions enumeration and LoadOptions.LoadDataFilterOptions property.

Aspose.Cells APIs have added the enumeration LoadDataFilterOptions which can be used to make the selection of data type to be loaded from the template file. Filtering data at the time of loading can improve the performance tremendously, especially when used with LightCells APIs. There are several selections that a user can make in order to customize the loading process by specifying the appropriate value from LoadDataFilterOptions.

The LoadDataFilterOptions enumeration provides the following selections.

*   ALL to load everything from the spreadsheet.
*   NONE to load nothing from the spreadsheet.
*   CELL\_BLANK loads the cells whose values are blank.
*   CELL\_BOOL loads cells whose values are Boolean.
*   CELL\_DATA loads cells data including values, formulas and formatting.
*   CELL\_ERROR loads cells whose values are error.
*   CELL\_NUMERIC loads cells whose values are numeric (including Date & Time).
*   CELL\_STRING loads cells whose values are text/string.
*   CELL\_VALUE loads only cell values (all types).
*   CHART loads only charts.
*   CONDITIONAL\_FORMATTING loads only conditional formatting rules.
*   DATA\_VALIDATION loads only data validation rules.
*   DOCUMENT\_PROPERTIES loads only document properties.
*   FORMULA loads formulas including defined names.
*   MERGED\_AREA loads only merged cells.
*   PIVOT\_TABLE loads Pivot Tables.
*   SETTINGS loads only Workbook & Worksheet settings.
*   SHAPE loads only shapes.
*   STYLE loads cells formatting.
*   TABLE loads Excel tables/List Objects.

Here is the simple usage scenario to demonstrate the [Data Filtering at the time of Template Loading][3].

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-TechnicalArticles-FilterDataWhileLoadingWorkbook-1.java" >}}

## Update References while Deleting Blank Rows & Columns

As per default behavior, Aspose.Cells APIs delete the blank rows & columns without updating the cell references that may have been affected by the delete process. This could lead to undesired results in certain cases, especially when the spreadsheet contains formulas or charts.

Aspose.Cells APIs have tried to overcome the aforementioned situation by exposing the overloaded versions of the Cells.deleteBlankRows & Cells.deleteBlankColumns methods with the release of Aspose.Cells for Android. The new methods can accept an instance of DeleteOptions class and can be used to overcome the situations that could arise due to the broken references in formulas, chart series data, and so on. The DeleteOptions class currently has one member, a Boolean type property by the name UpdateReference. If the said property is set to true and the instance of DeleteOptions class is passed to the Cells.deleteBlankRows & Cells.deleteBlankColumns methods, the API will internally adjust the formula references (if any) to accommodate the changes.

Below provided code snippet demonstrates the simple usage scenario of newly exposed overloads. If you wish to get more understanding where these methods should be used, please check the detailed article on [Updating Cell References while Deleting Blank Rows & Columns][4].

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-main-java-com-aspose-cells-examples-worksheets-management-Updatereferencesinotherworksheetswhiledeletingblankcolumnsandrowsinworksheet-1.java" >}}

## Render Grid Lines to HTML

Aspose.Cells APIs provide the ability to export spreadsheet contents in HTML format as per the standards opted by Excel application. If a spreadsheet is converted to HTML using Excel application, it does not render the grid lines. Aspose.Cells APIs behave in the same way using its default settings, however, with this release of the API, the developers can now choose to render the grid lines as well. Aspose.Cells for Android API has exposed the HtmlSaveOptions.ExportGridLines property with default value of false. If the said property is set to true, the API renders the grid lines for the available data range in HTML format.

Below provided code snippet demonstrates the simple usage scenario of newly exposed HtmlSaveOptions.ExportGridLines to render the grid lines to HTML format. In order to get a more detailed understanding of this feature, please check the article on [Rendering Grid Lines to HTML][5].

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-ExportExceltoHTML-ExportExceltoHTML.java" >}}

## Auto Refresh OleObject's Image

Aspose.Cells for Android has exposed the OleObject.AutoLoad property which allows to refresh the OleObject's image if the contents/data of the underlying object has been changed. The aforementioned property when set to true, forces the Excel application to refresh the OleObject's image when resultant spreadsheet is loaded in Excel interface.

Below provided code snippet demonstrates the simple usage scenario of newly exposed OleObject.AutoLoad property. In order to get a more detailed understanding of this feature, please check the article on [Automatically Refresh OleObect's Image][6].

## Add Comments for ListObjects

Aspose.Cells APIs now allow to get and set the comments for an instance of ListObject. In order to provide the aforementioned feature, the Aspose.Cells APIs have exposed the ListObject.Comment property with the release of 8.8.3.

Here is a simple usage scenario of newly exposed ListObject.Comment property. In order to get detailed understanding of this feature, please check the article on [Adding Comments for ListObjects][7].

## Set Default Font for Rendering Spreadsheets to Image Formats

Aspose.Cells for Android API has provided the ability to specify the default font name for rendering the spreadsheets in image formats by exposing the ImageOrPrintOptions.DefaultFont property. The DefaultFont property is of type System.string with default value as null. The said property can be used when Unicode characters in the spreadsheet have not been formatted with appropriate font in the cell's style, consequently such characters may appear as blocks in the resultant images. It is advised to set the DefaultFont property to MingLiu or MS Gothic to properly show the Unicode characters in the resultant images. If the DefaultFont property is not set, Aspose.Cells for Android API will use the system's default font to show the Unicode characters.

Below provided code snippet demonstrates the simple usage scenario of newly exposed ImageOrPrintOptions.DefaultFont property. Please check the detailed article on [Setting Default Font for Rendering Spreadsheets in Image Formats][8] if you wish to get more in-depth understanding of the aforementioned feature.

## Set Default Font for Rendering Spreadsheets to HTML

Aspose.Cells for Android 8.9.0 has exposed the DefaultFontName property for the HtmlSaveOptions class that allows to specify the default font name while rendering spreadsheets to HTML format. The default font will be used only when a particular font used to style some contents in the spreadsheet does not exist on the machine where conversion process has to take place. The default value of HtmlSaveOptions.DefaultFontName property is null that means, Aspose.Cells for Android API will use the universal font which has the same family with the original font.

Below provided code snippet demonstrates the simple usage scenario of newly exposed HtmlSaveOptions.DefaultFontName. In order to get a more in-depth  understanding of this feature, please check the article on Setting Default Font for Rendering Spreadsheets to HTML Format.

## Impose Restrictions of Excel 2003 while Refreshing Pivot Table

Aspose.Cells for Android API has exposed the Boolean type IsExcel2003Compatible property for the PivotTable class which allows to impose or remove the Excel 2003 restrictions for refreshing Pivot Tables. The default value of IsExcel2003Compatible property is true, that means a string must be less than or equal to 255 characters. If the string is greater than 255 characters, it will be truncated. If false, the aforementioned restriction will not be imposed.

Below provided code snippet demonstrates the simple usage scenario of PivotTable.IsExcel2003Compatible property. In order to get a more detailed understanding of this feature, please check the article on [Compatibility for Excel 2003 while Refreshing Pivot Tables][9].

## Setting Shadow as Text Effect for Shapes

Aspose.Cells for Android now provides the ability to set the shadow as text effects for any shape such as TextBox. The said feature has been provided by exposing the Shape.TextBody property. This property presents the settings of the shape's text and returns FontSetting objects which in turn can be used to set the shadow via ShadowEffect.PresetType property.

Here is the simple usage scenario demonstrating [how to set the shadow effect for the text in a TextBox][10].

## Other Enhancements & Improvements

The most notable enhancements in this release are as follow:

*   Ability to directly calculate the custom functions without inserting the function in worksheet.
*   Ability to export DataBar, ColorScale and IconSet of conditional formatting to HTML format.
*   Ability to render Unicode Supplementary Characters in PDF.
*   Refresh & recalculate the Pivot Tables having calculated items.
*   Specify text spacing for shapes using ShapeFont.Spacing property.
*   Load spreadsheets without importing charts.
*   Support to parse inner DIV tags while importing HTML.
*   Hide & show legend entry's text.
*   Load spreadsheet with specific paper size.
*   Set line spacing & text alignment for paragraphs in shapes.




[1]: http://www.aspose.com/downloads/cells/android/new-releases/aspose.cells-for-android-8.9.0/
[2]: https://docs.aspose.com/display/cellsjava/Add+ActiveX+Controls+using+Aspose.Cells
[3]: https://docs.aspose.com/display/cellsjava/Filtering+the+kind+of+data+while+loading+the+workbook+from+template+file
[4]: https://docs.aspose.com/display/cellsjava/Update+references+in+other+worksheets+while+deleting+blank+columns+and+rows+in+a+worksheet
[5]: https://docs.aspose.com/display/cellsjava/Export+Excel+to+HTML+with+GridLines
[6]: http://docs.aspose.com/display/cellsjava/Automatically+refresh+OLE+object+via+Microsoft+Excel+using+Aspose.Cells
[7]: https://docs.aspose.com/display/cellsjava/Set+the+Comment+of+Table+or+List+Object
[8]: https://docs.aspose.com/display/cellsjava/Set+Default+Font+while+rendering+spreadsheet+to+images
[9]: https://docs.aspose.com/display/cellsjava/Get+Pivot+Table+refresh+date+and+refresh+by+who+information
[10]: http://docs.aspose.com/display/cellsjava/Setting+Shadow+of+Text+Effects+of+Shape+or+TextBox




