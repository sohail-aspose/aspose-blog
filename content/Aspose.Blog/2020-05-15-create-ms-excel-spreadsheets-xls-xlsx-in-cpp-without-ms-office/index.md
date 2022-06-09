---
title: 'Create MS Excel Spreadsheets in C++ without MS Office - A Comprehensive Guide'
seoTitle: ""
description: ""
date: Fri, 15 May 2020 18:46:08 +0000
draft: false
url: /2020/05/15/create-ms-excel-spreadsheets-xls-xlsx-in-cpp-without-ms-office/
author: Usman Aziz
summary: ''
tags: ['Add tables in Excel using cpp', 'Calculate formulas in Excel in CPP', 'Create Excel XLSX files using Cpp', 'Create XLSX files using Cpp', 'Create charts in Excel using CPP']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Create-Excel-Files-in-C.jpg" alt="Create Excel Files in C++">}}


Previously, I have written a [post][1] on how to implement Excel automation features and create Excel XLS/XLSX files from scratch using C#. Today, I'll show you how to create Excel workbooks, insert data to Excel worksheets, calculate formulas, and create charts and tables in worksheets using C++. All the spreadsheet automation features will be powered by C++ Excel API - [Aspose.Cells for C++][2].

Aspose.Cells for C++ is a native C++ library that lets you create, read, parse, and convert spreadsheet documents without requiring Microsoft Excel. It provides a complete set of Excel automation features that can be utilized to generate and manipulate XLS/XLSX spreadsheets. In this article, we'll cover the following features of creating Excel XLS/XLSX files from scratch.

*   [Create Excel files (XLS/XLSX) using C++][3]
*   [Add data to an Excel worksheet using C++][4]
*   [Calculate workbook formulas using C++][5]
*   [Create tables in an Excel worksheet using C++][6]
*   [Create charts in Excel XLS/XLSX using C++][7]

## C++ Excel Spreadsheet API - Installation

You can download the complete package of library files of Aspose.Cells for C++ from the [Downloads][8] section. The package also contains a ready-to-run sample console application.

## Create Excel Files (XLS/XLSX) using C++ {#Create-Excel-XLS-or-XLSX-files-using-C++}

Lets first create a simple Excel XLSX workbook from scratch. A workbook is composed of one or multiple worksheets and each worksheet contains the data in the form of rows and columns. Therefore, in order to create an Excel spreadsheet, you need to create a workbook first and then add worksheets in it. The following are the steps to create an Excel file using Aspose.Cells for C++.

*   Create an object of the [IWorkbook][9] class.
*   Get the first worksheet (created by default) of the workbook into an [IWorksheet][10] object from [IWorksheetCollection][11].
*   Access the cells of the worksheet into an [ICells][12] object using the [IWorksheet->GetICells()][13] method.
*   Access the desired cell of the worksheet into an [ICell][14] object using the [ICells->GetObjectByIndex()][15] method by specifying the row and column index.
*   Add value to the cell using [ICell->PutValue()][16] method.
*   Save the workbook as .xlsx file using [IWorkbook->Save()][17] method.

The following code sample shows how to create an Excel XLSX file using C++.

{{< gist aspose-com-gists 5608dc642a88a2cc2b54339e908b6c6a "create-excel-workbook.cpp" >}}

### Excel Workbook

The following is the screenshot of the Excel workbook we have just created.



{{< figure align=center src="images/Create-Excel-XLSX-in-C.jpg" alt="Create Excel XLSX in C++">}}


## Add Data to an Excel Worksheet using C++ {#Add-data-to-an-Excel-worksheet-using-C++}

In the previous example, we have seen how to create a simple Excel file and insert value to a particular cell using row and column index. However, most often the cells in the Excel worksheets are identified using the column letter and row numbers such as A1, A2, B1, and etc. So let's look at the example of how to insert data into the worksheet using the cell names. The process only differs in adding value to cell and all other steps of creating the Excel workbook and worksheets are the same.

The following code sample shows how to create an Excel XLSX workbook and insert data into it using C++.

{{< gist aspose-com-gists 5608dc642a88a2cc2b54339e908b6c6a "add-data-to-excel-worksheet.cpp" >}}

## Calculate Workbook Formulas using C++ {#Calculate-workbook-formulas-using-C++}

Setting formulas in Excel workbooks is an amazing feature to perform calculations on data. It makes it quite easier to perform complex calculations on the data effectively and efficiently. The following are the steps to set and calculate formulas in Excel worksheets.

*   Create an object of the [IWorkbook][18] class.
*   Get the worksheet into an [IWorksheet][19] object from [IWorksheetCollection][20].
*   Use the [ICell][21] class to access the cell to which you want to apply the formula.
*   Set formula for the cell using the [ICell->SetFormula()][22] method.
*   Calculate the formula using [IWorkbook->CalculateFormula()][23] method.
*   Save the workbook using [IWorkbook->Save()][24] method.

The following code sample shows how to add and calculate formulas in an Excel XLSX workbook using C++.

{{< gist aspose-com-gists 5608dc642a88a2cc2b54339e908b6c6a "calculate-formula-in-excel.cpp" >}}

## Create Tables in an Excel Worksheet using C++ {#Create-tables-in-an-Excel-worksheet-using-C++}

The tables in Excel worksheets are used to organize a group of data located in a range of cells. Tables also help you maintain different types of lists in the worksheets. The following are the steps to create a table in the Excel worksheet.

*   Create a new Excel workbook using the [IWorkbook][25] class.
*   Access the default worksheet into the [IWorksheet][26] object or add a new one.
*   Insert value/data into the cells in the same way we have done in the previous example.
*   Add the range of cells to Lists collection of worksheet using [IWorksheet->GetIListObjects()->Add()][27] method.
*   Get the list into the [IListObject][28] object.
*   Apply styling to the table using [IListObject->SetTableStyleType()][29] method.
*   Save the workbook as .xlsx file.

The following code sample shows how to create a table in Excel XLSX file using C++.

{{< gist aspose-com-gists 5608dc642a88a2cc2b54339e908b6c6a "create-table-in-excel.cpp" >}}

### Excel Workbook with Table



{{< figure align=center src="images/Create-Excel-Table-in-C.jpg" alt="Create Table in Excel in C++">}}


## Create Charts in Excel Spreadsheet using C++ {#Add-charts-to-Excel-XLS/XLSX-using-C++}

Charts in Excel spreadsheets are used to visualize the data using different types of graphical objects. They give us a quick insight and understanding of the data particularly when data is huge. Aspose.Cells for C++ supports a variety of charts including Sunburst, Treemap, Histogram, Pyramid, Bubble, Line, and [many more][30]. The following are the steps to create a chart in Excel workbook using Aspose.Cells for C++.

*   Create a new Excel workbook.
*   Access the desired worksheet into the [IWorksheet][31] object.
*   Add a new chart to the worksheet using [IWorksheet->GetICharts()->Add()][32] method by passing chart's type.
*   Access the newly added chart into [IChart][33] object.
*   Set the data source for the chart using [IChart->GetNISeries()->Add()][34] method.
*   Save the workbook as .xlsx file.

The following code sample shows how to create a chart in Excel XLSX file using C++.

{{< gist aspose-com-gists 5608dc642a88a2cc2b54339e908b6c6a "create-chart-in-excel.cpp" >}}

### Excel Workbook with Chart



{{< figure align=center src="images/Create-Excel-Chart-in-C.jpg" alt="Create Chart in Excel in C++">}}


## Conclusion

In this article, we have covered how to create MS Excel spreadsheets from scratch using C++. The article also contains step by step guidelines and code samples on how to create tables, charts, and calculate formulas in Excel worksheets. You can learn more about other advanced features related to Excel automation from the [documentation][35] of Aspose.Cells for C++.

## Related Article

*   [Create PDF Files Programmatically using C++][36]




[1]: https://blog.aspose.com/2020/01/21/create-excel-xls-xlsx-programmatically-in-csharp-net/
[2]: https://products.aspose.com/cells/cpp
[3]: #Create-Excel-XLS-or-XLSX-files-using-C++
[4]: #Add-data-to-an-Excel-worksheet-using-C++
[5]: #Calculate-workbook-formulas-using-C++
[6]: #Create-tables-in-an-Excel-worksheet-using-C++
[7]: #Add-charts-to-Excel-XLS/XLSX-using-C++
[8]: https://downloads.aspose.com/cells/cpp/
[9]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[10]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet/
[11]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection/
[12]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_cells/
[13]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet/#a4ea63a44932c562552550c4f174e6bdd
[14]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_cell/
[15]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_cells/#a76bdc93952fac408c3bf2e84494c53f9
[16]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_cell/#a3bed4182c15428b97efdc15ed3c6f198
[17]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook/#a77072cfb929787df9ad1f38b02f58349
[18]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[19]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet/
[20]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection/
[21]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_cell/
[22]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_cell/#abe5297e74820c0509554030dacc25da3
[23]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook/#a990a5da177b7c3f1ed7b7c3592e6e038
[24]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook/#a77072cfb929787df9ad1f38b02f58349
[25]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[26]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet/
[27]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet/#a4356bc4b8cffee624891f10ea49a4705
[28]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.tables.i_list_object/
[29]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.tables.i_list_object/#a398d115b56c3be2dd3e094e18b069136
[30]: https://apireference.aspose.com/cells/cpp/namespace/aspose.cells.charts#a2f17e69bcefc754569019185d0621b70
[31]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet/
[32]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet/#a4dfecce61d7311ad41df2fdaf5592611
[33]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.charts.i_chart/
[34]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.charts.i_chart/#a3d2307281054e88ac12628162d010b5c
[35]: https://docs.aspose.com/display/cellscpp/Product+Overview
[36]: https://blog.aspose.com/2020/03/17/create-pdf-files-in-cpp-using-pdf-api/





