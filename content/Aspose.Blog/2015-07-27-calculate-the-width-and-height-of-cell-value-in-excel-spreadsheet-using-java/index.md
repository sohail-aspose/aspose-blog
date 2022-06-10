---
title: 'Calculate the Width and Height of the Cell Value in Excel using Java'
date: Mon, 27 Jul 2015 10:28:51 +0000
draft: false
url: /2015/07/27/calculate-the-width-and-height-of-cell-value-in-excel-spreadsheet-using-java/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We are pleased to announce that Aspose.Cells for Java 8.5.1 is now available for public use. This month's release contains many useful features and improvements along with some critical bug fixes. Please refer to the release notes of [Aspose.Cells for Java 8.5.1][1] for a full list of enhancements. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the [Public API Changes][2] section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Get a Range of Values using ICustomFunction

## Calculate the Width and Height of the Cell Value

Aspose.Cells for Java provides Cell.getWidthOfValue and Cell.getHeightOfValue methods to calculate the width & height of the cell value in unit of pixels. These methods are useful in scenarios where the application requirement is to set the width of the column and height of the row according to the size of the cell value.

The following sample code explains the usage of Cell.getWidthOfValue and Cell.getHeightOfValue methods.

{{< gist aspose-cells 87c05ec07dd1a65ac6fcdf2fa896b01e "Examples-src-main-java-com-aspose-cells-examples-articles-CalculateWidthAndHeightOfCell-CalculateWidthAndHeightOfCell.java" >}}

Aspose.Cells APIs provide the ICustomFunction interface which can be used to implement the user-defined or custom functions that are not supported by Microsoft Excel as built-in functions. While implementing the ICustomFunction interface, most of the time we require to return a single cell value however, sometimes we may also need to return a range of values.

The following code snippet demonstrates how to [return a range of values from ICustomFunction][3].

{{< gist aspose-cells 87c05ec07dd1a65ac6fcdf2fa896b01e "Examples-src-main-java-com-aspose-cells-examples-articles-ReturningRangeOfValues-ReturningRangeOfValues.java" >}}

## Release Unmanaged Resources of Workbook

Aspose.Cells for Java 8.5.1 has exposed the Workbook.dispose method to [release the unmanaged resources of the Workbook object][4]. The dispose pattern is used only for objects that access unmanaged resources, such as file and pipe handles, registry handles, wait handles, or pointers to blocks of unmanaged memory. This is because the garbage collector is very efficient at reclaiming unused managed objects, but it is unable to reclaim unmanaged objects.

## Detect the Data Source Type of ListObject

With this revision, the API has exposed the TableDataSourceType enumeration & read-only ListObject.DataSourceType property that can be used to [detect the data source type of a ListObject][5].

The TableDataSourceType enumeration has the following fields.

*   TableDataSourceType.QUERY\_TABLE
*   TableDataSourceType.XML
*   TableDataSourceType.WORKSHEET
*   TableDataSourceType.SHARE\_POINT

## Other Enhancements & Improvements

The most notable  enhancements in this release are as follow:

*   Improved the PDF rendering for text boxes, markers & arrows.
*   Tweaked calculate engine for handling custom functions & built-in TREND function.
*   Improved the Chart2Image module.
*   Handled ArrayIndexOutOfBoundsException triggered while saving some specific spreadsheets with Aspose.Cells API.

Please visit the [documentation][6] for details, and if you still have any questions, we always welcome inquiries on [Aspose.Cells Support Forum][7].




[1]: https://downloads.aspose.com/cells/java
[2]: http://docs.aspose.com/display/cellsjava/Migrating+from+Earlier+Versions+of+Aspose.Cells
[3]: https://docs.aspose.com/display/cellsjava/Returning+a+Range+of+Values+using+ICustomFunction
[4]: https://docs.aspose.com/display/cellsjava/Release+Unmanaged+Resources+of+the+Workbook
[5]: https://docs.aspose.com/display/cellsjava/Public+API+Changes+in+Aspose.Cells+8.5.1#PublicAPIChangesinAspose.Cells8.5.1-added
[6]: http://docs.aspose.com/display/cellsjava/Home
[7]: https://forum.aspose.com/




