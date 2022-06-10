---
title: 'Get Text of Chart Trendline Equation in Excel Spreadsheets in Android'
date: Thu, 27 Nov 2014 17:56:09 +0000
draft: false
url: /2014/11/27/get-text-of-chart-trendline-equation-in-excel-spreadsheets-in-android/
author: Amjad Sahi
summary: ''
tags: ['Get text of chart trendline equation', 'Track and manipulate Workbook file state']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Android_100.png" alt="Aspose.Cells for Android logo">}}


[Aspose.Cells for Android][1] 8.3.0 has been released. This release contains some useful features and other improvements. Below, we list some major features and other enhancements in the new release.

## Get a Chart Trendline Equation Text

Aspose.Cells allows you to retrieve the equation text of a chart trendline. Aspose.Cells provides the Trendline.getDataLabels().getText() method which returns the equation text of a chart's trendline. To make use of this property, first call the Chart.calculate() method.

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-GetEquationText-GetEquationText.java" >}}

Please see the detailed article on [retrieving the equation text of a chart trendline][2].

## Track Workbook State

Aspose.Cells for Android 8.3.0 has added several useful get/set methods that can enable the developers to track & manipulate the Workbook file's state. The aforesaid attributes and their brief descriptions are as follow.

*   WorkbookSettings.getCrashSave: Indicates whether the application last saved the workbook file after a crash.
*   WorkbookSettings.getDataExtractLoad: Indicated whether the application last opened the workbook file for data recovery.
*   WorkbookSettings.getRepairLoad: Provides information if the application last opened the workbook file in safe or repair mode.
*   WorkbookSettings.getAutoRecover: Indicates if auto-recovery has been performed on the Workbook file.

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-SetAutoRecoverProperty-SetAutoRecoverProperty.java" >}}

Please see the detailed article on [setting AutoRecover property of a Workbook][3].

## Other Enhancements and Fixes

Aspose.Cells for Android 8.3.0 has provided fixes and other enhancements for several important issues, such as reading/writing Microsoft Excel files, calculating formulas, manipulating charts and shapes, sheet to the image, chart to image, and Excel to PDF bugs, etc.

To see a complete list of enhancements and fixes and to download Aspose.Cells for Android 8.3.0, please visit the [download page][4].




[1]: https://products.aspose.com/cells/android-java
[2]: https://docs.aspose.com/display/cellsjava/Get+Equation+Text+of+Chart+Trendline
[3]: https://docs.aspose.com/display/cellsjava/How+to+set+AutoRecover+property+of+Workbook
[4]: http://downloads.aspose.com/cells/java




