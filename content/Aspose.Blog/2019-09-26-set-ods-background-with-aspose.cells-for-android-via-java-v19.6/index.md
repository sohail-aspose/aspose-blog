---
title: 'Set ODS Background with Aspose.Cells for Android via Java v19.6'
date: Thu, 26 Sep 2019 18:17:18 +0000
draft: false
url: /2019/09/26/set-ods-background-with-aspose.cells-for-android-via-java-v19.6/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Android_100-e1539021448359.png" alt="">}}


We are thrilled to present you all the exciting features, improvements and other fixes of [Aspose.Cells for Android via Java v19.6][1]. The new release includes new features, enhancements and other bug fixes that further improve the overall stability and usability of the Android API. You may check the [release notes][2] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Android via Java. Let us start reviewing what is there in this release.

## Read Background Information from ODS File

This time we have enhanced the capability of Aspose.Cells to process ODS files. One of the features which were requested by users was to read the background information from the ODS files. A new class ODSPageBackground is introduced which manages the background of an ODS file. Moreover, there are two options as the background of an ODS file, one is graphics and other is color. For this purpose, ODSPageBackgroundType enumerator is introduced which contains three values NONE, COLOR and GRAPHIC.

For depicting the position of the background content, there are nine possible locations on the page. These are defined by introducing an enumerator named ODSPageBackgroundGraphicPositionType. Now you can not only identify the type and position but also can save the graphic to a file if required. All these features can be exercised using a ready to run code along with a sample file in the following article:

[Read Background Information from OSD file][3]

Following is the image showing the input and output using these features:



{{< figure align=center src="images/RetrieveImage.png" alt="">}}


## Set Background Color

As mentioned earlier that we have two options to set the background of an ODS file. Here I will describe the colored background for which you have to use ODSPageBackground.Color property. Coding this feature is quite simple such that first get the ODSPageBackground object from the template file and then set color and type and that's all. Have a look at the following article which provides a complete working sample code to demonstrate this feature.

[Add colored background to ODS file][4]

Following is the image of output file created by above sample code:



{{< figure align=center src="images/ODSView-1024x222.png" alt="">}}
</li></ul></figure>

Note that there is no need to set the range of text as this feature will automatically set background for the entire data in the above example.  

## Set Background Graphics

Setting a graphical background is quite common while working with worksheets. This area is also covered by this new feature where property ODSPageBackground.GraphicData is available to serve this purpose. Visit the following article which demonstrates this feature. You can see that usage is quite simple where you need to set the background type, byte array containing image data and ODSPageBackgroundGraphicType. You may visit the following article to get a working code sample for this feature:

[Add Graphic Background to ODS file][5]

Following will be the output of this sample code in the print preview using OpenOffice Calc.



{{< figure align=center src="images/GraphicsBackground-2-1024x246.png" alt="">}}


## Import Custom Objects to Merged Area

The feature of importing custom objects to Excel file is already available in Aspose.Cells, however, if the destination file contains a merged area where data is to be imported, there can be issues. This feature is available now where you can import data to a merged area in the output file. You may set ImportTableOptions.CheckMergedCells to true and Pass the ImportTableOptions object along with the list of columns/properties to the method to display your desired list of objects. Visit the following article for a detailed example:

[Importing from Custom Objects to merged area][6]

Following image provides an overview of this feature:



{{< figure align=center src="images/CustomToMerge.png" alt="">}}


## Support for SXC and FODS

We always try to provide features which are supported by other spreadsheet handling software. Many users demanded support of SXC and FODS file types which are very common. So, here we are with the support of these file types in the latest release. Following is a brief description of these types along with the detail of their support in Aspose.Cells.

### SXC Files

Spreadsheet created by StarOffice Calc; supports formulas, functions, charts, and macros; also includes DataPilot tables, which can automatically extract and summarize data from raw data sets. SXC files are also compatible with Apache OpenOffice Calc and can be exported in Microsoft Excel or IBM Lotus 1-2-3 formats.

### FODS Files

Spreadsheet saved in the OpenDocument format, but stored as a flat XML file instead of the [.][7].ZIP container used by .ODS files; allows the spreadsheet information to be more human readable; also can be an easier alternative than the ODS format for generating spreadsheets automatically without needing a spreadsheet editor.

### Features provided by Aspose.Cells  

#### Generate file

You can generate SXC and FODS file using FileFormatType as argument in Workbook contructor i.e. use FileFormatType.SXC and FileFormatType.FODS as argument.

#### Load file

These files can be loaded using enumerator LoadFormat as follows:

**SXC File**

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-Files-Handling-OpeningSXCFiles-1.java" >}}

**FODS File**

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-Files-Handling-OpeningFODSFiles-1.java" >}}

#### Save File

Saving file of these types is quite easy by using SaveFormat enumerator while calling the Workbook.save() function with second argument as SaveFormat.SXC and SaveFormat.FODS.

## Enhancements

### Handling Excel file with large conditional formatting

While converting Excel files having large conditional formatting to PDF, sometimes there was an "Out of memory" exception. This exception is handled successfully now.

### Maintaining data format while saving Excel file

Excel files can have different data formatting settings along with the conditional formatting. An issue was reported about showing value with fraction instead of whole number. This type of issues are handled and now data formats are maintained while saving the Excel files.

### Improve reading Excel 95 files

Excel 95 files are still very common and need to be handled error-free while using Aspose.Cells. Sometimes an exception was raised as java.lang.NullPointerException for these files. This issue is removed now and Excel 95 files can be loaded without any issue.

### Enhance loading speed after deleting columns

A case was reported where after deleting the columns from an existing file and saving it on the disc, loading was quite slow for this modified file. It is suggested that always take care of the conditional formatting ranges. For these, you should merge them by setting SaveOptions.MergeArea to true before saving them. We have also improved the saving operation and now modified files do not take a long time to load.

## Bugs and Exceptions

Users report bugs and exceptions which are resolved and enhancements are done which improves the usability of the library. Following are few bugs and exceptions which were handled in this release.

*   Conditional formatting can be obtained properly using Cell.getDisplayStyle() after setting different values in the cell containing these conditional formatting based on the cell value. Like foreground colour value which was not obtained correctly earlier in some case can be obtained now.
*   There was an issue where lines were not rendered in the PDF from an Excel file. This issue is resolved and lines are rendered fine. Following is the depiction of the issue for better understanding.



{{< figure align=center src="images/Comparison-1024x764.png" alt="">}}


*   This is common to add images in the header of an Excel file. It was observed that in some cases, the output file after adding these images, was corrupted and could not be opened in Excel. This issue is resolved and now images can be added without any problem.
*   Filters should be maintained while opening and saving a file. A user faced an error that filter was lost after saving the file. Similarly in another case filters were changed. This is no more an issue now.
*   A chart was getting flattened in the saved file after loading it. This issue is resolved in the current release.
*   While loading an ODS file an exception _"Invalid "'""("Based on Name "test\_name)_ was observed. This issue is resolved.
*   A user reported that he is getting exception while calling Name.getRefersTo() function. This issue is resolved in this release.

## Useful Links

The resources, you might need to accomplish your tasks:

*   [Home of Aspose.Cells for Android via Java API][8].
*   [Aspose.Cells for Android via Java Download Section][9].
*   [Aspose.Cells for Android via Java Documentation][10] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Android via Java API Reference Guide][11] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][12] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][13] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Android via Java Examples][14] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://artifact.aspose.com/repo/com/aspose/aspose-cells/19.6/
[2]: https://docs.aspose.com/cells/java/aspose-cells-for-android-via-java-19-6-release-notes/
[3]: https://docs.aspose.com/cells/java/working-with-background-in-ods-files/#WorkingwithBackgroundinODSFiles-ReadBackgroundInformationfromOSDfile
[4]: https://docs.aspose.com/cells/java/working-with-background-in-ods-files/#WorkingwithBackgroundinODSFiles-AddColoredBackgroundtoODSfile
[5]: https://docs.aspose.com/cells/java/working-with-background-in-ods-files/#WorkingwithBackgroundinODSFiles-AddGraphicBackgroundtoODSfile
[6]: https://docs.aspose.com/cells/java/import-and-export-data/#ImportandExportData-ImportingfromCustomObjectstomergedarea
[7]: https://fileinfo.com/extension/zip
[8]: https://products.aspose.com/cells/android-java
[9]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-cells/
[10]: https://docs.aspose.com/cells/androidjava
[11]: https://apireference.aspose.com/java/cells
[12]: https://forum.aspose.com/c/cells
[13]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/
[14]: https://github.com/asposecells/Aspose_Cells_Java




