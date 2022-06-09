---
title: 'Create Charts in Excel using Java'
seoTitle: "Create Charts in Excel using Java | Column, Line, Pyramid, Bubble Charts"
description: "Use Java Excel API to create charts in Excel files using Java. Create a variety of charts including line, column, pyramid, bubble and other types."
date: Wed, 23 Jun 2021 07:54:29 +0000
draft: false
url: /2021/06/23/create-charts-in-excel-using-java/
author: Usman Aziz
summary: 'Charts and graphs are used to summarize and visually represent the data. They give an insight that can further be used to make the decisions. Charts are considered to be an integral part of Excel spreadsheets and are widely used in various applications. In this article, you will learn how to generate charts programmatically from the data provided in the Excel worksheets. Particularly, the article covers **how to create different types of charts in Excel using Java**.'
tags: ['Create a Chart in Excel using Java', 'Create a Line Chart in Excel using Java', 'Create a Pyramid Chart in Excel using Java', 'Java API to Create Excel Charts', 'Java Excel API to Create Charts']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/create-excel-charts.jpg" alt="create excel charts in Java">}}


Charts and graphs are used to summarize and visually represent the data. They give an insight that can further be used to make the decisions. Charts are considered to be an integral part of Excel spreadsheets and are widely used in various applications. In this article, you will learn how to generate charts programmatically from the data provided in the Excel worksheets. Particularly, the article covers **how to create different types of charts in Excel using Java**.

*   [Java API to Create Excel Charts][1]
*   [Create a Chart in Excel using Java][2]
*   [Create a Line Chart in Excel using Java][3]
*   [Generate a Pyramid Chart in Excel using Java][4]

## Java API to Create Excel Charts {#Java-API-to-Create-Excel-Charts}

In order to create charts in Excel files, we'll use [Aspose.Cells for Java][5]. It is a powerful API that allows you to implement Excel automation features in your Java applications. Furthermore, it lets you generate a variety of charts within a few lines of code. You can either [download][6] the API or install it using the following Maven configurations.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-cells</artifactId>
    <version>21.6</version>
</dependency>
```

## Supported Excel Chart Types

Aspose.Cells for Java provides a complete set of standard chart types. The list includes, but not limited to:

*   Column
*   Bar
*   Line
*   Pie
*   Scatter
*   Area
*   Doughnut
*   Radar
*   Surface 3D
*   Bubble
*   Stock
*   Cylinder
*   Cone
*   Pyramid

For more details about the supported Excel charts, visit [this article][7].

## Create a Chart in Excel using Java {#Create-Excel-Charts-in-Java}

The following are the steps to create a chart in an Excel file using Java.

*   Create an instance of the [Workbook][8] class to load an existing or create a new Excel file.
*   Get the reference of the desired worksheet into a [Worksheet][9] object.
*   Add data to the worksheet (optional).
*   Create a new chart by specifying its type using [Worksheet.getCharts().add()][10] method.
*   Get the reference of the added chart into a [Chart][11] object.
*   Set data for the chart using [Chart.setChartDataRange(String, boolean)][12] method.
*   Save the Excel workbook using [Workbook.save(String, SaveFormat)][13] method.

The following code sample shows how to create a chart in Excel using Java.

{{< gist aspose-com-gists f5d1733288db72c17d541ac5871cf15d "create-column-chart.java" >}}



{{< figure align=center src="images/Create-Column-Chart-in-Excel-Worksheet.jpg" alt="Create column chart in Excel">}}


For demonstration, lets now create some other types of charts in an Excel workbook.

## Create a Line Chart in Excel using Java {#Create-a-Line-Chart-in-Excel-using-Java}

The following are the steps to create a line chart in Excel using Java.

*   Create an instance of the [Workbook][14] class to load an existing or create a new Excel file.
*   Get the reference of the desired worksheet into a [Worksheet][15] object.
*   Add data to the worksheet (optional).
*   Create a new Line chart by specifying the type _ChartType.LINE_ using [Worksheet.getCharts().add()][16] method.
*   Get the reference of the added chart into a [Chart][17] object.
*   Set data for the chart using [Chart.setChartDataRange(String, boolean)][18] method.
*   Save the Excel workbook using [Workbook.save(String, SaveFormat)][19] method.

The following code sample shows how to create a line chart in Excel using Java.

{{< gist aspose-com-gists f5d1733288db72c17d541ac5871cf15d "create-line-chart.java" >}}



{{< figure align=center src="images/Create-Line-Chart-in-Excel-Worksheet.jpg" alt="Create line chart in Excel">}}


## Create a Pyramid Chart in Excel using Java {#Generate-a-Pyramid-Chart-in-Excel-using-Java}

The following are the steps to create a pyramid chart in Excel using Java.

*   Create an instance of the [Workbook][20] class to load an existing or create a new Excel file.
*   Get the reference of the desired worksheet into a [Worksheet][21] object.
*   Add data to the worksheet (optional).
*   Create a new Pyramid chart by specifying the type _ChartType.PYRAMID_ using [Worksheet.getCharts().add()][22] method.
*   Get the reference of the added chart into a [Chart][23] object.
*   Add NSeries (chart data source) to the chart using [Chart.getNSeries().add(String, boolean)][24] method.
*   Save the Excel workbook using [Workbook.save(String, SaveFormat)][25] method.

The following code sample shows how to create a pyramid chart in Excel using Java.

{{< gist aspose-com-gists f5d1733288db72c17d541ac5871cf15d "create-pyramid-chart.java" >}}



{{< figure align=center src="images/Create-Pyramid-Chart-in-Excel-Worksheet.jpg" alt="Create pyramid chart in Excel">}}


## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Cells for Java without evaluation limitations by getting a [temporary license][26].

## Conclusion

In this article, you have seen how to create charts in Excel worksheets using Java. Particularly, you have learned how to create column, line, and pyramid charts in Excel programmatically. You can use the same method to create other types of charts in Excel worksheets. To learn more about the API, visit the [documentation][27]. In case you would have any queries, contact us via our [forum][28].

## See Also

*   [Create Excel Files using Java without MS Office][29]




[1]: #Java-API-to-Create-Excel-Charts
[2]: #Create-Excel-Charts-in-Java
[3]: #Create-a-Line-Chart-in-Excel-using-Java
[4]: #Generate-a-Pyramid-Chart-in-Excel-using-Java
[5]: https://products.aspose.com/cells/java
[6]: https://downloads.aspose.com/cells/java
[7]: https://docs.aspose.com/cells/java/creating-and-customizing-charts/#creating-a-simple-chart
[8]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[9]: https://apireference.aspose.com/cells/java/com.aspose.cells/Worksheet
[10]: https://apireference.aspose.com/cells/java/com.aspose.cells/chartcollection#add(int,%20int,%20int,%20int,%20int)
[11]: https://apireference.aspose.com/cells/java/com.aspose.cells/Chart
[12]: https://apireference.aspose.com/cells/java/com.aspose.cells/chart#setChartDataRange(java.lang.String,%20boolean)
[13]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String,%20int)
[14]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[15]: https://apireference.aspose.com/cells/java/com.aspose.cells/Worksheet
[16]: https://apireference.aspose.com/cells/java/com.aspose.cells/chartcollection#add(int,%20int,%20int,%20int,%20int)
[17]: https://apireference.aspose.com/cells/java/com.aspose.cells/Chart
[18]: https://apireference.aspose.com/cells/java/com.aspose.cells/chart#setChartDataRange(java.lang.String,%20boolean)
[19]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String,%20int)
[20]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[21]: https://apireference.aspose.com/cells/java/com.aspose.cells/Worksheet
[22]: https://apireference.aspose.com/cells/java/com.aspose.cells/chartcollection#add(int,%20int,%20int,%20int,%20int)
[23]: https://apireference.aspose.com/cells/java/com.aspose.cells/Chart
[24]: https://apireference.aspose.com/cells/java/com.aspose.cells/seriescollection#add(java.lang.String,%20boolean)
[25]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String,%20int)
[26]: https://purchase.aspose.com/temporary-license
[27]: https://docs.aspose.com/cells/java/getting-started/
[28]: https://forum.aspose.com/
[29]: https://blog.aspose.com/2020/10/13/create-excel-xlsx-xls-using-java-without-ms-office/





