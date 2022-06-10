---
title: 'Read Large Excel Files with LightCells API using Java'
date: Tue, 21 Jan 2014 09:44:41 +0000
draft: false
url: /2014/01/21/read-large-excel-files-with-lightcells-api-and-find-cells-based-on-formatting-in-aspose.cells-for-java-7.7.1/
author: Amjad Sahi
summary: ''
tags: ['Excel Files', 'LighCells API', 'conditional formatting', 'export Excel workbooks to PDF', 'improved OOXML API', 'manipulate PivotTables', 'render MS Excel file formats', 'render images files from Charts', 'rendering Charts']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java logo">}}


We are pleased to announce the release of Aspose.Cells for Java 7.7.1 with certain new features, enhancements, and other bug fixes. This new release supports [reading large Excel files with LightCells API][1]. This is a useful feature. Sometimes you need to read data from a huge Microsoft Excel workbook with millions of records and you are always worried about the performance. You want it to take less time and memory to process big files. The LightCells API is useful in that scenario: to read huge Excel spreadsheets, it uses less memory, so you get better performance and efficiency.

The following sample code shows how to load an Excel file in light-weight mode. The sample code reads a big file and retrieves the total number of cells, a count of strings, and a count of formulas for each worksheet in the workbook.

{{< gist aspose-cells 87c05ec07dd1a65ac6fcdf2fa896b01e "Examples-src-main-java-com-aspose-cells-examples-articles-LightCellsTest1-LightCellsTest1.java" >}}

{{< gist aspose-cells 87c05ec07dd1a65ac6fcdf2fa896b01e "Examples-src-main-java-com-aspose-cells-examples-articles-LightCellsDataHandlerVisitCells-LightCellsDataHandlerVisitCells.java" >}}

## Finding Cells Based on Formatting

Another valuable feature is to [find the cells with some particular style or formatting][2]. Aspose.Cells supports finding all cells that have a common style or formatting. Aspose.Cells provides the FindOptions.setStyle() method which you can use to specify the style to search cells for.

## Transparent Images

You can now [create transparent images of Microsoft Excel worksheet][3]. Sometimes, you need to generate an image of your worksheet as a transparent image. For example, you might want to apply transparency to all the cells which have no fill color. Aspose.Cells provides the ImageOrPrintOptions.setTransparent() method which applies transparency to a  worksheet image.

We have added support to parse/ read ActiveX controls in the template files. We have also added a number of enhancements in the new release. In this version, we have refactored the PivotTables module. We've made tremendous enhancements and fixed several issues.

To see a complete list of enhancements and fixes and to download Aspose.Cells for Java 7.7.1, please visit the [download page][4].




[1]: https://docs.aspose.com/display/cellsjava/Using+LightCells+API
[2]: https://docs.aspose.com/display/cellsjava/Find+cells+with+specific+style
[3]: https://docs.aspose.com/display/cellsjava/Create+Transparent+Image+of+Excel+Worksheet
[4]: https://downloads.aspose.com/cells/java




