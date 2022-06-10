---
title: 'Modify VBA Code, Set PivotTable Layout, Remove PivotTables and Convert DataBars to Images with Aspose.Cells for Android 8.4.0'
date: Wed, 25 Mar 2015 13:56:13 +0000
draft: false
url: /2015/03/25/modify-vba-code-set-pivottable-layout-remove-pivottables-and-convert-databars-to-images-with-aspose.cells-for-android-8.4.0/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for Android logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/06/aspose-Cells-for-Android_100.png)Aspose.Cells for Android 8.4.0 has been released. This release contains many useful improvements and features including the long awaited feature to manipulate VBA code embedded inside the spreadsheets. This release also contains some useful features and other improvements. Below, we list some major features and other enhancements in the new release.

## Access & Modify VBA Code

Many of the Aspose.Cells users had been waiting for this feature, and now it is available with the release of Aspose.Cells for Android 8.4.0. The latest build of the API has exposed a new package and a few classes to provide the means to access the VBA code embedded inside the macro enabled spreadsheets, and to amend the code as per requirement. The details of the newly exposed classes are as follow.

*   VbaProject class can be used to fetch the VBA project from a given spreadsheet.
*   VbaModuleCollection class represents the collection of VBA modules that are part of a given VbaProject.
*   VbaModule class represents a single module from the VbaModuleCollection.

Please see the document on how to access and modify VBA codes via Aspose.Cells APIs for your reference.

## Ability to Remove Pivot Table from Worksheet

Another worth mentioning feature is the support for Pivot Table removal. Aspose.Cells for Android 8.4.0 has provided this feature by exposing two new methods for the PivotTableCollection class that allows to delete a specific PivotTable from the collection depending upon the input parameter.

Here are a few details about the newly exposed methods whereas the code snippets are available in the detailed article as linked above.

*   PivotTableCollection.remove method accepts an object of PivotTable, and removes it from the collection.
*   PivotTableCollection.removeAt method accepts a zero index based integer value and removes the particular PivotTable from the collection.

## Support for Different Pivot Table Layouts

Microsoft Excel has predefined layouts for the Pivot Tables as listed below. Upon choosing any of these layouts, Microsoft Excel formats the Pivot Tables accordingly.

*   Compact Form
*   Outline Form
*   Tabular Form

Aspose.Cells for Android 8.4.0 provides the same functionality while using the newly exposed methods for the PivotTable class that allows to dynamically set the layouts as discussed above. Detailed article and sample code snippets are available at Changing the Layout of Pivot Table.

## Convert DataBars to Images

With the release of v8.4.0, the Aspose.Cells API has provided the DataBar.toImage method to save the conditionally formatted DataBar in image format. The DataBar.toImage method accepts two parameters as detailed below.

*   The first parameter is of type Cell on which conditional formatting has been applied.
*   The second parameter is of type ImageOrPrintOptions in order to set different parameters of the resultant image.

Please see the document on how to generate conditional formatting DataBars' images for your reference.

## Custom Properties for the Document Information Panel

Aspose.Cells can be used to add custom properties inside the workbook object which are visible in the Document Information Panel when accessed through Microsoft Excel using the File > Info > Properties > Show Document Panel menu.

Please see the document on how to add custom properties that are visible inside Document Information Panel for your reference.

## Other Enhancements & Fixes

Aspose.Cells for Android 8.4.0 has provided fixes and other enhancements for several important issues, such as, reading/writing and rendering Microsoft Excel files, calculating formulas, manipulating charts and shapes, sheet to image, chart to image and Excel to PDF bugs, etc.

To see a complete list of enhancements and fixes and to download Aspose.Cells for Android 8.4.0, please visit the [download page][2].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/06/aspose-Cells-for-Android_100.png "Aspose.Cells for Android logo"
[2]: http://www.aspose.com/community/files/74/android-components/aspose.cells-for-android/entry614937.aspx




