---
title: 'Create or Edit Excel Files on Linux using .NET'
seoTitle: "Create Edit Excel Files in Linux | .NET Spreadsheet API for Linux"
description: "Learn how to create Excel XLSX and XLS files on Linux using .NET API. Add data to existing Excel files and generate charts and tables."
date: Wed, 20 Oct 2021 10:00:13 +0000
draft: false
url: /2021/10/20/create-or-edit-excel-files-on-linux/
author: Usman Aziz
summary: 'The emergence of automated solutions these days has made spreadsheet automation popular in various industries. The spreadsheet documents are created and manipulated programmatically from within the web or desktop solutions. Accordingly, this article covers **how to create Excel [XLSX][1] and [XLS][2] files on the Linux platform using .NET**.'
tags: ['create excel files on linux', 'create xls files on linux', 'create xlsx files on linux', 'edit excel files on linux']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/C-Excel-Automation-Library.png" alt="Create Excel File in Linux">}}


The emergence of automated solutions these days has made spreadsheet automation popular in various industries. The spreadsheet documents are created and manipulated programmatically from within the web or desktop solutions. Accordingly, this article covers **how to create Excel [XLSX][3] and [XLS][4] files on the Linux platform using .NET**.

*   [API to Create Excel Files on Linux][5]
*   [Create Excel XLS or XLSX Files on Linux][6]
*   [Write Data to Existing Excel Files][7]
*   [Create Charts in an Excel File][8]
*   [Create a Table in an Excel File][9]

## API to Create Excel Files on Linux {#Excel-Automation-API}

To create or edit Excel files on Linux, we will use [Aspose.Cells for .NET][10]. It is a feature-rich class library to create, manipulate, and convert Excel files. In order to use the API on Linux, you would need to install the following prerequisites.

*   [Visual Studio Code][11]
*   [C# Extension][12]
*   [.NET 5.0 SDK][13]

If you are new to .NET development on Linux, read [how to create a console application on Linux][14] using Visual Studio Code.

For the installation of Aspose.Cells for .NET in your application, you can use the [NuGet Package Manager extension][15] for Visual Studio Code. The package of the API is hosted on [NuGet][16].

## Create an Excel XLS or XLSX on Linux {#Create-Excel-XLS-or-XLSX-files-dynamically}

The Excel files are termed as the workbooks, which contain one or more worksheets. These worksheets are further divided into cells. Aspose.Cells for .NET uses the same naming convention to work with the Excel files. The following are the steps to create a new Excel file from scratch on Linux.

*   Create an instance of [Workbook][17] class.
*   Get reference of the first worksheet (created by default) of the workbook using [Workbook.Worksheets][18] collection.
*   Get reference of the desired cell from [Worksheet.Cells][19] collection using cell's name.
*   Add or update the cell's value.
*   Save the workbook using [Workbook.Save(string, SaveFormat)][20] method.

The following code sample shows how to create an Excel XLSX file on Linux.

{{< gist aspose-com-gists 07bc55e2c1eaaa5800d7c835df231e06 "create-excel-worksheets-csharp.cs" >}}

### Output



{{< figure align=center src="images/Create-Excel-Worksheet-in-C.png" alt="Create Excel Files on Linux" caption="Screenshot of the Excel file created using Aspose.Cells">}}


## Write Data to an Excel XLSX File on Linux {#Write-data-to-the-existing-Excel-file}

Aspose.Cells for .NET also allows you to write data to an existing Excel file. For this, you can initialize the Workbook object with the Excel file's path and manipulate the desired worksheets and cells. The following are the steps to edit an existing Excel file on Linux.

*   Create an instance of [Workbook][21] and initialize it with Excel file's path.
*   Use [Worksheet][22] and [Cell][23] classes to access the worksheets and cells in the Excel file, respectively.
*   Save the workbook using [Workbook.Save(string, SaveFormat)][24] method.

The following code sample shows how to edit and write data to an existing Excel XLSX file on Linux.

{{< gist aspose-com-gists 07bc55e2c1eaaa5800d7c835df231e06 "edit-excel-worksheets-csharp.cs" >}}

## Create Charts in Excel XLSX File on Linux {#Create-charts-or-graphs-in-an-Excel-file}

You can also generate graphs and charts to visualize the data in the spreadsheets. Aspose.Cells for .NET provides a complete set of classes to create and manipulate a [variety of charts][25] in Excel spreadsheets where each class is used to perform some specific tasks.

The following are the steps to create a chart in Excel file on Linux.

*   Create an Excel file using [Workbook][26] class.
*   Add some data to the worksheet by accessing its cells.
*   Add a new chart object to the worksheet using [Worksheet.Charts][27] collection by passing the type of chart using the [ChartType][28] enumeration.
*   Get the newly created chart from the collection in a [Chart][29] object.
*   Specify the cells' range to provide the data source to the chart object.
*   Save the workbook using [Workbook.Save(string, SaveFormat)][30] method.

The following code sample shows how to create a chart in an Excel XLSX file on Linux.

{{< gist aspose-com-gists 07bc55e2c1eaaa5800d7c835df231e06 "create-charts-in-excel-worksheets-csharp.cs" >}}

### Output



{{< figure align=center src="images/Create-Chart-in-Excel-Worksheet-in-C.png" alt="Create chart in Excel on Linux" caption="Chart generated using Aspose.Cells">}}


[Learn more][31] about creating charts in Excel worksheets.

## Create a Table in Excel XLSX File on Linux {#Create-a-table-in-an-Excel-file}

Aspose.Cells for .NET also provides an easy way to create a table from the range of cells in the worksheet. Also, you can add a row for the total in the table. The following are the steps to create a table in an Excel file.

*   Load an Excel workbook or create a new one using [Workbook][32] class.
*   Add data to the cells of the worksheet.
*   Add a new [ListObject][33] to the worksheet.
*   Set [ListObject.ShowTotals][34] property to _true_.
*   Calculate the total and save the workbook as an Excel file.

The following code sample shows how to create a table in an Excel file on Linux.

{{< gist aspose-com-gists 07bc55e2c1eaaa5800d7c835df231e06 "create-table-in-excel-worksheets-csharp.cs" >}}

### Output



{{< figure align=center src="images/Create-Table-in-Excel-Worksheet-in-C.png" alt="Create table in Excel Worksheet on Linux">}}


[Learn more][35] about working with tables in Excel worksheets.

## Explore Aspose.Cells for .NET

Aspose.Cells for .NET provides a complete package to create and manipulate simple as well as complex Excel files. You can read more about other features of the API using the [documentation][36].

## Get a Free License {#Get-a-Free-License}

You can get a [temporary license][37] and use Aspose.Cells for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to create Excel files from scratch on Linux. Moreover, you have seen how to add data and create charts and tables in Excel files. This article just covered some basic features of the API. However, you can explore other features by consulting the [documentation][38]. In case you would have any queries, you can ask us via our [forum][39].

## See Also

*   [Convert Excel Files to PDF on Linux using .NET][40]
*   [Import Data from JSON to Excel on Linux using .NET][41]




[1]: https://docs.fileformat.com/spreadsheet/xlsx/
[2]: https://docs.fileformat.com/spreadsheet/xl/
[3]: https://docs.fileformat.com/spreadsheet/xlsx/
[4]: https://docs.fileformat.com/spreadsheet/xl/
[5]: #Excel-Automation-API
[6]: #Create-Excel-XLS-or-XLSX-files-dynamically
[7]: #Write-data-to-the-existing-Excel-file
[8]: #Create-charts-or-graphs-in-an-Excel-file
[9]: #Create-a-table-in-an-Excel-file
[10]: https://products.aspose.com/cells/net
[11]: https://code.visualstudio.com/
[12]: https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp
[13]: https://dotnet.microsoft.com/download
[14]: https://docs.microsoft.com/en-us/dotnet/core/tutorials/with-visual-studio-code
[15]: https://marketplace.visualstudio.com/items?itemName=jmrog.vscode-nuget-package-manager
[16]: https://www.nuget.org/packages/Aspose.Cells
[17]: https://apireference.aspose.com/net/cells/aspose.cells/workbook
[18]: https://apireference.aspose.com/cells/net/aspose.cells/workbook/properties/worksheets
[19]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet/properties/cells
[20]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/3
[21]: https://apireference.aspose.com/net/cells/aspose.cells/workbook
[22]: https://apireference.aspose.com/net/cells/aspose.cells/worksheet
[23]: https://apireference.aspose.com/net/cells/aspose.cells/cell
[24]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/3
[25]: https://apireference.aspose.com/net/slides/aspose.slides.charts/charttype
[26]: https://apireference.aspose.com/net/cells/aspose.cells/workbook
[27]: https://apireference.aspose.com/net/cells/aspose.cells/worksheet/properties/charts
[28]: https://apireference.aspose.com/net/slides/aspose.slides.charts/charttype
[29]: https://apireference.aspose.com/net/slides/aspose.slides.charts/chart
[30]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/3
[31]: https://docs.aspose.com/cells/net/charts/
[32]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[33]: https://apireference.aspose.com/net/cells/aspose.cells.tables/listobject
[34]: https://apireference.aspose.com/net/cells/aspose.cells.tables/listobject/properties/showtotals
[35]: https://docs.aspose.com/cells/net/tables/
[36]: https://docs.aspose.com/cells/net/developer-guide/
[37]: https://purchase.aspose.com/temporary-license
[38]: https://docs.aspose.com/cells/net/developer-guide/
[39]: https://forum.aspose.com/
[40]: https://blog.aspose.com/2021/10/12/convert-excel-files-to-pdf-on-linux/
[41]: https://blog.aspose.com/2021/09/16/import-data-from-json-to-excel-on-linux/




