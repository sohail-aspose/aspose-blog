---
title: 'Read Gantt Chart of Project using Java'
seoTitle: "Read Gantt Chart of Project using Java | Read Gantt Chart View in Java"
description: "Programmatically, read Gantt Chart of MS Project using Java with Aspose.Tasks for Java API. Read Bar styles, gridlines, timescale tiers, and progress lines."
date: Wed, 08 Jun 2022 10:58:26 +0000
draft: false
url: /2022/06/08/read-gantt-chart-of-project-using-java/
author: Muzammil Khan
summary: 'The Gantt chart view is the default view of the project. It lists project tasks, their relationship to one another, and the schedule of the project. In this article, you will learn **how to read the Gantt chart of the MS project using Java**.'
tags: ['gantt chart in ms project', 'gantt chart view', 'java api to read gantt chart', 'read gantt chart', 'read gantt chart view', 'read gantt chart view in java', 'what is gantt chart']
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/read-gantt-chart-of-project-using-java-1.jpg" alt="Read Gantt Chart of Project using Java">}}


MS Project is a popular project management software, widely used to organize, manage, and track project activities efficiently. It allows creating the tasks, adding resources, allocating tasks to resources, monitoring the progress, and managing budget-related activities. The Gantt chart view is the default view of the project. It lists project tasks and shows their relationship to one another. It also shows the schedule of the project using Gantt bars. In this article, we will learn **how to read the Gantt chart of the MS project using Java**.

The following topics shall be covered in this article:

*   [What is Gantt Chart in Microsoft Project][1]
*   [Java API to Read Gantt Chart of Project][2]
*   [Read Gantt Chart View and Retrieve Bar Styles][3]
*   [Read Grid Lines of Gantt Chart View][4]
*   [Extract Text Style of Gantt Chart View][5]
*   [Retrieve Progress Lines of Gantt Chart View][6]
*   [Read Bottom Timescale Tier][7]
*   [Read Middle Timescale Tier][8]
*   [Retrieve Top Timescale Tier][9]

## What is Gantt Chart in Microsoft Project {#What-is-Gantt-Chart-in-Microsoft-Project}

A Gantt chart is a type of bar chart that shows the project schedule. It is a graphical representation of project tasks against time and offers a bird's eye view of the entire project. The Gantt chart view in Microsoft Project shows the following:

*   Project schedule
*   Time estimates
*   Project resources & team members
*   Task priorities
*   Task dependency



{{< figure align=center src="images/What-is-Gantt-Chart-in-Microsoft-Project-1024x342.jpg" alt="" caption="Gantt Chart View of a Project in Microsoft Project.">}}


## Java API to Read Gantt Chart of Project {#Java-API-to-Read-Gantt-Chart-of-Project}

For reading the Gantt chart view of a Project from the [MPP][10] file, we will be using the [Aspose.Tasks for Java][11] API. It allows creating, editing, or manipulating Microsoft Project files programmatically in Java applications. The **_[Project][12]_** class of the API represents a project. It is the main class exposing various methods to perform different functions. It also allows reading one of the supported project management formats such as MPP, [MPT][13], [MPX][14], and [XML][15]. The **_[GanttChartView][16]_** class of the API represents a Gantt chart view. It exposes various properties and methods to work with the Gantt chart programmatically.

Please either [download][17] the JAR of the API or add the following _**pom.xml**_ configuration in a Maven-based Java application.

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
    <artifactId>aspose-tasks</artifactId>
    <version>22.5</version>
    <classifier>jdk18</classifier>
</dependency>
```

## Read Gantt Chart View and Retrieve Bar Styles {#Read-Gantt-Chart-View-and-Retrieve-Bar-Styles}

The _**[GanttBarStyle][18]**_ class of the API represents a bar-style used by MS Project in the Gantt chart view. We can read the Gantt chart view and retrieve the bar styles by following the steps given below:

1.  Firstly, load the project file using the **_Project_** class.
2.  Next, get the default view from the **_ViewCollection_** by its index.
3.  Then, create an instance of the **_GanttChartView_** class and typecast view.
4.  Optionally, read basic properties and show data.
5.  After that, get a list of bar styles of the Gantt chart view using the **_[getBarStyles()][19]_**.
6.  Finally, loop through bar styles as **_GanttBarStyle_** class object and show values.

The following code example shows **how to read bar styles of the Gantt chart view in Java**.

\[gist id="aad111c6fae7fc54d5eb2c13faafc15e" file="Read-Gantt-Chart-MS-Project-Java\_ReadBarStyles.java"\]

```
Bar Rounding: true
Show Bar Splits: true
Show Drawings: true
RollUp Gantt Bars: false
Hide Rollup Bars When Summary Expanded: false
Bar Size: 3
Bar Styles count: 40
-----------------------------------------------
Row: 1
Name: Task
ShowFor: null
From:TaskStart
To:TaskFinish
Middle Shape:RectangleBar
Middle Shape Color:java.awt.Color[r=0,g=0,b=255]
Start Shape:NoBarEndShape
End Shape:NoBarEndShape
End Shape Color:java.awt.Color[r=0,g=0,b=0]
-----------------------------------------------
...
```

## Read Grid Lines of Gantt Chart View in Java {#Read-Grid-Lines-of-Gantt-Chart-View-in-Java}

The **_[Gridlines][20]_** class of the API represents grid lines that appear in a Gantt chart view. We can read the grid line's color, interval, pattern, and type by following the steps given below:

1.  Firstly, load the project file using the **_Project_** class.
2.  Next, get the default view from the **_ViewCollection_** by its index.
3.  Then, create an instance of the **_GanttChartView_** class and typecast view.
4.  After that, get a list of Grid lines of the Gantt chart view using the **_[getGridlines()][21]_**.
5.  Finally, loop through grid lines as the **_Gridlines_** class object and show values.

The following code example shows **how to read grid lines of the Gantt chart view in Java**.

\[gist id="aad111c6fae7fc54d5eb2c13faafc15e" file="Read-Gantt-Chart-MS-Project-Java\_ReadGridLines.java"\]

```
Gridlines Count: 14
Gridlines Type: 3
Gridlines Interval: 0
Gridlines NormalColor: java.awt.Color[r=192,g=192,b=192]
Gridlines NormalPattern: Solid
Gridlines IntervalPattern: 0
Gridlines IntervalColor: java.awt.Color[r=192,g=192,b=192]
```

## Extract Text Style of Gantt Chart View in Java {#Extract-Text-Style-of-Gantt-Chart-View-in-Java}

The **_[TextStyle][22]_** class of the API represents the visual style of the text for an item in a Gantt chart view. We can read the color, background color, font, and font style by following the steps given below:

1.  Firstly, load the project file using the **_Project_** class.
2.  Next, get the default view from the **_ViewCollection_** by its index.
3.  Then, create an instance of the **_GanttChartView_** class and typecast view.
4.  After that, get a list of text styles of the Gantt chart view using the **_[get**_TextStyle_**s()][23]_**.
5.  Finally, initialize the **_**_TextStyle_**_** class object for the first text style and show values.

The following code example shows **how to read text styles of the Gantt chart view in Java**.

\[gist id="aad111c6fae7fc54d5eb2c13faafc15e" file="Read-Gantt-Chart-MS-Project-Java\_ReadTextStyle.java"\]

```
Text Styles Count: 19
Background Color: java.awt.Color[r=0,g=0,b=0]
Text Color: java.awt.Color[r=0,g=0,b=255]
Font Family: Arial
Font Size: 8.0
Font Style: Regular
```

## Retrieve Progress Lines of Gantt Chart View in Java {#Retrieve-Progress-Lines-of-Gantt-Chart-View-in-Java}

The progress lines appear on the Gantt Chart view showing whether tasks are behind, or right on schedule. We can read the various properties of the progress lines by following the steps given below:

1.  Firstly, load the project file using the **_Project_** class.
2.  Next, get the default view from the **_ViewCollection_** by its index.
3.  Then, create an instance of the **_GanttChartView_** class and typecast view.
4.  After that, get a list of progress lines of the Gantt chart view using the **_[getProgressLines()][24]_**.
5.  Finally, show progress line attribute values.

The following code example shows **how to read progress lines of the Gantt chart view in Java**.

\[gist id="aad111c6fae7fc54d5eb2c13faafc15e" file="Read-Gantt-Chart-MS-Project-Java\_ReadProgressLines.java"\]

## Read Bottom Timescale Tier in Java {#Read-Bottom-Timescale-Tier-in-Java}

Timescale shows time units, days, months, calendar year, or fiscal year. There are three [timescale tiers][25] in the project view to show the timescale values for each tier such as count, unit, label, alignment, etc. We can read the bottom timescale tier by following the steps given below:

1.  Firstly, load the project file using the **_Project_** class.
2.  Next, get the default view from the **_ViewCollection_** by its index.
3.  Then, create an instance of the **_GanttChartView_** class and typecast view.
4.  After that, get the settings of the view's bottom timescale tier using the **_[getBottomTimescaleTier()][26]_**.
5.  Finally, show bottom timescale tier values.

The following code example shows **how to read the bottom timescale tier of the Gantt chart view in Java**.

\[gist id="aad111c6fae7fc54d5eb2c13faafc15e" file="Read-Gantt-Chart-MS-Project-Java\_ReadBottomTimescaleTier.java"\]

```
BottomTimescaleTier Count: 2
BottomTimescaleTier Unit: Days
BottomTimescaleTier UsesFiscalYear: true
BottomTimescaleTier Alignment: Center
BottomTimescaleTier ShowTicks: true
BottomTimescaleTier Label: DayOfMonthDd
```

## Read Middle Timescale Tier in Java {#Read-Middle-Timescale-Tier-in-Java}

Similarly, we can read the middle timescale tier by following the steps mentioned earlier. However, we will get the settings of the view's middle timescale tier using the **_[getMiddleTimescaleTier()][27]_** in step 4.

The following code example shows **how to read the middle timescale tier of the Gantt chart view in Java**.

\[gist id="aad111c6fae7fc54d5eb2c13faafc15e" file="Read-Gantt-Chart-MS-Project-Java\_ReadMiddleTimescaleTier.java"\]

```
MiddleTimescaleTier.Count: 1
TimescaleUnit.Weeks: Months
MiddleTimescaleTier.Alignment: Center
MiddleTimescaleTier.ShowTicks: true
MiddleTimescaleTier.Label: MonthMmmmYyyy
```

## Retrieve Top Timescale Tier in Java {#Retrieve-Top-Timescale-Tier-in-Java}

We can also read the top timescale tier by following the steps mentioned earlier. However, we will get the settings of the view's top timescale tier using the **_[getTopTimescaleTier()][28]_** in step 4.

The following code example shows **how to read the top timescale tier of the Gantt chart view in Java**.

\[gist id="aad111c6fae7fc54d5eb2c13faafc15e" file="Read-Gantt-Chart-MS-Project-Java\_ReadTopTimescaleTier.java"\]

```
TopTimescaleTier Unit: Quarters
TopTimescaleTier UsesFiscalYear: true
TopTimescaleTier Alignment: Center
TopTimescaleTier ShowTicks: true
TopTimescaleTier Label: QuarterQtrQYyyy
```

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][29] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned how to

*   read the Gantt chart view programmatically in Java;
*   extract Gantt chart view's bar styles and text style;
*   retrieve grid lines and progress lines of the Gantt chart view;
*   read timescale units of Gantt chart view using Java.

Besides, you can learn more about **_Aspose.Tasks for Java_** API using the [documentation][30]. In case of any ambiguity, please feel free to contact us on the [forum][31].

## See Also

*   [Convert MPP to Excel using Java][32]


[1]: #What-is-Gantt-Chart-in-Microsoft-Project
[2]: #Java-API-to-Read-Gantt-Chart-of-Project
[3]: #Read-Gantt-Chart-View-and-Retrieve-Bar-Styles
[4]: #Read-Grid-Lines-of-Gantt-Chart-View-in-Java
[5]: #Extract-Text-Style-of-Gantt-Chart-View-in-Java
[6]: #Retrieve-Progress-Lines-of-Gantt-Chart-View-in-Java
[7]: #Read-Bottom-Timescale-Tier-in-Java
[8]: #Read-Middle-Timescale-Tier-in-Java
[9]: #Retrieve-Top-Timescale-Tier-in-Java
[10]: https://docs.fileformat.com/project-management/mpp/
[11]: https://products.aspose.com/tasks/java/
[12]: https://reference.aspose.com/tasks/java/com.aspose.tasks/project
[13]: https://docs.fileformat.com/project-management/mpt/
[14]: https://docs.fileformat.com/project-management/mpx/
[15]: https://docs.fileformat.com/project-management/p6xml/
[16]: https://reference.aspose.com/tasks/java/com.aspose.tasks/GanttChartView
[17]: https://downloads.aspose.com/tasks/java
[18]: https://reference.aspose.com/tasks/java/com.aspose.tasks/GanttBarStyle
[19]: https://reference.aspose.com/tasks/java/com.aspose.tasks/ganttchartview#getBarStyles()
[20]: https://reference.aspose.com/tasks/java/com.aspose.tasks/Gridlines
[21]: https://reference.aspose.com/tasks/java/com.aspose.tasks/ganttchartview#getGridlines()
[22]: https://reference.aspose.com/tasks/java/com.aspose.tasks/TextStyle
[23]: https://reference.aspose.com/tasks/java/com.aspose.tasks/ganttchartview#getTextStyles()
[24]: https://reference.aspose.com/tasks/java/com.aspose.tasks/ganttchartview#getProgressLines()
[25]: https://reference.aspose.com/tasks/java/com.aspose.tasks/TimescaleTier
[26]: https://reference.aspose.com/tasks/java/com.aspose.tasks/ganttchartview#getBottomTimescaleTier()
[27]: https://reference.aspose.com/tasks/java/com.aspose.tasks/ganttchartview#getMiddleTimescaleTier()
[28]: https://reference.aspose.com/tasks/java/com.aspose.tasks/ganttchartview#getTopTimescaleTier()
[29]: https://purchase.aspose.com/temporary-license
[30]: https://docs.aspose.com/tasks/java/
[31]: https://forum.aspose.com/c/tasks/
[32]: https://blog.aspose.com/2022/05/10/convert-mpp-to-excel-using-java/





