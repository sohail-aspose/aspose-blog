---
title: 'Add VBA Modules and Create Chart in Excel'
date: Mon, 25 May 2015 10:55:37 +0000
draft: false
url: /2015/05/25/add-vba-modules-create-chart/
author: Babar Raza
summary: ''
tags: ['Babar Raza', 'Chart in excel', 'Create Charts and Shapes in Excel', 'VBA in Excel', 'create charts and graphs in excel']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="VBA in Excel">}}


We are pleased to announce the monthly release of Aspose.Cells for Java, version 8.4.2. This month's release contains many useful features & enhancements, where most worth mentioning feature of this release is the support for adding VBA modules to the spreadsheet. In case you are planning to upgrade the API from any previous revision, we strongly suggest you to go through the Public API Changes section first to know what has been changed since your current version of the API.

You may start exploring the newly added features, however, before you head to the [download section][1] here is a look at just a few of the showcased features of this release. For a full list of bug fixes and improvements please refer to the download page in the link above.

## Adding VBA Modules to Spreadsheet

Starting with this release, Aspose.Cells for Java has provided support for adding VBA modules to the spreadsheets. Aspose.Cells for Java 8.4.2 has exposed the VbaModuleCollection.add method to add a new VBA module to the instance of Workbook. The VbaModuleCollection.add method accepts a parameter of type Worksheet to add a worksheet specific module, whereas the existing VbaModule class contains all the module specific properties.

The following code snippet shows how to use the VbaModuleCollection.add method.

```
//Create new workbook
Workbook workbook = new Workbook();

//Access first worksheet
Worksheet worksheet = workbook.getWorksheets().get(0);

//Add VBA module
int idx = workbook.getVbaProject().getModules().add(worksheet);

//Access the VBA Module, set its name and code
VbaModule module = workbook.getVbaProject().getModules().get(idx);
module.setName("TestModule");

module.setCodes("Sub ShowMessage()" + "\\r\\n" +
"    MsgBox \\"Welcome to Aspose!\\"" + "\\r\\n" +
"End Sub");

//Save the workbook
workbook.save(output, SaveFormat.XLSM);

```

## Improved Chart Creation Mechanism

Aspose.Cells for Java 8.4.2 has exposed simplified mechanism to create charts on the fly. Please note, the conventional means of creating charts involves several steps that may include, but not limited to specifying the series and category axis data ranges separately. With new mechanism, all you have to do is to specify the chart's data range while using the Chart.setChartDataRange method.

The setChartDataRange method accepts two parameters, where first parameter is of type String in order to specify the cell area from which to plot the data series. The second parameter is of type Boolean that specifies the plot orientation, that is; whether to plot the chart data series from a range of cell values by row or by columns.

The following code snippet shows how to create a column chart with few lines of code assuming that the chart's plot series data is present on the same worksheet from cell A1 to D4.

```
//Add a new chart of type Column to the chart collection
int idx = worksheet.getCharts().add(ChartType.COLUMN, 6, 5, 20, 13);

//Retrieve the newly added chart instance
Chart chart = worksheet.getCharts().get(idx);

//Specify the chart's data series from cell A1 to D4
chart.setChartDataRange("A1:D4", true);

```

## Other Enhancements & Fixes

Aspose.Cells for Java 8.4.2 has fixed a number of issues and enhanced the core to accommodate many customer requests. Following are a few worth mentioning enhancements & fixes.

*   Provided support for IFNA function.
*   Added an overloaded version of Cells.copyColumns method that can be used to repeat the source columns onto the destination while copy operation.
*   Exposed 2 new fields for the PasteType enumeration in order to mimic the Excel's 'All' & 'All except borders' functionality for pasting range of cells.
*   Improved the PDF rendering engine to handle cases that involve WordArt, shapes and uppercase characters converted through Excel's 'All caps' functionality.
*   Improved Chart2Image functionality for EMF file format to correctly render axis and data labels.
*   Addressed a few exceptions related to the spreadsheets loading & saving mechanism of Aspose.Cells for Java API.

Please visit the documentation for details, and if you still have any questions, we always welcome inquiries on [Aspose.Cells Support Forum][2].




[1]: http://www.aspose.com/community/files/72/java-components/aspose.cells-for-java/entry628881.aspx "Download Aspose.Cells for Java 8.4.2"
[2]: https://forum.aspose.com/




