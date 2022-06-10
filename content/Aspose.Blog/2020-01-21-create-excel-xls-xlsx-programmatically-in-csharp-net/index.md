---
title: 'Create MS Excel Files Programmatically in C# without MS Office'
seoTitle: "How to Create Excel XLSX Files in C# | Create Charts and Tables in Excel"
description: "Create Excel XLSX files using C# programmatically without MS Office or MS Excel. Create an Excel file with charts, graphs, and tables in C# ASP.NET."
date: Tue, 21 Jan 2020 13:11:07 +0000
draft: false
url: /2020/01/21/create-excel-xls-xlsx-programmatically-in-csharp-net/
author: Usman Aziz
summary: ''
tags: ['Excel Automation API', 'Excel Library for .NET', 'create charts and graphs in excel', 'create excel files in csharp .net', 'create excel files programmatically', 'create excel files without ms office', 'create tables in excel files in C# .net']
categories: ['Aspose.Cells Product Family']
---

In this article, you will learn how to **create Excel XLS/XLSX files programmatically in C#** without installing MS Office.



{{< figure align=center src="images/C-Excel-Automation-Library.png" alt="Create Excel File in C# API">}}


**Spreadsheets** nowadays have become an essential part of keeping, organizing and analyzing the data. Spreadsheets, such as **MS Excel**, are capable of doing calculations and sorting, generating graphs or charts, creating budgets, and performing many other accounting or data analysis tasks. Since **automated solutions** are more in business these days, the trend of creating and manipulating Excel documents (XLS/XLSX) has emerged and growing at a huge pace. This use case has raised the need for having an **Excel automation** solution.

In accordance with the above-mentioned scenario, this comprehensive article aims to show you some basic features for **Excel automation** in **C# .NET** applications.

*   [C# Excel Automation API][1]
*   [Create Excel XLS or XLSX files dynamically using C#][2]
*   [Write data to the existing Excel file using C#][3]
*   [Create charts or graphs in an Excel file using C#][4]
*   [Create a table in an Excel file using C#][5]

## C# API to Create Excel Files {#CSharp-Excel-Automation-API}

In order to work with Excel documents, we will use [Aspose.Cells for .NET][6] which is a powerful API to create, read, and manipulate spreadsheet documents including **XLS** and **XLSX** files. You can either [download][7] or install the API using one of the following ways:

### Using NuGet Package Manager



{{< figure align=center src="images/Aspose.Cells-NuGet.png" alt="C# Excel Automation Library ">}}


### Using the Package Manager Console```
PM> Install-Package Aspose.Cells
```

## Create an Excel XLS or XLSX in C# {#Create-Excel-XLS-or-XLSX-files-dynamically-using-CSharp}

An Excel file is also known as a **Workbook** which is composed of single or multiple worksheets containing the rows and columns to hold the data. Thus, a workbook acts as the container of the worksheets in an Excel file. So in order to create an Excel file, you will first create a workbook and then the worksheets within that workbook. The following are the steps to create an Excel file using _Aspose.Cells for .NET_.

*   Create an instance of [Workbook][8] class.
*   Access the first worksheet (created by default) of the workbook.
*   Access the desired cell(s) of the worksheet and put the value in the cell(s).
*   Save the workbook as an XLS or XLSX file.

The following code sample shows how to create an Excel XLSX file using C#.

{{< gist aspose-com-gists e5148ce4baea9950cfc46c674b56b29b "create-excel-worksheets-csharp.cs" >}}

### Output



{{< figure align=center src="images/Create-Excel-Worksheet-in-C.png" alt="Create Excel Files in C#">}}


## Write Data to an Excel XLSX File in C# {#Write-data-to-the-existing-Excel-file-using-CSharp}

In case you want to edit and write data to an existing Excel file, you can also do it in a similar fashion. Simply load the source Excel spreadsheet document using the Workbook object and access the desired worksheets and cells. The following are the steps to edit an existing Excel file.

*   Open Excel file in a _FileStream_ object.
*   Create an instance of [Workbook][9] and initialize it with the _FileStream_ object.
*   Access the worksheets and cells using the [Worksheet][10] and [Cell][11] classes respectively.
*   Save the workbook as an Excel _.xlsx_ file.

The following code sample shows how to edit and write data to an existing Excel XLSX file in C#.

{{< gist aspose-com-gists e5148ce4baea9950cfc46c674b56b29b "edit-excel-worksheets-csharp.cs" >}}

## Create Charts or Graphs in Excel XLSX File using C# {#Create-charts-or-graphs-in-an-Excel-file-using-CSharp}

Excel spreadsheets provide a fine way of analyzing or presenting the data visually using the graphs and charts. _Aspose.Cells for .NET_ provides a complete set of classes to create and manipulate a [variety of charts][12] in Excel spreadsheets where each class is used to perform some specific tasks.

In order to create the charts in an Excel file, you'll have to follow the following steps:

*   Add some data (to be used as a data source) to the worksheet by accessing its cells.
*   Add a new chart object to the worksheet using [Worksheet.Charts][13] collection by passing the type of chart using the [ChartType][14] enumeration.
*   Get the newly created chart from the collection in a [Chart][15] object.
*   Specify the cells' range to provide the data source to the chart object.
*   Save the workbook as an Excel _.xlsx_ file.

The following code sample shows how to create a chart in an Excel XLSX file in C#.

{{< gist aspose-com-gists e5148ce4baea9950cfc46c674b56b29b "create-charts-in-excel-worksheets-csharp.cs" >}}

### Output



{{< figure align=center src="images/Create-Chart-in-Excel-Worksheet-in-C.png" alt="Create chart in Excel in C#">}}


[Learn more][16] about creating charts in Excel worksheets using C#.

## Create a Table in Excel XLSX File in C# {#Create-a-table-in-an-Excel-file-using-CSharp}

You can also create a table from the range of cells in an Excel worksheet and add a row for the total (sum, count, etc.) in the table. The following are the steps to create a table in an Excel (XLSX) file using Aspose.Cells for .NET:

*   Load an Excel workbook or create a new one using _Workbook_ class.
*   Add data to the cells of the worksheet.
*   Add a new [ListObject][17] to the worksheet.
*   Set [ListObject.ShowTotals][18] property to _true_.
*   Calculate the total and save the workbook as an Excel _.xlsx_ file.

The following code sample shows how to create a table in Excel worksheet in C#.

{{< gist aspose-com-gists e5148ce4baea9950cfc46c674b56b29b "create-table-in-excel-worksheets-csharp.cs" >}}

### Output



{{< figure align=center src="images/Create-Table-in-Excel-Worksheet-in-C.png" alt="Create table in Excel Worksheet in C#">}}


[Learn more][19] about working with tables in Excel worksheets using C#.

## Conclusion

In this article, you have learned how to create Excel files from scratch using C#. Furthermore, you have seen how to insert data in sheets, generate charts, and insert tables in Excel files. You may have a look at the [documentation][20] of _Aspose.Cells for .NET_ to learn the advanced features for manipulation of Excel files in C#.

## Related Article

*   [Create and Sort Pivot Tables in Excel Worksheets][21]
*   [Create Excel Files in Node.js Applications][22]




[1]: #CSharp-Excel-Automation-API
[2]: #Create-Excel-XLS-or-XLSX-files-dynamically-using-CSharp
[3]: #Write-data-to-the-existing-Excel-file-using-CSharp
[4]: #Create-charts-or-graphs-in-an-Excel-file-using-CSharp
[5]: #Create-a-table-in-an-Excel-file-using-CSharp
[6]: https://products.aspose.com/cells/net
[7]: https://downloads.aspose.com/cells/net
[8]: https://apireference.aspose.com/net/cells/aspose.cells/workbook
[9]: https://apireference.aspose.com/net/cells/aspose.cells/workbook
[10]: https://apireference.aspose.com/net/cells/aspose.cells/worksheet
[11]: https://apireference.aspose.com/net/cells/aspose.cells/cell
[12]: https://apireference.aspose.com/net/slides/aspose.slides.charts/charttype
[13]: https://apireference.aspose.com/net/cells/aspose.cells/worksheet/properties/charts
[14]: https://apireference.aspose.com/net/slides/aspose.slides.charts/charttype
[15]: https://apireference.aspose.com/net/slides/aspose.slides.charts/chart
[16]: https://docs.aspose.com/cells/net/charts/
[17]: https://apireference.aspose.com/net/cells/aspose.cells.tables/listobject
[18]: https://apireference.aspose.com/net/cells/aspose.cells.tables/listobject/properties/showtotals
[19]: https://docs.aspose.com/cells/net/tables/
[20]: https://docs.aspose.com/display/cellsnet/Developer+Guide
[21]: https://blog.aspose.com/2020/01/10/create-pivot-tables-in-excel-sort-hide-pivot-table-data-programmatically/
[22]: https://blog.aspose.com/2020/08/05/create-excel-files-in-node.js/





