---
title: 'Create Charts in PowerPoint Presentations using C#'
seoTitle: "Create Charts in PowerPoint PPT in C# | Pie, Histogram, Column, Stock"
description: "Use .NET API to create charts in PowerPoint PPT PPTX using C#. Create pie chart, scatter chart, column chart, histogram chart and stock chart in PPTX."
date: Mon, 01 Feb 2021 11:51:00 +0000
draft: false
url: /2021/02/01/create-charts-in-powerpoint-using-csharp/
author: Usman Aziz
summary: 'Charts are used to summarize and visually represent the data within the PowerPoint presentations. Therefore, PowerPoint provides a wide range of chart types to visualize the data. Among all, the most commonly used chart types include pie charts, line charts, bar charts, histograms, stock charts, and etc. In this article, you will learn **how to create these popular types of charts in PowerPoint presentations using C#**.'
tags: ['create charts in powerpoint in csharp', 'create column chart in powerpoint in csharp', 'create histogram chart in powerpoint in csharp', 'create pie chart in powerpoint in csharp', 'create scattered chart in powerpoint in csharp', 'create stock chart in powerpoint in csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/create-charts.jpg" alt="create charts in powerpoint ppt C#">}}


Charts are used to summarize and visually represent the data within the PowerPoint presentations. Therefore, PowerPoint provides a wide range of chart types to visualize the data. Among all, the most commonly used chart types include pie charts, line charts, bar charts, histograms, stock charts, and etc. In this article, you will learn **how to create these charts in PowerPoint presentations using C#**.

*   [C# API to Create Charts in PowerPoint][1]
*   [Create Column Chart in PowerPoint using C#][2]
*   [Create Scatter Chart in PowerPoint using C#][3]
*   [Add Pie Chart in PowerPoint using C#][4]
*   [Add Histogram Chart in PowerPoint using C#][5]
*   [Create a Stock Chart in PowerPoint using C#][6]
*   [Get Free API License][7]

## C# API to Create Charts in PowerPoint {#CSharp-API-to-Create-Charts-in-PowerPoint}

[Aspose.Slides for .NET][8] is a C# class library that lets you create and manipulate PowerPoint presentations from within .NET applications. Furthermore, the API allows you to create and add charts to the presentations seamlessly. Aspose.Slides for .NET can be downloaded as [DLL][9] or installed via [NuGet][10].

```
PM> Install-Package Aspose.Slides
```

## Create Column Chart in PowerPoint PPT using C# {#Create-Column-Chart-in-PowerPoint-using-CSharp}

In this section, you will learn how to create a column chart and add categories and series to populate that chart. The following are the steps to perform this operation.

*   First, create an instance of the [Presentation][11] class.
*   Get the reference of the slide in the [ISlide][12] object.
*   Add a _ClusteredColumn_ chart with default data and get its reference in [IChart][13] object.
*   Set chart title using [IChart.ChartTitle.AddTextFrameForOverriding(String)][14] method and set its properties.
*   Access the chart data workbook into the [IChartDataWorkbook][15] object.
*   Clear all the default series and categories from chart data using [IChart.ChartData.Series.Clear()][16] and [IChart.ChartData.Categories.Clear()][17] methods respectively.
*   Add new series and categories.
*   Access each chart series into the [IChartSeries][18] object and add data points to it.
*   Add fill color for chart series and set labels.
*   Finally, save the presentation using [Presentation.Save(String, SaveFormat)][19] method.

For demonstration, the following code sample shows how to create a column chart in PowerPoint presentation using C#.

{{< gist aspose-com-gists b153e69edb99d4fb64f022bd6fd8879e "add-column-chart.cs" >}}

The following is the screenshot of the resultant column chart.



{{< figure align=center src="images/column-chart.jpg" alt="create column chart in powerpoint in C#">}}


## Create Scatter Chart in PowerPoint PPT using C# {#Create-Scattered-Chart-in-PowerPoint-using-CSharp}

The following are the steps to create a scatter chart in the PowerPoint presentation using C#.

*   Create a new presentation using the [Presentation][20] class.
*   Get the reference of the slides in the [ISlide][21] object.
*   Add a _ScatterWithSmoothLines_ chart type with default data and get its reference in [IChart][22] object.
*   Access the chart data workbook into the [IChartDataWorkbook][23] object and clear the default series.
*   Add new series to the chart data.
*   Access each series into the [IChartSeries][24] object and add data points to the series.
*   Set the marker for the series using [IChartSeries.Marker][25] property.
*   Save the presentation using [Presentation.Save(String, SaveFormat)][26] method.

The following code sample shows how to create a scatter chart in PowerPoint presentations using C#.

{{< gist aspose-com-gists b153e69edb99d4fb64f022bd6fd8879e "add-scattered-chart.cs" >}}

The following screenshot shows the resultant scatter chart.



{{< figure align=center src="images/scattered-chart.jpg" alt="create scattered chart in powerpoint in C#">}}


## Create Pie Chart in PowerPoint PPT using C# {#Add-Pie-Chart-in-PowerPoint-using-CSharp}

The following are the steps to create a pie chart in a PowerPoint presentation using C#.

*   Create a new presentation using the [Presentation][27] class.
*   Get the reference of the slides in the [ISlide][28] object.
*   Add a _Pie_ chart type with default data and get its reference in [IChart][29] object.
*   Set chart title using [IChart.ChartTitle.AddTextFrameForOverriding(String)][30] method and set its properties.
*   Set visibility of the values.
*   Clear the default series and categories using using [IChart.ChartData.Series.Clear()][31] and [IChart.ChartData.Categories.Clear()][32] methods respectively.
*   Access the chart data workbook into the [IChartDataWorkbook][33] object.
*   Add new categories to the chart data into [IChart.ChartData.Categories][34] collection.
*   Add new series to the chart data into [IChart.ChartData.Series][35] collection.
*   Obtain each series into the [IChartSeries][36] object and add data points to the series.
*   Access each data point into [IChartDataPoint][37] object and set its formatting.
*   Access data labels in the data points using [IDataLabel][38] object and set their formatting.
*   Set leader lines and rotation angles.
*   Save the presentation using [Presentation.Save(String, SaveFormat)][39] method.

The following code sample shows how to create a pie chart in PowerPoint presentation using C#.

{{< gist aspose-com-gists b153e69edb99d4fb64f022bd6fd8879e "add-pie-chart.cs" >}}

The following is the screenshot of the generated pie chart.



{{< figure align=center src="images/pie-chart.jpg" alt="create pie chart in powerpoint in C#">}}


## Add Histogram Chart in PowerPoint PPTX using C# {#Add-Histogram-Chart-in-PowerPoint-using-CSharp}

The following are the steps to create a histogram chart in PowerPoint presentations using Aspose.Slides for .NET.

*   Create an instance of the [Presentation][40] class.
*   Obtain a slide’s reference in the [ISlide][41] object by its index.
*   Add a _Histogram_ chart with default data.
*   Clear the default series and categories.
*   Access the chart data workbook in the [IChartDataWorkbook][42] object.
*   Add new series and get its reference in the [IChartSeries][43] object.
*   Add data points to the series.
*   Set aggregation type of the chart axis.
*   Save the presentation using [Presentation.Save(String, SaveFormat)][44] method.

The following code sample shows how to create a histogram chart using C#.

{{< gist aspose-com-gists b153e69edb99d4fb64f022bd6fd8879e "add-histogram-chart.cs" >}}

The following is the screenshot of the created histogram chart.



{{< figure align=center src="images/histogram-chart.jpg" alt="create histogram chart in powerpoint in C#">}}


## Create a Stock Chart in PowerPoint using C# {#Create-a-Stock-Chart-in-PowerPoint-using-CSharp}

Stock chart is also one of the commonly used chart types within PowerPoint presentations. The following are the steps to create a stock chart.

*   Create a new PowerPoint presentation using [Presentation][45] class.
*   Obtain slide’s reference in an [ISlide][46] object using the slide's index.
*   Add _OpenHighLowClose_ chart to the slide and get its reference in the [IChart][47] object.
*   Clear the default series and categories.
*   Access the chart data in [IChartDataWorkbook][48] object.
*   Add new series and categories to the chart.
*   Access each chart series and add data points.
*   Specify _HiLowLines_ format.
*   Save the presentation using [Presentation.Save(String, SaveFormat)][49] method.

The following code sample shows how to add a stock chart to PowerPoint presentation using C#.

{{< gist aspose-com-gists b153e69edb99d4fb64f022bd6fd8879e "add-stock-chart.cs" >}}

The following is the screenshot of the created stock chart.



{{< figure align=center src="images/stock-chart.jpg" alt="create stock chart in powerpoint in C#">}}


## More Chart Types

In addition to the above-mentioned charts, there are other types of charts as well that you can add to the PowerPoint presentations. In order to read more about the supported chart types, you can visit [this][50] documentation article.

## Get a Free API License {#Get-a-Free-API-License}

You can [get a free temporary license][51] in order to try the API without evaluation limitations.

## Conclusion

In this article, you have learned how to create charts in PowerPoint presentations using C#. Furthermore, the step-by-step guide and code samples have shown how to add column charts, scatter charts, pie charts, histograms, and stock charts. You can explore more about Aspose.Slides for .NET using [documentation][52].

## See Also

*   [Create MS PowerPoint Presentations in C#][53]




[1]: #CSharp-API-to-Create-Charts-in-PowerPoint
[2]: #Create-Column-Chart-in-PowerPoint-using-CSharp
[3]: #Create-Scattered-Chart-in-PowerPoint-using-CSharp
[4]: #Add-Pie-Chart-in-PowerPoint-using-CSharp
[5]: #Add-Histogram-Chart-in-PowerPoint-using-CSharp
[6]: #Create-a-Stock-Chart-in-PowerPoint-using-CSharp
[7]: #Get-a-Free-API-License
[8]: https://products.aspose.com/slides/net
[9]: https://downloads.aspose.com/slides/net
[10]: https://nuget.org/packages/Aspose.Slides
[11]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[12]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[13]: https://apireference.aspose.com/slides/net/aspose.slides.charts/ichart
[14]: https://apireference.aspose.com/slides/net/aspose.slides.charts/ioverridabletext/methods/addtextframeforoverriding
[15]: https://apireference.aspose.com/slides/net/aspose.slides.charts/ichartdataworkbook
[16]: https://apireference.aspose.com/slides/net/aspose.slides.charts/ichartseriescollection/methods/clear
[17]: https://apireference.aspose.com/slides/net/aspose.slides.charts/ichartcategorycollection/methods/clear
[18]: https://apireference.aspose.com/slides/net/aspose.slides.charts/ichartseries
[19]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/4
[20]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[21]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[22]: https://apireference.aspose.com/slides/net/aspose.slides.charts/ichart
[23]: https://apireference.aspose.com/slides/net/aspose.slides.charts/ichartdataworkbook
[24]: https://apireference.aspose.com/slides/net/aspose.slides.charts/ichartseries
[25]: https://apireference.aspose.com/slides/net/aspose.slides.charts/ichartseries/properties/marker
[26]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/4
[27]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[28]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[29]: https://apireference.aspose.com/slides/net/aspose.slides.charts/ichart
[30]: https://apireference.aspose.com/slides/net/aspose.slides.charts/ioverridabletext/methods/addtextframeforoverriding
[31]: https://apireference.aspose.com/slides/net/aspose.slides.charts/ichartseriescollection/methods/clear
[32]: https://apireference.aspose.com/slides/net/aspose.slides.charts/ichartcategorycollection/methods/clear
[33]: https://apireference.aspose.com/slides/net/aspose.slides.charts/ichartdataworkbook
[34]: https://apireference.aspose.com/slides/net/aspose.slides.charts/ichartdata/properties/categories
[35]: https://apireference.aspose.com/slides/net/aspose.slides.charts/ichartdata/properties/series
[36]: https://apireference.aspose.com/slides/net/aspose.slides.charts/ichartseries
[37]: https://apireference.aspose.com/slides/net/aspose.slides.charts/ichartdatapoint
[38]: https://apireference.aspose.com/slides/net/aspose.slides.charts/idatalabel
[39]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/4
[40]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[41]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[42]: https://apireference.aspose.com/slides/net/aspose.slides.charts/ichartdataworkbook
[43]: https://apireference.aspose.com/slides/net/aspose.slides.charts/ichartseries
[44]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/4
[45]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[46]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[47]: https://apireference.aspose.com/slides/net/aspose.slides.charts/ichart
[48]: https://apireference.aspose.com/slides/net/aspose.slides.charts/ichartdataworkbook
[49]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/4
[50]: https://docs.aspose.com/slides/net/create-chart/
[51]: https://purchase.aspose.com/temporary-license
[52]: https://docs.aspose.com/slides/net/getting-started/
[53]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/





