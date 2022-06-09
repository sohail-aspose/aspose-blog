---
title: 'Create Pivot Tables in Excel using Java'
seoTitle: "Create Pivot Table in Excel in Java | Create Chart from Pivot Table"
description: "Use Java Excel API to create a pivot table in Excel worksheets using Java. Generate charts using the pivot tables programmatically using Java."
date: Mon, 26 Apr 2021 18:58:05 +0000
draft: false
url: /2021/04/26/create-pivot-tables-in-excel-using-java/
author: Usman Aziz
summary: 'Pivot tables in Excel spreadsheets are used to summarize the data in an interactive way. Suppose, you have the data of a number of invoices in a worksheet. In that case, you can use a pivot table to total the invoices grouped by the customers or products. In this article, you will learn how to deal with pivot tables in Excel programmatically. Particularly, you will come to know **how to create a pivot table and generate a chart based on that pivot table in Java**.'
tags: ['Create a Pivot Table in Excel using Java', 'Generate Chart using Pivot Table', 'Java API to Work with Excel Pivot Tables']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Excel-File.png" alt="">}}


Pivot tables in Excel spreadsheets are used to summarize the data in an interactive way. Suppose, you have the data of a number of invoices in a worksheet. In that case, you can use a pivot table to total the invoices grouped by the customers or products. In this article, you will learn how to deal with pivot tables in Excel programmatically. Particularly, you will come to know **how to create a pivot table in Excel using Java.** Furthermore, we will also generate charts based on the pivot table.

*   [Java API to Work with Excel Pivot Tables][1]
*   [Create a Pivot Table in Excel][2]
*   [Generate Chart using a Pivot Table][3]
*   [Get a Free API License][4]

## Java API to Create Pivot Table in Excel {#Java-API-to-Work-with-Excel-Pivot-Tables}

In order to create Excel pivot table, we'll use [Aspose.Cells for Java][5]. It is a powerful API that lets you generate, modify and convert Excel files from within your Java applications. You can either [download][6] the API or install it using the following Maven configurations.

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
    <version>21.4</version>
</dependency>
```

## Create a Pivot Table in Excel using Java {#Create-a-Pivot-Table-in-Excel-using-Java}

The following are the steps to create a pivot table in Excel using Java.

*   Create a new or load an existing Excel file using the [Workbook][7] class.
*   Populate the worksheet with data (optional).
*   Get collection of pivot tables into a [PivotTableCollection][8] object using [Worksheet.getPivotTables()][9] method.
*   Add a new pivot table using [PivotTableCollection.add(string, string, string)][10] method, and get its reference in a [PivotTable][11] object.
*   Set options such as grand total, formatting, etc.
*   Add fields to area using [PivotTable.addFieldToArea(int, int)][12] method.
*   Save the workbook using [Workbook.save(string)][13] method.

The following code sample shows how to add a pivot table in Excel.

{{< gist aspose-com-gists 619c240a0fdeeaf0db0bae5d390ae3de "create-pivot-table.java" >}}

### Excel Data



{{< figure align=center src="images/Create-Pivot-Table.jpg" alt="Data source for excel pivot table">}}


### Pivot Table



{{< figure align=center src="images/Excel-Pivot-Table.jpg" alt="create pivot table in excel in java">}}


## Generate a Chart using Excel Pivot Tables in Java {#Generate-Chart-using-Pivot-Table}

The following are the steps to generate a chart using Excel pivot tables in Java.

*   Create a new or load an existing Excel file using the [Workbook][14] class.
*   Populate the worksheet (optional).
*   Add a new worksheet of chart type using [Workbook.getWorksheets().add(SheetType.CHART)][15] and get its reference in a [Worksheet][16] object.
*   Add a new chart using [Worksheet.getCharts().add()][17] method and get its reference in a [Chart][18] object.
*   Set pivot table as the data source of chart using [Chart.setPivotSource(string)][19] method.
*   Save the workbook using [Workbook.save(string)][20] method.

The following code sample shows how to generate a chart using an Excel pivot table.

{{< gist aspose-com-gists 619c240a0fdeeaf0db0bae5d390ae3de "create-chart-from-pivot-table.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [get a free temporary license][21] to use the API without evaluation limitations.

## Conclusion

In this article, you have learned how to create a pivot table in Excel using Java. Furthermore, you have seen how to generate charts using the pivot tables in Excel. You can explore more about Java Excel API using [documentation][22]. In case you would have any questions, feel free to let us know via our [forum][23].

## See Also

*   [Create Excel XLSX or XLS Files in Java][24]




[1]: #Java-API-to-Work-with-Excel-Pivot-Tables
[2]: #Create-a-Pivot-Table-in-Excel-using-Java
[3]: #Generate-Chart-using-Pivot-Table
[4]: #Get-a-Free-API-License
[5]: https://products.aspose.com/cells/java
[6]: https://downloads.aspose.com/cells/java
[7]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[8]: https://apireference.aspose.com/cells/java/com.aspose.cells/PivotTableCollection
[9]: https://apireference.aspose.com/cells/java/com.aspose.cells/worksheet#PivotTables
[10]: https://apireference.aspose.com/cells/java/com.aspose.cells/pivottablecollection#add(java.lang.String,%20java.lang.String,%20java.lang.String)
[11]: https://apireference.aspose.com/cells/java/com.aspose.cells/PivotTable
[12]: https://apireference.aspose.com/cells/java/com.aspose.cells/pivottable#addFieldToArea(int,%20int)
[13]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String)
[14]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[15]: https://apireference.aspose.com/cells/java/com.aspose.cells/worksheetcollection#add(int)
[16]: https://apireference.aspose.com/cells/java/com.aspose.cells/Worksheet
[17]: https://apireference.aspose.com/cells/java/com.aspose.cells/chartcollection#add(int,%20int,%20int,%20int,%20int)
[18]: https://apireference.aspose.com/cells/java/com.aspose.cells/Chart
[19]: https://apireference.aspose.com/cells/java/com.aspose.cells/chart#PivotSource
[20]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String)
[21]: https://purchase.aspose.com/temporary-license
[22]: https://docs.aspose.com/cells/java/getting-started/
[23]: https://forum.aspose.com/
[24]: https://blog.aspose.com/2020/10/13/create-excel-xlsx-xls-using-java-without-ms-office/





