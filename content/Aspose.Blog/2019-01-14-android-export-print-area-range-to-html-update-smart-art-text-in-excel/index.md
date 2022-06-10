---
title: 'Export Print Area Range to HTML and Update Smart Art Text in Excel Worksheets in Android'
date: Mon, 14 Jan 2019 18:28:03 +0000
draft: false
url: /2019/01/14/android-export-print-area-range-to-html-update-smart-art-text-in-excel/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Android_100-e1539021448359.png" alt="">}}


We are pleased to announce the release of [Aspose.Cells for Android via Java 18.12][1]. This release includes some new features, enhancements, and other bug fixes that further improve the overall stability and usability of the API. For easy access and utilization, Aspose.Cells for Android via Java APIs can be directly installed from the Maven repository, see the [document][2] for your reference. Please check the [release notes][3] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Android via Java. While you are downloading the latest build, here is a quick look at the most worth mentioning features in this release.

## Export Print Area Range to HTML

We can convert a worksheet to HTML but rendering the entire sheet at once may not be required always. You may require just a selected area of the sheet to be rendered to HTML. Worksheets contain page setup where the print area can be set. There was a need that only this print area shall be rendered to HTML if required. HtmlSaveOptions is extended by adding a new enumerator ExportPrintAreaOnly which enables users to render only print area in the HTML.

For a working example refer to the following article:

*   [Replace tag with text in a textbox inside the worksheet][4]

## Update Smart Art Text

Smart art is used for better representation of information however earlier the text in the smart art shapes was fixed. This limitation is gone now as now smart art text can be updated. For this purpose shape.setText() function is introduced which sets the new text in the smart art shape.

For a working example refer to the following article:

*   [Replace smart art text][5]

## Scalable Column Width

Depiction of data through the HTML page is very common, however, this page can be opened in a variety of devices including mobiles, tabs, and other handheld devices that contain small screens. The size of the columns is defined in "pt" which works in many cases. However, there can be case where this fixed size may not be required. For example, if the container panel width is 600px where this HTML page is being displayed. In this case, you may get a horizontal scrollbar if the generated table width is bigger. This requirement is addressed by providing scalable units like em or percent for a better presentation.

For a working example refer to the following article:

*   [Set column width to scalable unit like em or percent][6]

## Support to Handle Self-Closing Tags in HTML

Empty tags are very common while working with HTML like we can face <td></td> or simply <td/>. Earlier self-closing tags were not supported however now this support is provided. Now you can load any HTML with self-closing tags and convert it to an Excel file.

For a working example refer to the following article:

*   [Recognise self closing tags][7]

## Support for German Locale in Named Range Formulae

Named regions can have English formulae and this file can be used in environments where systems are configured to German Locale. There is a need to translate these English formulae completely to the German language for correct usage in Excel configured for the German language. This feature is fully functional and can be used without any extra coding.

For a working example along with a template file refer to the following article:

*   [Support German Locale in Named range formulae][8]

## Custom Filter with BeginsWith and EndsWith

Excel provides custom filters like filter rows which begins with and ends with some specific string. This feature is available in Aspose.Cells and demonstrated by providing working examples.

For a working example refer to the following article:

*   [Data filtering with custom filter BeginsWith][9]
*   [Data filtering with custom filter EndsWith][10] 

## Get Connection Points from Shapes 

Aspose.Cells provide rich features to manage shapes in the spreadsheet. Sometimes there is a need to get the connection points of a shape for aligning or placing the shapes at the appropriate place. For this purpose, all the connection points are required. The following code can be used to get the list of connection points of a shape where Shape.GetConnectionPoints() function is used.

For a working example refer to the following article:

*   [Get connection points from shape][11]

## Pivot Table Refresh Date/Time and Refreshed By Information

Pivot tables are very common reports which are present in the workbooks. These reports are updated time by time and it is important to know the last time when the report was updated for better decision making. Aspose.Cells has provided this feature by introducing property RefreshDate. Similarly, name of the person who updated the pivot table is also provided as property RefreshedByWho. 

For a working example refer to the following article:

*   [Get PivotTable refresh date and refreshed by who information][12]

## Data Validation for Huge Numbers

Data validation is done in a variety of ways to control the input in the Excel file. Like limit can be defined for a cell within which some number can be entered, otherwise, an error message is raised. Issues were faced for validation of large numbers like 12345678901 etc. in the past but now these much large numbers are supported by Aspose.Cells.

For a working example along with a template file refer to the following article:

*   [Data validation for large numbers][13]

## Rendering Active Worksheet in a Workbook to SVG

Aspose.Cells has introduced rendering active worksheet in a workbook to SVG. For this purpose load an Excel file into the workbook object and set the active sheet index like for Sheet2, set index to 1. Then save the Workbook as SVG which will render active worksheet to SVG:

For a working example refer to the following article:

*   [Rendering active worksheet in a workbook][14]

## Export Single Sheet Workbook to HTML

The workbook can have multiple sheets that are rendered as multiple tab pages when converted to HTML using Excel. Similarly, if a workbook contains a single sheet, it shows one tab page when converted to HTML using Excel. This conversion was working fine for multiple sheets while using Aspose.Cells. However, for a single sheet workbook, there was no tab page and only HTML file was created without creating a separate folder containing CSS. Now Aspose.Cells has enhanced its library to create similar output for single sheet workbooks as compared to output created by Excel.

For a working example refer to the following article:

*   Export single sheet workbook to HTML

## Load Workbook Efficiently Without Loading VBA Project

In complex Excel files (XLSM/XSLB) there can be a large number of macros which can be very very long. Many times there is a need to load the workbooks without loading these VBA projects like just extracting the sheet names from loaded workbook. In this case, we need a filter that can load VBA projects in when they are actually required. This time Aspose.Cells has introduced a filter option LoadDataFilterOptions.VBA which can be used for this purpose.

For a working example refer to the following article:

*   [Filter VBA Project while loading a workbook][15]

## Replacing Tags in Textbox within a Worksheet

The textbox is very common control which can be used in a worksheet. This is not necessary that text in the textbox is fixed. It may have tags that can be replaced with some text at runtime. It helps users to configure the controls as per the data on the sheet or from some other source. Worksheet.replace can be used for this purpose and textbox can be set with the desired text.  

For a working example refer to the following article:

*   [Replace tag with text in a textbox inside the worksheet][16]

## Identification of Validation as Dropdown

A worksheet can have different types of validations including dropdown. There can be a need where user may want to detect the type of validation and take some decision based on this information. Validation object can be obtained from a cell and a new function is defined for this validation which returns if validation is a dropdown or not. Use this function as Validation.getInCellDropDown() which returns a boolean value i.e. true or false.

For a working example refer to the following article:

*   [Check if validation in cell is dropdown][17]

## Aspose.Cells for Android via Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Android via Java API][18].
*   [Aspose.Cells for Android via Java Download Section][19].
*   [Aspose.Cells for Android via Java Documentation][20] – up-to-date documentation containing Programmer's Guide, Knowledge Base, and much more.
*   [Aspose.Cells for Android via Java API Reference Guide][21] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][22] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][23] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes, and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Android via Java Examples][24] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://artifact.aspose.com/repo/com/aspose/aspose-cells/18.12/
[2]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Android+via+Java+Installation#Aspose.CellsforAndroidviaJavaInstallation-InstallAspose.CellsforAndroidviaJavafromMavenRepository
[3]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Android+via+Java+18.12+Release+Notes
[4]: https://docs.aspose.com/display/cellsjava/Replace+tag+with+text+in+a+textbox+inside+the+Worksheet
[5]: https://docs.aspose.com/display/cellsjava/Replace+text+in+smart+art
[6]: https://docs.aspose.com/display/cellsjava/Set+column+width+to+scalable+unit+like+em+or+percent
[7]: https://docs.aspose.com/display/cellsjava/Recognise+self+closing+tags
[8]: https://docs.aspose.com/display/cellsjava/Support+for+German+Locale+in+Named+Range+Formulae
[9]: https://docs.aspose.com/display/cellsjava/Data+Filtering#DataFiltering-CustomfilterwithBeginsWith
[10]: https://docs.aspose.com/display/cellsjava/Data+Filtering#DataFiltering-CustomfilterwithEndsWith
[11]: https://docs.aspose.com/display/cellsjava/Get+Connection+points+from+shape
[12]: https://docs.aspose.com/display/cellsjava/Get+Pivot+Table+refresh+date+and+refresh+by+who+information
[13]: https://docs.aspose.com/display/cellsjava/Data+Validation#DataValidation-DataValidationRules
[14]: https://docs.aspose.com/display/cellsjava/Converting+Worksheet+to+Different+Image+Formats#ConvertingWorksheettoDifferentImageFormats-Renderactiveworksheetinaworkbook
[15]: https://docs.aspose.com/display/cellsjava/Filter+VBA+Project+while+loading+a+workbook
[16]: https://docs.aspose.com/display/cellsjava/Replace+tag+with+text+in+a+textbox+inside+the+Worksheet
[17]: https://docs.aspose.com/display/cellsjava/Data+Validation#DataValidation-Checkifvalidationincellisdropdown
[18]: https://www.aspose.com/products/cells/android-java
[19]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-cells/18.6/
[20]: https://docs.aspose.com/display/cellsandroidjava/Aspose.Cells+for+Android+via+Java+Home
[21]: https://apireference.aspose.com/java/cells
[22]: https://forum.aspose.com/c/cells
[23]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/
[24]: https://github.com/asposecells/Aspose_Cells_Java




