---
title: 'Create Sunburst and Treemap Charts in PowerPoint Presentations using Java'
date: Sat, 28 Dec 2019 05:34:16 +0000
draft: false
url: /2019/12/28/create-format-sunburst-or-treemap-charts-in-powerpoint-in-java/
author: Usman Aziz
summary: ''
tags: ['Aspose.Slides for Java', 'Format Sunburst chart', 'Format Treemap Chart', 'create sunburst chart in java', 'create treemap chart in java', 'sunburst chart in powerpoint', 'treemap chart in powerpoint']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/aspose_slides-for-java.jpg" alt="create sunburst and treemap chart in PowerPoint in Java">}}


The **Sunburst** charts are used to visually represent the hierarchical data structures in the form of multiple rings where each ring represents a level in the hierarchy. The **Treemap** is another type of chart to represent the hierarchical data to compare proportions within the hierarchy. [Aspose.Slides for Java][1] provides easy ways to **create Sunburst** and **Treemap** charts in **PowerPoint** presentations in **Java**. In the [latest release][2], we have extended this feature and now along with creating Sunburst and Treemap charts, you can **format the data points** as well. Let's check out how to create a Sunburst or Treemap chart and format the data points to apply different colors in Java.

## Create a Sunburst Chart in PowerPoint in Java

Let's first create a Sunburst chart in a PowerPoint presentation using Aspose.Slides for Java. The following are the steps required for this operation:

*   Create an instance of the [Presentation][3] class.
*   Get a slide's reference by index.
*   Add [ChartType.Sunburst][4] chart with default data.
*   Save the presentation to a PPTX file.

The following code sample shows how to create a Sunburst chart in a PowerPoint presentation in Java.

\[gist id="322d1ede29e94f5536291ce0d2dc1efe" file="Create-Sunburst-Chart-in-PowerPoint-in-Java.java"\]

### Output



{{< figure align=center src="images/Sunburst_Simple.png" alt="">}}


## Create a Treemap Chart in PowerPoint in Java {#mce_2}

Similar to the Sunburst chart, you can also create a Treemap chart in a few steps in Java using Aspose.Slides for Java. All the steps for creating a Treemap chart will be the same except for the chart type. The following code sample shows how to create a Treemap chart in a PowerPoint presentation in Java.

\[gist id="322d1ede29e94f5536291ce0d2dc1efe" file="Create-Treemap-Chart-in-PowerPoint-in-Java.java" \]

### Output



{{< figure align=center src="images/Treemap-in-PowerPoint.png" alt="">}}


## Format Data Point Label of Sunburst Chart in Java

Using the latest release of Aspose.Slides for Java, you will be able to format the data point labels of a Sunburst or Treemap chart programmatically in Java. For the demonstration, we'll format the labels in the Sunburst chart type only. You can perform formatting to the Treemap chart in a similar way.

### Change Data Point Label Color

Let's assume that you want to change the color of the data label of "Branch 1" in the Sunburst chart we have previously created. To accomplish this, we have added **[IChartDataPointLevelsManager][5]** and **[IChartDataPointLevel][6]** classes to get access to properties of data point levels.

The following code sample shows how to change the color of the data label of "Branch 1" in the Sunburst chart using Java.

\[gist id="322d1ede29e94f5536291ce0d2dc1efe" file="Format-DataLabel-Sunburst-Chart-in-PowerPoint-in-Java.java" \]

#### **Output**



{{< figure align=center src="images/Sunburst_FormatDataPointLabel.png" alt="">}}


### Change Data Point Branch Color

You can also change the color of a specific data point branch in the Sunburst chart. The following Java code sample shows how to change the color of the "Steam 4" branch.

\[gist id="322d1ede29e94f5536291ce0d2dc1efe" file="Format-Branch-Sunburst-Chart-in-PowerPoint-in-Java.java" \]

#### **Output**



{{< figure align=center src="images/Sunburst_FormatDataPointBranch.png" alt="">}}


For more details on how to format charts in PowerPoint presentations, please visit [formatting charts][7].

You can download the complete source code examples of Aspose.Slides for Java from [GitHub][8]. In case you would find any issue, please feel free to let us know via our [forum][9].



[1]: https://products.aspose.com/slides/java
[2]: https://downloads.aspose.com/slides/java/new-releases/aspose.slides-for-java-19.12/
[3]: https://apireference.aspose.com/java/slides/com.aspose.slides/Presentation
[4]: https://apireference.aspose.com/java/slides/com.aspose.slides/ChartType#Sunburst
[5]: https://apireference.aspose.com/java/slides/com.aspose.slides/IChartDataPointLevelsManager
[6]: https://apireference.aspose.com/java/slides/com.aspose.slides/IChartDataPointLevel
[7]: https://docs.aspose.com/display/slidesjava/Formatting+Charts#FormattingCharts-FormattingChartEntities
[8]: https://github.com/aspose-slides/Aspose.Slides-for-Java
[9]: https://forum.aspose.com/c/slides




