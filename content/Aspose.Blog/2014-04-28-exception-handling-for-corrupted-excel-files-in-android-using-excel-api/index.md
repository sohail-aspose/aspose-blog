---
title: 'Exception Handling for Corrupted Excel Files in Android'
date: Mon, 28 Apr 2014 14:24:45 +0000
draft: false
url: /2014/04/28/exception-handling-for-corrupted-excel-files-in-android-using-excel-api/
author: Amjad Sahi
summary: ''
tags: ['API', 'Aspose.Cells', 'Aspose.Cells for Java', 'CellsException', 'Excel Files', 'Java API', 'Large Data Sets', 'Large Excel Files', 'Memory Optimization', 'MemorySetting', 'Worksheet', 'cells', 'java', 'spreadsheet']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Android_100.png" alt="Aspose.Cells for Android logo">}}


We are pleased to announce the release of Aspose.Cells for Android 7.0.0 with new features, enhancements, and bug fixes.

There are some valuable features in this month’s release. For a full list of bug fixes and other improvements please refer to the download page.

## Optimize Memory for Existing Worksheets

Aspose.Cells for Android provided memory optimization settings for newly created worksheets by exposing the setMemorySetting method for the Workbook.Settings class. The previously provided approach was useful for minimizing the overall memory cost while working with existing large Microsoft Excel spreadsheets containing huge datasets.

With release 7.0.0, we have enhanced this feature for existing worksheets by exposing a similar method for the Cells class. Now you may use the setMemorySetting method provided by the Cells class to cope with the memory issues for situations where large data sets have to be built-in memory. The setMemorySetting method accepts a parameter of type MemorySetting with the default value NORMAL. In order to properly utilize this newly introduced feature, memory optimization settings have to be explicitly specified for existing worksheets. Please check the detailed technical article on how to [optimize the memory while working with large data sets][1].

## Identify Corrupted Excel Files

We have also enhanced the CellsException class to identify potentially damaged or corrupted files when loaded with the Workbook constructor. With the new enhancements integrated, Aspose.Cells for Android API now throws an error of type CellsException whenever it encounters a damaged file.

## Other Enhancements

Aspose.Cells for Android 7.0.0 has also provided fixes for several important issues. For example, problems with converting Excel files to PDF format, rendering & manipulating charts, retrieving & removing OLE objects. Moreover, we have improved the overall performance as well as the accuracy of results for the formula calculation engine when working with Excel formulas.

To see a complete list of enhancements and fixes and to download Aspose.Cells for Android 7.0.0, please visit the [download page][2].




[1]: https://docs.aspose.com/display/cellsjava/Optimizing+Memory+Usage+while+Working+with+Big+Files+having+Large+Datasets
[2]: https://downloads.aspose.com/cells/androidjava




