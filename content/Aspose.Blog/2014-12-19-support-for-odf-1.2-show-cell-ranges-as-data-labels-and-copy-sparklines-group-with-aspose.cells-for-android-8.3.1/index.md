---
title: 'Support for ODF 1.2, Show Cell Ranges as Data Labels and Copy Sparklines Group with Aspose.Cells for Android 8.3.1'
date: Fri, 19 Dec 2014 09:00:33 +0000
draft: false
url: /2014/12/19/support-for-odf-1.2-show-cell-ranges-as-data-labels-and-copy-sparklines-group-with-aspose.cells-for-android-8.3.1/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for Android logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/06/aspose-Cells-for-Android_100.png)Aspose.Cells for Android 8.3.1 has been released. This release contains some useful features and other improvements. Below, we list some major features and other enhancements in the new release.

## Save ODS File in ODF 1.1 and 1.2 Specifications

Aspose.Cells APIs have extended its support for the OpenDocument Format. Now users can save the ODS (OpenDocument Spreadsheets) in conformance to ODF 1.2 specifications. Aspose.Cells APIs have exposed the methods isStrictSchema11 & setStrictSchema11 for the OdsSaveOptions class to support this feature. The default value of the setStrictSchema11 property is false, which means that from version 8.3.1 of Aspose.Cells, ODS files will be saved as ODF format version 1.2 by default. For more details, please check the article Save ODS file in ODF 1.1 and 1.2 Specifications.

## Insert Values in ListObjects using Row/Column Offset

Normally, you add values inside the ListObject/Table using the Cell.putValue method, however, the putValue method must be associated with an instance of a Cell to identify the correct location where value has to be inserted. This mechanism is not usable when you need to add values inside the ListObject using the row and column offsets. Aspose.Cells for Android 8.3.1 has exposed the methods Cell.getTable & ListObject.putCellValue methods to facilitate the users in Accessing the ListObject from a Cell and Add Values using the Row and Column Offsets.

## Create Sparkline by Specifying Data Range and Location

Aspose.Cells APIs have exposed the SparklineCollection.add(String dataRange, int row, int column) method to Specify the Data Range and Location of Sparkline Group.

## Show Cell Ranges as Data Labels

Aspose.Cells provides the DataLabels.setShowCellRange attribute to select or clear the option **Label Contains - Value From Cells**. For more details, please see the article Showing Cell Range as the Data Labels.

## Other Enhancements and Fixes

Aspose.Cells for Android 8.3.1 has provided fixes and other enhancements for several important issues, such as, reading/writing Microsoft Excel files, calculating formulas, manipulating charts and shapes, sheet to image, chart to image and Excel to PDF bugs, etc.

To see a complete list of enhancements and fixes and to download Aspose.Cells for Android 8.3.1, please visit the [download page][2].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/06/aspose-Cells-for-Android_100.png "Aspose.Cells for Android logo"
[2]: http://www.aspose.com/community/files/74/android-components/aspose.cells-for-android/entry593248.aspx




