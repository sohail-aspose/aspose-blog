---
title: 'Convert Excel Charts to SVG Format using Java with Aspose.Cells for Java 8.3.0'
date: Thu, 20 Nov 2014 15:01:04 +0000
draft: false
url: /2014/11/20/convert-excel-charts-to-svg-format-using-java-with-aspose.cells-for-java/
author: Babar Raza
summary: ''
tags: ['Babar Raza', 'Convert Excel Charts to SVG in Java']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We have our regular monthly Aspose.Cells for Java release, version 8.3.0, ready for public use. While you download the latest version, here is a look at the biggest features in this month’s release. For a full list of bug fixes and improvements please refer to the release notes for [Aspose.Cells for Java 8.3.0][1]. If you are planning to upgrade the API from any previous version, we would suggest you to check the [Public API Changes][2] section.

## Convert Excel Charts to SVG Format

Aspose.Cells for Java 8.3.0 provides support for exporting charts in Scalable Vector Graphics (SVG) format, an XML-based vector image format for two-dimensional graphics which supports interactivity and animation. Please refer to the following piece of code to see how it's done and feel free to read the detailed article on [saving charts to SVG][3].

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-main-java-com-aspose-cells-examples-articles-ConvertCharttoImageinSVGFormat-ConvertCharttoImageinSVGFormat.java" >}}

## Track Excel Workbook State in Java

Aspose.Cells for Java 8.3.0 has added several properties that could enable developers to track and manipulate a workbook file's state. The aforesaid properties and their brief descriptions are as follow.

*   WorkbookSettings.CrashSave: Indicates whether the application last saved the workbook file after a crash.
*   WorkbookSettings.DataExtractLoad: Indicated whether the application last opened the workbook file for data recovery.
*   WorkbookSettings.RepairLoad: Provides information if the application last opened the workbook file in safe or repair mode.
*   WorkbookSettings.AutoRecover: Indicates if auto-recovery has been performed on the Workbook file.

## Uniquely Identify Shapes in Excel

Version 8.3.0 of Aspose.Cells for Java has added a getter/setter for the property Shape.Id to help developers identify each shape object in a spreadsheet. This property also helps them to uniquely identify the Chart objects in a spreadsheet as demonstrated below.

```
//Create an object of Workbook class and load an exiting spreadsheet
Workbook book = new Workbook("sample.xlsx");

//Retrieve the collection of charts from the first worksheet
ChartCollection charts = book.getWorksheets().get(0).getCharts();

//Iterate over all the charts in the collection
for(int index = 0; index <= charts.getCount(); index++)
{
    //Get a specific chart object
    Chart chart = charts.get(index);

    //Convert the chart object to shape
    Shape shape = (Shape)chart.getChartObject();

    //Display the unique ID
    System.out.println(shape.getId());
}

```

## Other Enhancements & Improvements

The latest release of Aspose.Cells for Java 8.3.0 has fixed numerous problems, and the most notable of these  enhancements are:

*   Enhanced PDF rendering engine to address a few visual problems. Moreover, this release has made sure that Aspose.Cells for Java generated PDF/A-1b files pass the preflight compliance test.
*   Tweaked the chart rendering mechanism.
*   Improved the Formula Engine to address a few issues related to the NOW & RATE functions.
*   Addressed a few issues related to the color pallets.

Please visit the documentation for details, and if you still have any questions, we always welcome inquiries on [Aspose.Cells Support Forum][4].




[1]: https://downloads.aspose.com/cells/java
[2]: https://docs.aspose.com/display/cellsjava/Migrating+from+Earlier+Versions+of+Aspose.Cells
[3]: https://docs.aspose.com/display/cellsjava/Converting+Chart+to+Image+in+SVG+Format
[4]: https://forum.aspose.com/




