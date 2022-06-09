---
title: 'Create Charts in PowerPoint Presentations using Java'
seoTitle: "Java: Create Charts in PowerPoint | Column, Pie, Histogram, Scattered"
description: "Use Java PowerPoint API to create charts in PPT/PPTX presentations using Java. Create column, scatter, pie, histograms, stock and other charts."
date: Thu, 29 Jul 2021 00:04:00 +0000
draft: false
url: /2021/07/29/create-charts-in-powerpoint-using-java/
author: Usman Aziz
summary: 'Charts are used to summarize and visually represent the data within the presentations. To visualize the data, MS PowerPoint provides a wide range of chart types. Among all, the most commonly used chart types include pie charts, line charts, bar charts, histograms, stock charts, and etc. In this article, you will learn **how to create charts in PowerPoint presentations using Java**.'
tags: ['Add Histogram Chart in PowerPoint using Java', 'Add Pie Chart in PowerPoint using Java', 'Create Column Chart in PowerPoint using Java', 'Create Scattered Chart in PowerPoint using Java', 'Create a Stock Chart in PowerPoint using Java']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/create-charts.jpg" alt="create charts in powerpoint ppt java">}}


Charts are used to summarize and visually represent the data within the presentations. To visualize the data, MS PowerPoint provides a wide range of chart types. Among all, the most commonly used chart types include pie charts, line charts, bar charts, histograms, stock charts, and etc. In this article, you will learn **how to create charts in PowerPoint presentations using Java**.

*   [API to Create Charts in PowerPoint][1]
*   [Create Column Chart in PowerPoint using Java][2]
*   [Create Scattered Chart in PowerPoint using Java][3]
*   [Add Pie Chart in PowerPoint using Java][4]
*   [Add Histogram Chart in PowerPoint using Java][5]
*   [Create a Stock Chart in PowerPoint using Java][6]

## Java API to Create Charts in PowerPoint {#Java-API-to-Create-Charts-in-PowerPoint}

In order to create different types of charts in presentations, we will use [Aspose.Slides for Java][7]. The said API lets you create and manipulate PowerPoint presentations from within your Java applications. Furthermore, it allows you to create and add charts to the presentations seamlessly. You can either [download][8] the API or install it using the following Maven configurations.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-slides</artifactId>
    <version>21.7</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Create Column Chart in PowerPoint PPT using Java {#Create-Column-Chart-in-PowerPoint-using-CSharp}

The following are the steps to create a column chart in a PowerPoint presentation using Java.

*   First, create an instance of the [Presentation][9] class (specify path of the file in the constructor in case of loading exisitng presentation).
*   Obtain the slide’s reference by specifying it's index.
*   Add a chart with default data along with the type [ChartType][10].ClusteredColumn.
*   Clear the default series and categories.
*   Access the chart data workbook in a [IChartDataWorkbook][11] object.
*   Add new series and categories of the chart to the workbook.
*   Add new chart data to the chart series.
*   Finally, save the presentation using [Presentation.save(String, SaveFormat)][12] method.

For demonstration, the following code sample shows how to create a column chart in a PowerPoint presentation using Java.

{{< gist aspose-com-gists 84e6152077c1d97df6d8d624c0299ad2 "add-column-chart.java" >}}

The following is the screenshot of the resultant column chart.



{{< figure align=center src="images/column-chart-2.jpg" alt="Create Column Chart in PowerPoint Java">}}


## Create Scattered Chart in PowerPoint PPT using Java {#Create-Scattered-Chart-in-PowerPoint-using-CSharp}

The following are the steps to create a scattered chart in the PowerPoint presentation using Java.

*   Create a new presentation or load an existing one using the [Presentation][13] class.
*   Get the reference of the slide in the [ISlide][14] object.
*   Add a _ScatterWithSmoothLines_ chart type with default data and get its reference in [IChart][15] object.
*   Access the chart data workbook into the [IChartDataWorkbook][16] object and clear the default series.
*   Add new series to the chart data.
*   Access each series into the [IChartSeries][17] object and add data points to the series.
*   Access the marker of the series using [IChartSeries.getMarker()][18] and set its properties.
*   Save the presentation using [Presentation.save(String, SaveFormat)][19] method.

The following code sample shows how to create a scattered chart in PowerPoint presentations using Java.

{{< gist aspose-com-gists 84e6152077c1d97df6d8d624c0299ad2 "add-scattered-chart.java" >}}

The following screenshot shows the resultant scattered chart.



{{< figure align=center src="images/scattered-chart.jpg" alt="create scattered chart in powerpoint in C#">}}


## Create Pie Chart in PowerPoint PPT using Java {#Add-Pie-Chart-in-PowerPoint-using-CSharp}

The following are the steps to create a pie chart in a PowerPoint presentation using Java.

*   Create a new presentation or load an existing one using the [Presentation][20] class.
*   Get reference of the slide by providing its index.
*   Add a chart with default data along with the type [ChartType][21].Pie.
*   Access the chart data in a [IChartDataWorkbook][22] object.
*   Clear the default series and categories.
*   Create new series and categories.
*   Add new chart data for the chart series.
*   Add new points for charts and add custom colors for the pie chart’s sectors.
*   Set labels for series and leader lines for labels.
*   Set the rotation angle for pie chart slides.
*   Save the presentation using [Presentation.save(String, SaveFormat)][23] method.

The following code sample shows how to create a pie chart in PowerPoint presentation using Java.

{{< gist aspose-com-gists 84e6152077c1d97df6d8d624c0299ad2 "add-pie-chart.java" >}}

The following is the screenshot of the generated pie chart.



{{< figure align=center src="images/pie-chart-2.jpg" alt="Creat Pie Chart in PowerPoint Java">}}


## Add Histogram Chart in PowerPoint PPTX using Java {#Add-Histogram-Chart-in-PowerPoint-using-CSharp}

The following are the steps to create a histogram chart in PowerPoint presentations using Java.

*   Create a new presentation or load existing one using [Presentation][24] class.
*   Obtain reference of the slide by providing its index.
*   Add a chart with default data along with the type [ChartType][25].Histogram.
*   Access the chart data in [IChartDataWorkbook][26] object.
*   Clear the default series and categories.
*   Add new series and categories.
*   Save the presentation using [Presentation.save(String, SaveFormat)][27] method.

The following code sample shows how to create a histogram chart using Java.

{{< gist aspose-com-gists 84e6152077c1d97df6d8d624c0299ad2 "add-histogram-chart.java" >}}

The following is the screenshot of the created histogram chart.



{{< figure align=center src="images/histogram-chart.jpg" alt="create histogram chart in powerpoint in C#">}}


## Create a Stock Chart in PowerPoint using Java {#Create-a-Stock-Chart-in-PowerPoint-using-CSharp}

Stock chart is also one of the commonly used chart types within PowerPoint presentations. The following are the steps to create a stock chart in Java.

*   Create an instance of the [Presentation][28] class.
*   Get the reference of the slide by providing its index.
*   Add a chart with default data along with the type [ChartType][29].OpenHighLowClose.
*   Access the chart data in [IChartDataWorkbook][30] object.
*   Clear the default series and categories.
*   Add new series and categories.
*   Add new chart data for the chart series.
*   Specify HiLowLines format.
*   Save the presentation using [Presentation.save(String, SaveFormat)][31] method.

The following code sample shows how to add a stock chart to PowerPoint presentation using C#.

{{< gist aspose-com-gists 84e6152077c1d97df6d8d624c0299ad2 "add-stock-chart.java" >}}

The following is the screenshot of the created stock chart.



{{< figure align=center src="images/stock-chart.jpg" alt="create stock chart in powerpoint in C#">}}


## More Chart Types

In addition to the above-mentioned charts, there are other types of charts as well that you can add to the PowerPoint presentations. In order to read more about the supported chart types, you can visit [this][32] documentation article.

## Get a Free API License {#Get-a-Free-API-License}

You can [get a free temporary license][33] in order to use the API without evaluation limitations.

## Try Online

You can also try the free online tool for creating charts in PowerPoint presentations, which is based on Aspose.Slides.

*   [Create PowerPoint Charts and Diagrams Online][34]

## Conclusion

In this article, you have learned how to create charts in PowerPoint presentations using Java. The step-by-step guide and code samples have shown how to add column charts, scatter charts, pie charts, histograms, and stock charts. You can explore more about Aspose.Slides for Java using [documentation][35]. In case you would have any queries, inform us via our [forum][36].

## See Also

*   [Create PowerPoint PPTX Presentation in Java][37]




[1]: #Java-API-to-Create-Charts-in-PowerPoint
[2]: #Create-Column-Chart-in-PowerPoint-using-CSharp
[3]: #Create-Scattered-Chart-in-PowerPoint-using-CSharp
[4]: #Add-Pie-Chart-in-PowerPoint-using-CSharp
[5]: #Add-Histogram-Chart-in-PowerPoint-using-CSharp
[6]: #Create-a-Stock-Chart-in-PowerPoint-using-CSharp
[7]: https://products.aspose.com/slides/java
[8]: https://downloads.aspose.com/slides/java
[9]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/ChartType
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/IChartDataWorkbook
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/IChart
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/IChartDataWorkbook
[17]: https://apireference.aspose.com/slides/java/com.aspose.slides/IChartSeries
[18]: https://apireference.aspose.com/slides/java/com.aspose.slides/IChartSeries#getMarker--
[19]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[20]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[21]: https://apireference.aspose.com/slides/java/com.aspose.slides/ChartType
[22]: https://apireference.aspose.com/slides/java/com.aspose.slides/IChartDataWorkbook
[23]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[24]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[25]: https://apireference.aspose.com/slides/java/com.aspose.slides/ChartType
[26]: https://apireference.aspose.com/slides/java/com.aspose.slides/IChartDataWorkbook
[27]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[28]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[29]: https://apireference.aspose.com/slides/java/com.aspose.slides/ChartType
[30]: https://apireference.aspose.com/slides/java/com.aspose.slides/IChartDataWorkbook
[31]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[32]: https://docs.aspose.com/slides/java/powerpoint-charts/
[33]: https://purchase.aspose.com/temporary-license
[34]: https://products.aspose.app/slides/chart
[35]: https://docs.aspose.com/slides/java
[36]: https://forum.aspose.com/
[37]: https://blog.aspose.com/2021/01/18/create-powerpoint-presentations-using-java/





