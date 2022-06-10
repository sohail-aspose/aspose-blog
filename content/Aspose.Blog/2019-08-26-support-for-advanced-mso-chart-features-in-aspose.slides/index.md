---
title: 'Use Advanced MSO Chart Features in PowerPoint Presentations in C# or Java'
date: Mon, 26 Aug 2019 05:03:28 +0000
draft: false
url: /2019/08/26/support-for-advanced-mso-chart-features-in-aspose.slides/
author: Mudassir
summary: ''
tags: []
categories: ['Aspose.Slides Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Slides-for-net_100.png) Hi guys! In today's blog, I would like to share my experience after using the latest [Aspose.Slides][2] 19.7 which has been enriched with improved chart manipulation features. The best thing about Aspose.Slides is that it has a monthly release where .NET, Java, Android via Java, and C++ based APIs are published together. So, what's available in .NET based API is also available for Java, Android via Java and C++ based APIs. This way the users feels comfortable with API they are using and with same features available across the board.

In the following sections, I am going to give you a walk through of what new features have been included and what improvements have been carried in API.

## Set External Workbook for Chart

When working with MSO charts insider PowerPoint presentation, one may set an external workbook to chart as a data source. Now, Aspose.Slides also offers this support and for this purpose **IChartData.SetExternalWorkbook** method has been added. This method can be also used to update a path to the external workbook if it has been moved. Workbooks placed on remote resources unavailable for data editing but still can be assigned as an external data source. If the relative path was provided for an external workbook, it converts to full path automatically.

This example demonstrates how to manage the external workbooks for the chart.

{{< gist aspose-com-gists a56eda38c01ad33dc653116c7bae4293 "Examples-CSharp-Charts-SetExternalWorkbookWithUpdateChartData-SetExternalWorkbookWithUpdateChartData.cs" >}}

The similar Java-based example for this is:

{{< gist aspose-com-gists 1f55f0222bc39a382d831900e8de7400 "Examples-src-main-java-com-aspose-slides-examples-Slides-Charts-SetExternalWorkbookWithUpdateChartData-SetExternalWorkbookWithUpdateChartData.java" >}}

The similar C++ based example for this is:

{{< gist aspose-com-gists 81aeb05e6d3a070aa76fdea22ed53bc7 "Examples-SlidesCPP-SetExternalWorkbook-SetExternalWorkbook.cpp" >}}

## Add Default Chart Markers

Aspose.Slides also provides a simple API to set the chart series marker automatically. In the following feature, every chart series will get different default marker symbols automatically. The following example exhibits the use of a new future.

{{< gist aspose-com-gists a56eda38c01ad33dc653116c7bae4293 "Examples-CSharp-Charts-DefaultMarkersInChart-DefaultMarkersInChart.cs" >}}

The similar Java based example for this is:

{{< gist aspose-com-gists 1f55f0222bc39a382d831900e8de7400 "Examples-src-main-java-com-aspose-slides-examples-Slides-Charts-DefaultMarkersInChart-DefaultMarkersInChart.java" >}}

The similar C++ based example for this is:

{{< gist aspose-com-gists 81aeb05e6d3a070aa76fdea22ed53bc7 "Examples-SlidesCPP-DefaultMarkersInChart-DefaultMarkersInChart.cpp" >}}

## Improved Chart Series Data Points Management {#mce_24}

Aspose.Slides also offer support for removing the individual chart series data points. All you need to do is to access the desired series data point and clear that. The following example exhibits the use of new future.

{{< gist aspose-com-gists a56eda38c01ad33dc653116c7bae4293 "Examples-CSharp-Charts-ClearSpecificChartSeriesDataPointsData-ClearSpecificChartSeriesDataPointsData.cs" >}}

The similar Java-based example for this is:

{{< gist aspose-com-gists 1f55f0222bc39a382d831900e8de7400 "Examples-src-main-java-com-aspose-slides-examples-Slides-Charts-ClearSpecificChartSeriesDataPointsData-ClearSpecificChartSeriesDataPointsData.java" >}}

The similar C++ based example for this is:

{{< gist aspose-com-gists 81aeb05e6d3a070aa76fdea22ed53bc7 "Examples-SlidesCPP-ClearSpecificChartSeriesDataPointsData-ClearSpecificChartSeriesDataPointsData.cpp" >}}

Wait, there's many other features, enhancement, and bug fixes included in this release. [Here you can get the detail!][3]

When time allows you can check out API [examples at Github][4], talk about this release and other API related issues in our [forum][5].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Slides-for-net_100.png "Aspose.Slides or .NET logo"
[2]: https://products.aspose.com/slides
[3]: https://docs.aspose.com/slides/net/aspose-slides-for-net-19-7-release-notes/
[4]: https://github.com/aspose-slides/
[5]: https://forum.aspose.com/c/slides




