---
title: 'Set Creation Time in Excel to PDF with Aspose.Cells for Java 8.0.0'
date: Tue, 01 Apr 2014 08:29:41 +0000
draft: false
url: /2014/04/01/memory-usage-optimized-and-set-the-creation-time-in-the-generated-pdf-using-aspose.cells-for-java-8.0.0/
author: Amjad Sahi
summary: ''
tags: ['Calculate Excel formulas', 'export Excel workbooks to PDF', 'improved OOXML API', 'manipulate PivotTables', 'render MS Excel file formats', 'render images files from Charts', 'rendering Charts']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java logo">}}


We are pleased to announce the release of Aspose.Cells for Java 8.0.0 with new features, enhancements and bug fixes. This release supports [optimizing memory usage when working with big Microsoft Excel files with large data sets][1]. When building a workbook with large data sets, or reading a big template file, the total amount of RAM the process will use is always a concern.Aspose.Cells provides measures that can be adopted to cope with the challenge. Aspose.Cells provides some relevant options to lower, reduce and optimize memory usage. For example, the MemorySetting.MEMORY\_PREFERENCE option optimizes memory use for the cells data to decrease the overall memory cost.

Aspose.Cells also allows to get/set the time of generating the PDF documents for [Excel to PDF conversion][2], sometimes you might need to set your desired custom DateTime for the PDF files.

There is another valuable Microsoft Excel's feature is to [show formulas instead of values in a worksheet][3]. You can show formulas instead of the calculated values in Microsoft Excel using the **Show Formulas** option from the **Formulas** ribbon. Once, you enable it, Microsoft Excel displays formulas inside the worksheet. You can achieve this using Aspose.Cells APIs.

Aspose.Cells provides a Worksheet.setShowFormulas() method which you can set to true to set Microsoft Excel to display formulas.

## Enhancements and Fixes

We have added a number of enhancements and fixes to this release. We have also fixed some exceptions which were thrown when reading and writing Excel files and rendering images from worksheets. We have improved the [chart to image][4] and [sheet to image][5] modules and fixed issues with [manipulating charts][6] and shapes as well.

Several other important issues have also been addressed. For example, issues with rendering Excel files to HTML file format, applying formatting, auto-filtering data in List objects/Tables and [exporting Excel workbooks to PDF format][7] have been resolved in this release. A few other improvements are also made to Aspose.Cells for Java's formula calculation engine.

To see a complete list of enhancements and fixes and to download Aspose.Cells for Java 8.0.0, please visit the [download page][8].




[1]: https://docs.aspose.com/display/cellsjava/Optimizing+Memory+usage+while+working+with+Big+Files+having+large+Datasets
[2]: https://docs.aspose.com/display/cellsjava/Converting+Workbook+to+Different+Formats#ConvertingWorkbooktoDifferentFormats-ConvertingExceltoPDF
[3]: https://docs.aspose.com/display/cellsjava/Show+Formulas+instead+of+Values+in+a+Worksheet
[4]: https://docs.aspose.com/display/cellsjava/Chart+Rendering#ChartRendering-RenderingChartstoImages
[5]: https://blog.aspose.com/
[6]: https://docs.aspose.com/display/cellsjava/Chart+Formatting#ChartFormatting-ManipulatingDesignerCharts
[7]: https://docs.aspose.com/display/cellsjava/Converting+Workbook+to+Different+Formats#ConvertingWorkbooktoDifferentFormats-ConvertingExceltoPDF
[8]: https://downloads.aspose.com/cells/java




