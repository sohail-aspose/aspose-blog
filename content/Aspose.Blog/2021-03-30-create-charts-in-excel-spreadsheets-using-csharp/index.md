---
title: 'Create Charts in Excel Spreadsheets using C#'
seoTitle: "Create Charts in Excel in C# | Create Column, Line, and Pyramid Charts"
description: "Use .NET Excel API to create charts in Excel spreadsheets using C#. Create column, line, pyramid and other types of charts in Excel using C#."
date: Tue, 30 Mar 2021 04:32:00 +0000
draft: false
url: /2021/03/30/create-charts-in-excel-spreadsheets-using-csharp/
author: Usman Aziz
summary: 'Excel charts are used to visualize the data in spreadsheets. MS Excel supports a variety of charts such as line, bar, pie, doughnut, pyramid, bubble, etc. In this article, you will learn **how to create different types of charts in Excel files using C#**.'
tags: ['create charts in excel csharp', 'create column charts in excel csharp', 'create line charts in excel csharp', 'create pyramid charts in excel csharp']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/create-excel-charts.jpg" alt="create excel charts C#">}}


Excel charts are used to visualize the data in spreadsheets. MS Excel supports a variety of charts such as line, bar, pie, doughnut, pyramid, bubble, etc. In this article, you will learn **how to create charts in Excel files using C#**.

*   [C# API to Create Charts in Excel][1]
*   [Create Charts in Excel using C#][2]
*   [Create a Line Chart in Excel using C#][3]
*   [Generate a Pyramid Chart in Excel using C#][4]
*   [Get a Free API License][5]

## C# API to Create Charts in Excel {#C-API-to-Create-Excel-Charts}

In order to work with Excel charts, we'll use [Aspose.Cells for .NET][6]. It is a powerful API that lets you implement Excel automation in .NET applications. Furthermore, it allows you create a variety of charts seamlessly. To use the API, you can either [download][7] the DLL or install it using [NuGet][8].

```
Install-Package Aspose.Cells
```

## Supported Excel Chart Types

Aspose.Cells for .NET provides a complete set of standard chart types. The list includes, but not limited to:

<figure class="wp-block-table is-style-stripes"><table><thead><tr><th>**Chart Types</strong></th><th><strong>Description**</th></tr></thead><tbody><tr><td>Column</td><td>Represents Clustered Column Chart</td></tr><tr><td>ColumnStacked</td><td>Represents Stacked Column Chart</td></tr><tr><td>Column100PercentStacked</td><td>Represents 100% Stacked Column Chart</td></tr><tr><td>Column3DClustered</td><td>Represents 3D Clustered Column Chart</td></tr><tr><td>Column3DStacked</td><td>Represents 3D Stacked Column Chart</td></tr><tr><td>Column3D100PercentStacked</td><td>Represents 3D 100% Stacked Column Chart</td></tr><tr><td>Column3D</td><td>Represents 3D Column Chart</td></tr><tr><td>Bar</td><td>Represents Clustered Bar Chart</td></tr><tr><td>BarStacked</td><td>Represents Stacked Bar Chart</td></tr><tr><td>Bar100PercentStacked</td><td>Represents 100% Stacked Bar Chart</td></tr><tr><td>Bar3DClustered</td><td>Represents 3D Clustered Bar Chart</td></tr><tr><td>Bar3DStacked</td><td>Represents 3D Stacked Bar Chart</td></tr><tr><td>Bar3D100PercentStacked</td><td>Represents 3D 100% Stacked Bar Chart</td></tr><tr><td>Line</td><td>Represents Line Chart</td></tr><tr><td>LineStacked</td><td>Represents Stacked Line Chart</td></tr><tr><td>Line100PercentStacked</td><td>Represents 100% Stacked Line Chart</td></tr><tr><td>LineWithDataMarkers</td><td>Represents Line Chart with data markers</td></tr><tr><td>LineStackedWithDataMarkers</td><td>Represents Stacked Line Chart with data markers</td></tr><tr><td>Line100PercentStackedWithDataMarkers</td><td>Represents 100% Stacked Line Chart with data markers</td></tr><tr><td>Line3D</td><td>Represents 3D Line Chart</td></tr><tr><td>Pie</td><td>Represents Pie Chart</td></tr><tr><td>Pie3D</td><td>Represents 3D Pie Chart</td></tr><tr><td>PiePie</td><td>Represents Pie of Pie Chart</td></tr><tr><td>PieExploded</td><td>Represents Exploded Pie Chart</td></tr><tr><td>Pie3DExploded</td><td>Represents 3D Exploded Pie Chart</td></tr><tr><td>PieBar</td><td>Represents Bar of Pie Chart</td></tr><tr><td>Scatter</td><td>Represents Scatter Chart</td></tr><tr><td>ScatterConnectedByCurvesWithDataMarker</td><td>Represents Scatter Chart connected by curves, with data markers</td></tr></tbody></table></figure>

For a complete list of supported Excel charts, visit [this article][9].

## Create Charts in Excel using C# {#Create-Excel-Charts-in-C}

The following are the steps to create a chart in Excel using C#.

*   First, create a new Excel workbook or load an existing one using [Workbook][10] class.
*   Access the desired worksheet into a [Worksheet][11] object.
*   Insert data into the worksheet (if worksheet is empty).
*   Create a chart in the worksheet using [Worksheet.Charts.Add(ChartType type, int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)][12] method.
*   Access the chart by its index into a [Chart][13] object.
*   Set data source for the chart using [Chart.SetChartDataRange("A1:C4", true)][14] method.
*   Finally, save the workbook using [Workbook.Save(string)][15] method.

The following code sample shows how to create an Excel chart using C#.

{{< gist aspose-com-gists eddcc259381039dc73a7060e7f520f7c "create-column-chart.cs" >}}



{{< figure align=center src="images/Create-Column-Chart-in-Excel.jpg" alt="create column chart in C#">}}


## Create a Line Chart in Excel using C# {#Create-a-Line-Chart-in-Excel-using-C}

In order to insert a line chart, you only need to specify the [ChartType.Line][16] type in [Worksheet.Charts.Add()][17] method. The rest of the steps will be the same as mentioned in the previous section.

*   First, create an Excel workbook using the [Workbook][18] class.
*   Access the desired worksheet into a [Worksheet][19] object.
*   Insert data into the worksheet.
*   Create the line chart using [Worksheet.Charts.Add()][20] method.
*   Access the chart by its index into a [Chart][21] object.
*   Set data source for the chart using [Chart.SetChartDataRange("A1:C4", true)][22] method.
*   Finally, ave the workbook using [Workbook.Save(string)][23] method.

The following code sample shows how to create a line chart in Excel using C#.

{{< gist aspose-com-gists eddcc259381039dc73a7060e7f520f7c "create-line-chart.cs" >}}



{{< figure align=center src="images/Create-Line-Chart-in-Excel.jpg" alt="line chart in in Excel C#">}}


## Create a Pyramid Chart in Excel using C# {#Generate-a-Pyramid-Chart-in-Excel-using-C}

For adding a pyramid chart, simply pass ChartType.Pyramid type while adding the chart to the worksheet. The following are the steps to add a pyramid chart in Excel using C#.

*   First, create an Excel workbook using the [Workbook][24] class.
*   Access the desired worksheet into a [Worksheet][25] object.
*   Insert data into the worksheet.
*   Create the pyramid chart using [Worksheet.Charts.Add()][26] method.
*   Access the chart by its index into a [Chart][27] object.
*   Set data source for the chart using [Chart.SetChartDataRange("A1:C4", true)][28] method.
*   Finally, save the workbook using [Workbook.Save(string)][29] method.

The following code sample shows how to insert a pyramid chart in an Excel worksheet using C#.

{{< gist aspose-com-gists eddcc259381039dc73a7060e7f520f7c "create-pyramid-chart.cs" >}}



{{< figure align=center src="images/Create-Pyramid-Chart-in-Excel.jpg" alt="create pyramid chart in Excel">}}


To learn more about working with Excel charts, read [this][30] documentation article.

## Get a Free API License {#Get-a-Free-API-License}

You can try Aspose.Cells for .NET without evaluation limitations by requesting a [temporary license][31].

## Conclusion

In this article, you have seen how to create charts in Excel worksheets using C#. Particularly, you have learned how to create column, line, and pyramid charts in Excel. Furthermore, you can also create other types of charts seamlessly using Aspose.Cells for .NET. For more details, visit the [documentation][32] of the API. In case you would have any queries, contact us via our [forum][33].

## See Also

*   [Copy or Move Excel Worksheets using C#][34]




[1]: #Create-Excel-Charts-in-C
[2]: #Create-Excel-Charts-in-C
[3]: #Create-a-Line-Chart-in-Excel-using-C
[4]: #Generate-a-Pyramid-Chart-in-Excel-using-C
[5]: #Get-a-Free-API-License
[6]: https://products.aspose.com/cells/net
[7]: https://downloads.aspose.com/cells/net
[8]: https://nuget.org/packages/Aspose.Cells
[9]: https://docs.aspose.com/cells/net/creating-charts/#create-chart-using-asposecells
[10]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[11]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[12]: https://apireference.aspose.com/cells/net/aspose.cells.charts/chartcollection/methods/add
[13]: https://apireference.aspose.com/cells/net/aspose.cells.charts/chart
[14]: https://apireference.aspose.com/cells/net/aspose.cells.charts/chart/methods/setchartdatarange
[15]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/2
[16]: https://apireference.aspose.com/cells/net/aspose.cells.charts/charttype
[17]: https://apireference.aspose.com/cells/net/aspose.cells.charts/chartcollection/methods/add
[18]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[19]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[20]: https://apireference.aspose.com/cells/net/aspose.cells.charts/chartcollection/methods/add
[21]: https://apireference.aspose.com/cells/net/aspose.cells.charts/chart
[22]: https://apireference.aspose.com/cells/net/aspose.cells.charts/chart/methods/setchartdatarange
[23]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/2
[24]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[25]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[26]: https://apireference.aspose.com/cells/net/aspose.cells.charts/chartcollection/methods/add
[27]: https://apireference.aspose.com/cells/net/aspose.cells.charts/chart
[28]: https://apireference.aspose.com/cells/net/aspose.cells.charts/chart/methods/setchartdatarange
[29]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/2
[30]: https://docs.aspose.com/cells/net/charts/
[31]: https://purchase.aspose.com/temporary-license
[32]: https://docs.aspose.com/cells/net/getting-started/
[33]: https://forum.aspose.com/
[34]: https://blog.aspose.com/2021/03/15/copy-excel-worksheets-using-csharp/





