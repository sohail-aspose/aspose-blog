---
title: 'Work with SXC and FODS Files using Java'
date: Mon, 22 Jul 2019 16:49:39 +0000
draft: false
url: /2019/07/22/handle-sxc-and-fods-files-with-aspose.cells-for-java-19.6/
author: Ahsaniqbal
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

A new version [Aspose.Cells for Java][1] 19.6 is released that handles file types SXC and FODS contains a lot of enhancements and few bug removals. Support for handling file types SXC and FODS is added like you can generate, load and save these files. This release also contains improvements for handling files with large conditional formattings, enhancements in the process of saving Excel files with data formats, filters and chart rendering. You can get the details of all these enhancements and changes in the [release notes][2]. You might be curious about the new features, enhancements and exceptions handled in this release, so let us start to review this release in detail.

## Handle SXC and FODS using Java

We always try to provide features which are supported by other spreadsheet handling software. Many users demanded support of SXC and FODS file types which are very common. So, here we are with the support of these file types in the latest release. Following is a brief description of these types along with the detail of their support in Aspose.Cells.

### SXC Files

Spreadsheet created by StarOffice Calc; supports formulas, functions, charts, and macros; also includes DataPilot tables, which can automatically extract and summarize data from raw data sets. SXC files are also compatible with Apache OpenOffice Calc and can be exported in Microsoft Excel or IBM Lotus 1-2-3 formats.

### FODS Files

Spreadsheet saved in the OpenDocument format, but stored as a flat XML file instead of the [.][3].ZIP container used by .ODS files; allows the spreadsheet information to be more human readable; also can be an easier alternative than the ODS format for generating spreadsheets automatically without needing a spreadsheet editor.

## Generate File SXC and FODS File using Java

You can generate SXC and FODS file using FileFormatType as argument in Workbook contructor i.e. use FileFormatType.SXC and FileFormatType.FODS as argument.

### Load File

These files can be loaded using enumerator LoadFormat as follows:

#### SXC File{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-Files-Handling-OpeningSXCFiles-1.java" >}}

#### FODS File{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-Files-Handling-OpeningFODSFiles-1.java" >}}

### Save File

Saving file of these types is quite easy by using SaveFormat enumerator while calling the Workbook.save() function with second argument as SaveFormat.SXC and SaveFormat.FODS.

## Improvements in this Version

### Handling Excel file with large conditional formatting

While converting Excel files having large conditional formatting to PDF, sometimes there was an "Out of memory" exception in JVM. This exception is handled successfully now.

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

For all the resources, documentation, examples and forum support please visit [here][4].




[1]: https://products.aspose.com/cells/java
[2]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+19.6+Release+Notes
[3]: https://fileinfo.com/extension/zip
[4]: https://products.aspose.com/cells/java




