---
title: 'Improved AutoFitRows and AutoFitColumns in Aspose.Cells for Android'
date: Wed, 27 Aug 2014 10:27:33 +0000
draft: false
url: /2014/08/27/enhanced-multithreading-support-autofitrows-and-autofitcolumns-features-improved-in-aspose.cells-for-android-8.2.0/
author: Amjad Sahi
summary: ''
tags: ['autofit columns in android', 'autofit rows in android']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Android_100.png" alt="autofitrows autofitcolumns android">}}


Aspose.Cells for Android 8.2.0 has been released. This release contains useful new features and other improvements. Below, we list some major features and other enhancements in this month’s release.

## Extended Support for Multi-Threading Environment

The Aspose.Cells for Android API is useful in a multi-threading environment as in a single thread execution plan. However, recent changes to the core make the API more reliable when reading cell values in multiple threads simultaneously. Aspose.Cells for Android has exposed the MultiThreadReading property for the Cells class in order to make sure that the correct cell values are returned when API works in a multi-threading environment. For more details, have a look at the detailed article on Simultaneously Reading Cell Values with Multiple Threads.

## Add Useful Overloads to autoFitRows and autoFitColumns New Methods

Now you may also use the new overloads we have included to this release - autoFitRows(int startRow, int endRow, AutoFitterOptions options) and autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options) - from the list if you need to auto-fit rows or columns with the desired AutoFitterOptions.

## Bug Fixes

Aspose.Cells for Android 8.2.0 has provided fixes and other enhancements for several important issues, such as reading/writing Microsoft Excel files, calculating formulas, manipulating charts and shapes, sheet to image conversion bugs, etc.

The latest release has some notable enhancements:

*   Enhanced the PDF rendering engine to handle shapes better.
*   Improvements to the core for better handling of embedded OleObjects.

To see a complete list of enhancements and fixes and to download Aspose.Cells for Android 8.2.0, please visit the [download page][1].




[1]: http://www.aspose.com/community/files/74/android-components/aspose.cells-for-android/entry568362.aspx




