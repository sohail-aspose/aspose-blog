---
title: 'Adjust Excel Workbook Compression Level using Java'
date: Wed, 30 Oct 2019 01:47:35 +0000
draft: false
url: /2019/10/30/adjust-workbook-compression-level-with-aspose.cells-for-java-19.9/
author: Ahsaniqbal
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose_cells-for-java-e1558954178996.jpg" alt="This image has an empty alt attribute; its file name is aspose_cells-for-java-e1558954178996.jpg">}}


Its great pleasure to share that we have achieved another milestone by publishing new release Aspose.Cells for Java 19.9 that will enable developers to adjust the workbook compression level. Don't worry, this is not the only feature as there are many other enhancements as well including the facility to print multiple copies of a workbook and support for reading and rendering Control of ODS files.  Details of all the new features, enhancements and bugs resolution can be seen in the [release notes][1]. This latest release [Aspose.Cells for Java v19.9][2] can be downloaded from the download section. Let us have a brief look at the salient features of this exciting release.

## Adjust Excel Workbook Compression Level using Java

The compression level of the workbook is an important factor while working with larger workbooks. You should have control over setting the priority to create either small file with little more time or create files quickly but having comparatively large file size. Aspose.Cells have now provided this control such that the developer will have the control to adjust the compression level. A new enumerator [OoxmlCompressionType][3] is provided which can be used to set the compression level. Following members are available under this enumerator. 

*   [LEVEL\_1][4]: The fastest but least effective compression.
*   [LEVEL\_2][5]: A little slower, but better, than level 1.
*   [LEVEL\_3][6]: A little slower, but better, than level 2.
*   [LEVEL\_4][7]: A little slower, but better, than level 3.
*   [LEVEL\_5][8]: A little slower than level 4, but with better compression.
*   [LEVEL\_6][9]: A good balance of speed and compression efficiency.
*   [LEVEL\_7][10]: Pretty good compression!
*   [LEVEL\_8][11]: Better compression than Level7!
*   [LEVEL\_9][12]: The "best" compression, where best means greatest reduction in the size of the input data stream. This is also the slowest compression.

Following example can be used to exercise this new exciting feature by changing the compression type and comparing the file size with the time taken to create this file.

{{< gist aspose-com-gists 439a68a5e4305388c50ca306ef238de5 "Examples-src-AsposeCellsExamples-Workbook-AdjustCompressionLevel-1.java" >}}

## Other enhancements

*   An Excel file having AutoFilter was converted to HTML with HiddenColDisplayType "HtmlHiddenColDisplayType.REMOVE". This was causing an issue that the hidden rows in the Excel file were becoming visible. This issue is resolved and now these rows remain hidden in HTML as well.
*   There was a need to enable the product to support large formulas like issues were observed in the SUM function if there were more than 128 cells. This issue is resolved and now large formulas are supported by Aspose.Cells.
*   A user reported that an XLSX file is loaded and saved back after calling calculateFormula(). Inspecting and comparing `input.xlsx` and `output.xlsx` files, some formulas containing structured references seem to have been broken by Aspose Cells. This issue was corrupting the file and crashing Excel while opening such files. This issue is resolved and there is no more formula corruption by calling calculateFormula() and saving the file.
*   An issue was reported where footer text font and formatting was not maintained while converting the Excel file to PDF. This issue is resolved now and you will get proper font and formatting while converting Excel file to PDF.
*   In another scenario, Workbook.setRecalculateOnOpen(false) is used before saving the Excel file. When this file is opened in Excel 365, it starts calculating the file and hangs. This issue is resolved now and the output file does not hang Excel 365 anymore.
*   An exception was raised while converting XLSM to the image. This is no more an issue now.
*   While working in macOS, an Excel file was converted to PDF, but it was raising an exception that "Column width must be between 0 and 255". Now this issue is resolved and macOS users will face no problem while converting Excel file to PDF.
*   Other issues like "Java.lang.NumberFormatException: For input string: 0.0" and IllegalArgumentException while executing deleteBlankColumns() are also removed. 

The wait is over and you may get ready to test the new features. Following resources may help you to achieve your targets using Aspose.Cells.

*   [Developer's Guide][13]
*   [Code Samples][14]
*   [Forums﻿][15]




[1]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+19.9+Release+Notes
[2]: https://downloads.aspose.com/cells/java/new-releases/aspose.cells-for-java-19.9/
[3]: https://apireference.aspose.com/java/cells/com.aspose.cells/OoxmlCompressionType
[4]: https://apireference.aspose.com/java/cells/com.aspose.cells/ooxmlcompressiontype#LEVEL_1
[5]: https://apireference.aspose.com/java/cells/com.aspose.cells/ooxmlcompressiontype#LEVEL_2
[6]: https://apireference.aspose.com/java/cells/com.aspose.cells/ooxmlcompressiontype#LEVEL_3
[7]: https://apireference.aspose.com/java/cells/com.aspose.cells/ooxmlcompressiontype#LEVEL_4
[8]: https://apireference.aspose.com/java/cells/com.aspose.cells/ooxmlcompressiontype#LEVEL_5
[9]: https://apireference.aspose.com/java/cells/com.aspose.cells/ooxmlcompressiontype#LEVEL_6
[10]: https://apireference.aspose.com/java/cells/com.aspose.cells/ooxmlcompressiontype#LEVEL_7
[11]: https://apireference.aspose.com/java/cells/com.aspose.cells/ooxmlcompressiontype#LEVEL_8
[12]: https://apireference.aspose.com/java/cells/com.aspose.cells/ooxmlcompressiontype#LEVEL_9
[13]: https://docs.aspose.com/display/cellsjava/Developer+Guide
[14]: https://github.com/aspose-cells/Aspose.Cells-for-Java
[15]: https://forum.aspose.com/c/cells




