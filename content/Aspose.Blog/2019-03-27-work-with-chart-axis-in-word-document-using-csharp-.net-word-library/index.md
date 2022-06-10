---
title: 'Work with Chart Axis in Word Document using C#'
date: Wed, 27 Mar 2019 17:53:22 +0000
draft: false
url: /2019/03/27/work-with-chart-axis-in-word-document-using-csharp-.net-word-library/
author: Muzammil Khan
summary: ''
tags: ['Work with Chart Axis in Word using Csharp']
categories: ['Aspose.Words Product Family']
---

The chart is a very useful feature to graphically represent or visualize any kind of data in a way to create maximum impact on target audiences. Charts allow users to see the results of the represented data in order to better understand and predict current and future data.

In a Word document, there are various types of charts available to work with based on the needs of users. To make a chart easier to understand, the chart title and axis titles can be added to any type of chart. Axis titles are typically available for all axes that can be displayed in a chart and most commonly used chart types have two axis. The X-axis along the bottom of the chart, usually the horizontal axis and the Y-axis along the left, usually the vertical axis.

## Hide Chart Axis in Word Document using C#

In some cases, the user may need to hide the chart axis or anyone of them. Using [Aspose.Words for .NET][1], this can simply be achieved by setting the value of **ChartAxis.Hidden** property for a specific axis to false. This property gets or sets a flag indicating whether this axis is hidden or not. The default value is **false**.

The following code snippet shows how to hide the Y-axis of the chart.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Programming-Documents-Charts-WorkingWithChartAxis-HideChartAxis.cs" >}}

The resulting view of the chart is given below where Y-axis is hidden:



{{< figure align=center src="images/HideYAxis.png" alt="">}}


## Multi-line Label Alignment in Charts

While working with ChartAxis, [Aspose.Words][2] for .NET provides an opportunity to set user-defined label alignment for the axis of the series. Microsoft Word aligns all the axis labels to the center by default as shown below:



{{< figure align=center src="images/Default_View.png" alt="">}}


The [**TickLabelAlignment**][3] property has been introduced under [ChartAxis][4] class for setting the label alignment. The ChartAxis class represents the axis options of the chart. The **TickLabelAlignment** property gets or sets text alignment of axis tick labels and it has effect only in case of multi-line labels. The default value is "[**ParagraphAlignment**][5]**.Center**".

The following code snippet shows the working of **TickLabelAlignment**.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Programming-Documents-Charts-WorkingWithChartAxis-TickMultiLineLabelAlignment.cs" >}}

The resulting view of the chart is shown below:



{{< figure align=center src="images/Right_Aligned_View.png" alt="">}}





[1]: https://products.aspose.com/words
[2]: https://products.aspose.com/words
[3]: https://apireference.aspose.com/net/words/aspose.words.drawing.charts/chartaxis/properties/ticklabelalignment
[4]: https://apireference.aspose.com/net/words/aspose.words.drawing.charts/chartaxis
[5]: https://apireference.aspose.com/net/words/aspose.words/paragraphalignment




