---
title: 'Java Excel to TIFF - Track Conversion Progress with Aspose.Cells for Java'
date: Thu, 21 Nov 2019 01:56:14 +0000
draft: false
url: /2019/11/21/track-conversion-progress-with-aspose.cells-for-java-19.10/
author: Ahsaniqbal
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose_cells-for-java-e1558954178996.jpg" alt="This image has an empty alt attribute; its file name is aspose_cells-for-java-e1558954178996.jpg">}}


We are happy to share the release of the latest version of Aspose.Cells for Java v19.10 having a long-awaited feature of tracking the conversion progress of huge files. This is not the end of features in this release as it also supports custom data sorting for the specific area in PivotTable report and provides [Workbook.ContentTypeProperties.Add][1] method to add custom ContentTypeProperties to an excel file. Many other enhancements and bug resolutions are there in this release. You may get complete details of enhancements, new features and bugs resolution in the [release notes][2]. Just download the latest release and start testing the exciting features in [Aspose.Cells for Java v19.10][3]. Following is a brief overview of this new release.

## Convert Excel to Image - Track Conversion Progress

Converting large Excel files to other formats is quite common, however, if it takes a long time, then you may want to provide some indication to the user about the progress of this conversion. Many users demanded this feature and we were working on its support. The wait is over as this new release has provided this feature where an interface [IPageSavingCallback][4] is provided to support tracking of the conversion. A custom class is to be written where the methods [PageStartSaving][5] and [PageEndSaving][6] provided by the IPageSavingCallback are to be implemented. Control is also provided for the conversion of each page in the document. In this case, you may skip some page or put a limit on the number of pages during the conversion. For the demonstration of this feature, you may download the source excel file and use it with the following sample code where conversion progress is shown by displaying messages on the console.

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-LoadingSavingConvertingAndManaging-DocumentConversionProgressForTiff-1.java" >}}

The following is the code for the _TestTiffPageSavingCallback_ custom class.

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-LoadingSavingConvertingAndManaging-DocumentConversionProgressForTiff-2.java" >}}

Console output



{{< figure align=center src="images/Capture-1024x288.png" alt="">}}


Visit the following article for more information and sample files.

*   [Tracking the progress of Excel to image conversion][7]

## Customize Data Sorting in Pivot Table Report for a Specific Area

Pivot tables can provide rich information with little effort. Sometimes we may require to sort a pivot table on field values. For this purpose pivotField.setAutoSortField() function can be used where you have to provide the index of the item to be sorted. This will provide you with a lot of new representation of data for analysis and reporting. A sample code is provided here where usage os this function is demonstrated. Sample files are also provided in this article which can be used to for testing.

*   [Customizing the sorting of Pivot Table][8]



{{< figure align=center src="images/Screenshot-2019-11-20-at-6.16.33-PM-1-1024x574.png" alt="">}}


If you follow this example you will observe that an Excel file is loaded and three pivot tables are added into it. The pivot table at top is added such that no sorting is done in it. In the second pivot table sorting is down for row field values "SeaFood". In the third table sorting the column field values ( "28/07/2000") is demonstrated.  

## Using the Content-Type Properties 

Custom properties can be added in an Excel file along with the default properties like tag, title and size etc. This can assist in searching specific files or grouping different type of files for a specific purpose. The option is also provided to mark some property as optional such that user is not enforced to provide value for some property. For adding a property you may use [Workbook.ContentTypeProperties.Add][9] and for setting a property optional set the value of [ContentTypeProperty.IsNillable][10] as true. In the following sample code, this new feature is demonstrated along with the image showing its effect.

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-Workbook-WorkingWithContentTypeProperties-1.java" >}}



{{< figure align=center src="images/Capture-1.png" alt="">}}


Review the following article to get more details and sample files:

*   [﻿Working with ContentTypeProperties][11]

## Other Enhancements

*   An issue was reported about the performance of calculateFormula(). This issue is resolved by implementing more robust logics covering maximum scenarios.
*   While converting Excel file to PDF, Pivot table data colouring and formatting was not rendering properly. This issue is resolved now.
*   We have improved our product for conversion to PDF like keeping the similar layout as in the source Excel file, appropriate space between the widgets and exact size of images.
*   A bug is removed like Cell.getStyle.getCustom was returning the wrong format for German locale but now the correct value is returned.
*   Exception ArrayIndexOutOfBoundsException while loading the Excel file is removed.

So we are done for now and take your time to try all these new features. Use the following resources to get more information and sample code for testing this latest release.

*   [Developer's Guide][12]
*   [Code Samples][13]
*   [Forums﻿][14]




[1]: https://apireference.aspose.com/java/cells/com.aspose.cells/contenttypepropertycollection#add(java.lang.Object)
[2]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+19.10+Release+Notes
[3]: https://downloads.aspose.com/cells/java/new-releases/aspose.cells-for-java-19.10/
[4]: https://apireference.aspose.com/java/cells/com.aspose.cells/IPageSavingCallback
[5]: https://apireference.aspose.com/java/cells/com.aspose.cells/ipagesavingcallback#pageStartSaving(com.aspose.cells.PageStartSavingArgs)
[6]: https://apireference.aspose.com/java/cells/com.aspose.cells/ipagesavingcallback#pageEndSaving(com.aspose.cells.PageEndSavingArgs)
[7]: https://docs.aspose.com/display/cellsjava/Track+Conversion+Progress+of+Excel+to+TIFF
[8]: https://docs.aspose.com/display/cellsjava/Custom+sorting+in+Pivot+Table
[9]: https://apireference.aspose.com/java/cells/com.aspose.cells/contenttypepropertycollection#add(java.lang.Object)
[10]: https://apireference.aspose.com/java/cells/com.aspose.cells/contenttypeproperty#IsNillable
[11]: https://docs.aspose.com/display/cellsjava/Working+with+ContentTypeProperties
[12]: https://docs.aspose.com/display/cellsjava/Developer+Guide
[13]: https://github.com/aspose-cells/Aspose.Cells-for-Java
[14]: https://forum.aspose.com/c/cells




