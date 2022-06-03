---
title: 'Create Charts in PowerPoint Presentations in Python'
date: Wed, 16 Feb 2022 14:51:58 +0000
draft: false
url: /2022/02/16/create-charts-in-powerpoint-in-python/
author: ''Usman Aziz''
summary: 'Charts are used for the graphical representation of the data to make the analysis easier. Therefore, MS PowerPoint supports a range of charts to visualize the data in different ways. Among all, the most commonly used charts include pie charts, line charts, bar charts, histograms, stock charts, etc. In this article, you will learn **how to create these charts in PowerPoint PPT or PPTX in Python**.'
tags: ['Add Histogram Chart in PowerPoint in Python', 'Add Pie Chart in PowerPoint in Python', 'Create Column Chart in PowerPoint in Python', 'Create Scatter Chart in PowerPoint in Python', 'Create a Stock Chart in PowerPoint in Python', 'Python Library to Create Charts in PowerPoint']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/create-charts.jpg" alt="Create Charts in PowerPoint Presentations in Python">}}


Charts are used for the graphical representation of the data, which makes the analysis easier. Therefore, MS PowerPoint supports a range of charts to visualize the data in different ways. Among all, the most commonly used charts include pie charts, line charts, bar charts, histograms, stock charts, etc. In this article, you will learn **how to create these charts in PowerPoint PPT or PPTX in Python**.

*   [Python Library to Create Charts in PowerPoint][1]
*   [Create Column Chart in PowerPoint in Python][2]
*   [Create Scatter Chart in PPT in Python][3]
*   [Add Pie Chart in PPT in Python][4]
*   [Add Histogram Chart in PPT in Python][5]
*   [Create a Stock Chart in PowerPoint in Python][6]
*   [More about Charts][7]

## Python Library to Create Charts in PowerPoint PPT {#API-to-Create-Charts-in-PowerPoint}

To create charts in PowerPoint PPT/PPTX, we will use [Aspose.Slides for Python via .NET][8]. It is a feature-rich library that provides a complete package to create and manipulate PowerPoint presentations. You can install it from [PyPI][9] using the following pip command.

```
> pip install aspose.slides
```

Aspose.Slides supports a variety of charts that can be added to the presentations dynamically. In the following sections, we will demonstrate how to create some popular types of charts.

## Create Column Chart in PowerPoint PPT in Python {#Create-Column-Chart-in-PowerPoint}

In this section, you will learn how to create a column chart in a PowerPoint presentation in Python. The following are the steps to perform this operation.

*   First, create an instance of the **Presentation** class.
*   Get the reference of the slide from **Presentations.slides** in an object.
*   Add a Clustered Column chart with default data using **Slide.shapes.add\_chart()** method.
*   Set chart title and other properties such as text formatting.
*   Access the chart data workbook into an object using **Chart.chart\_data.chart\_data\_workbook()** method.
*   Clear all the default series and categories from chart data using **Chart.chart\_data.series.clear()** and **Chart.chart\_data.categories.clear()** methods respectively.
*   Add new series and categories.
*   Access each chart series into an object and add data points to it.
*   Add fill color for chart series and set labels.
*   Finally, save the presentation using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to create a column chart in PowerPoint PPT in Python.

{{< gist aspose-com-gists de5345d7b26f8e48dc5eac6787835b70 "add-column-chart.py" >}}

The following is the screenshot of the resultant column chart.



{{< figure align=center src="images/column-chart.jpg" alt="create column chart in powerpoint in Python">}}


## Create Scatter Chart in PowerPoint PPT in Python {#Create-Scattered-Chart-in-PowerPoint}

The following are the steps to create a scatter chart in the PowerPoint PPT in Python.

*   First, create an instance of the **Presentation** class.
*   Get the reference of the slide from **Presentations.slides** in an object.
*   Add a Scatter chart with default data using **Slide.shapes.add\_chart()** method.
*   Access the chart data workbook into an object using **Chart.chart\_data.chart\_data\_workbook()** method.
*   Add new series to the chart data.
*   Access each series into an object and add data points to the series.
*   Set the marker for the series.
*   Finally, save the presentation using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to create a scatter chart in PowerPoint PPTX in Python.

{{< gist aspose-com-gists de5345d7b26f8e48dc5eac6787835b70 "add-scatter-chart.py" >}}

The following screenshot shows the resultant scatter chart.



{{< figure align=center src="images/scattered-chart.jpg" alt="create scatter chart in powerpoint in Python">}}


## Create Pie Chart in PowerPoint PPT in Python {#Add-Pie-Chart-in-PowerPoint}

The following are the steps to create a pie chart in a PowerPoint PPT in Python.

*   First, create an instance of the **Presentation** class.
*   Get the reference of the slide from **Presentations.slides** in an object.
*   Add a Pie chart with default data using **Slide.shapes.add\_chart()** method.
*   Set chart title and other properties such as text formatting.
*   Set visibility of the values.
*   Clear all the default series and categories from chart data using **Chart.chart\_data.series.clear()** and **Chart.chart\_data.categories.clear()** methods respectively.
*   Access the chart data workbook into an object using **Chart.chart\_data.chart\_data\_workbook()** method.
*   Add new categories to the chart data.
*   Add new series to the chart data.
*   Access each series into an object and add data points to the series.
*   Access each data point and set its formatting.
*   Apply formatting to data labels in the data points.
*   Set leader lines and rotation angles.
*   Finally, save the presentation using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to create a pie chart in PowerPoint PPTX in Python.

{{< gist aspose-com-gists de5345d7b26f8e48dc5eac6787835b70 "add-pie-chart.py" >}}

The following is the screenshot of the generated pie chart.



{{< figure align=center src="images/pie-chart.jpg" alt="create pie chart in powerpoint in Python">}}


## Add Histogram Chart in PowerPoint PPTX in Python {#Add-Histogram-Chart-in-PowerPoint}

The following are the steps to create a histogram chart in PowerPoint PPT using Aspose.Slides for Python.

*   First, create an instance of the **Presentation** class.
*   Get the reference of the slide from **Presentations.slides** in an object.
*   Add a Histogram chart with default data using **Slide.shapes.add\_chart()** method.
*   Clear the default series and categories.
*   Access the chart data workbook into an object using **Chart.chart\_data.chart\_data\_workbook()** method.
*   Add new series to the chart data.
*   Access each series into an object and add data points to the series.
*   Set aggregation type of the chart axis.
*   Finally, save the presentation using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to create a histogram chart in PPTX in Python.

{{< gist aspose-com-gists de5345d7b26f8e48dc5eac6787835b70 "add-histogram-chart.py" >}}

The following is the screenshot of the created histogram chart.



{{< figure align=center src="images/histogram-chart.jpg" alt="create histogram chart in powerpoint in Python">}}


## Create a Stock Chart in PowerPoint using Python {#Create-a-Stock-Chart-in-PowerPoint}

Stock charts are also among the commonly used chart types in PowerPoint presentations. The following are the steps to create a stock chart in a PPT in Python.

*   First, create an instance of the **Presentation** class.
*   Get the reference of the slide from **Presentations.slides** in an object.
*   Add a Open High Low Close chart with default data using **Slide.shapes.add\_chart()** method.
*   Clear the default series and categories.
*   Access the chart data workbook into an object using **Chart.chart\_data.chart\_data\_workbook()** method.
*   Add new series and categories to the chart.
*   Access each chart series and add data points.
*   Specify Hi Low Lines format.
*   Finally, save the presentation using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to add a stock chart to PowerPoint PPTX in Python.

{{< gist aspose-com-gists de5345d7b26f8e48dc5eac6787835b70 "add-stock-chart.py" >}}

The following is the screenshot of the created stock chart.



{{< figure align=center src="images/stock-chart.jpg" alt="create stock chart in powerpoint in Python">}}


## More about Charts {#More-about-Charts}

There are a lot of other charts that you can add to the PowerPoint presentations using Aspose.Slides for Python. To read more about the supported chart types, you can visit [this documentation article][10].

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][11] to try the library without evaluation limitations.

## Conclusion

In this article, you have learned how to create charts in PowerPoint PPT or PPTX in Python. We have gone through the steps and code samples of how to add column charts, scatter charts, pie charts, histograms, and stock charts. You can explore more about Aspose.Slides for Python using [documentation][12]. In case you would have any questions or queries, let us know via our [forum][13].

## See Also

*   [Create PowerPoint Files in Python][14]
*   [Convert PPTX to PDF in Python][15]
*   [Convert PPT to PNG in Python][16]
*   [PPT/PPTX to HTML in Python][17]
*   [Add Watermark in PowerPoint PPT in Python][18]




[1]: #API-to-Create-Charts-in-PowerPoint
[2]: #Create-Column-Chart-in-PowerPoint
[3]: #Create-Scattered-Chart-in-PowerPoint
[4]: #Add-Pie-Chart-in-PowerPoint
[5]: #Add-Histogram-Chart-in-PowerPoint
[6]: #Create-a-Stock-Chart-in-PowerPoint
[7]: #More-about-Charts
[8]: https://products.aspose.com/slides/python-net
[9]: https://pypi.org/project/aspose.slides/
[10]: https://docs.aspose.com/slides/python-net/create-chart/
[11]: https://purchase.aspose.com/temporary-license
[12]: https://docs.aspose.com/slides/python-net/
[13]: https://forum.aspose.com/
[14]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[15]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/
[16]: https://blog.aspose.com/2021/12/29/convert-ppt-to-png-in-python/
[17]: https://blog.aspose.com/2021/12/16/convert-ppt-to-html-in-python/
[18]: https://blog.aspose.com/2022/02/09/add-watermark-to-powerpoint-ppt-in-python/




