---
title: 'How to Read Excel Files in C#'
seoTitle: "How to Read Excel Files in C# .NET | .NET Excel Library"
description: "Use .NET Excel library to read Excel files in XLSX/XLS/CVS and other formats in C#. Read data from a single or all worksheets in an Excel file."
date: Sun, 10 Oct 2021 13:57:00 +0000
draft: false
url: /2021/10/10/how-to-read-excel-files-in-csharp/
author: Usman Aziz
summary: 'MS Excel files are largely used to keep tabular data in the form of worksheets. Often, the huge datasets are also maintained in Excel files. Therefore, you may come across the scenario where you need to read and fetch data from the worksheets in an Excel file. To achieve that, this article shows **how to read an Excel file in C#**. We will demonstrate how to read the whole Excel file or only a single worksheet programmatically.'
tags: ['read csv files in csharp dotnet', 'read data from excel file in csharp dotnet', 'read excel files in csharp dotnet', 'read xls files in csharp dotnet', 'read xlsx files in csharp dotnet']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Excel-File.jpg" alt="Read data in Excel files using C#">}}


MS Excel files are widely used to store data in the form of rows and columns. In various cases, the large datasets are also maintained in Excel files. Often, you have to read Excel files and fetch data from within your .NET applications. To achieve that within a few simple steps, this article shows **how to read an Excel file in C#**. Particularly, it covers how to read a whole Excel file or only a single worksheet from it.

*   [C# Library to Read Excel Files][1]
*   [Read Data from an Excel File][2]
*   [Read a Worksheet in an Excel File][3]

## C# Library to Read Excel Files {#Library-to-Read-Excel-Files}

To read data from the worksheets, we will use [Aspose.Cells for .NET][4]. It is a powerful and feature-rich API to create and manipulate Excel files. Moreover, it allows you to read Excel files quite easily. The API can be downloaded from the [downloads section][5] or installed via [NuGet][6].

```
PM> Install-Package Aspose.Cells
```

## Read an Excel File in C# {#Read-Data-from-an-Excel-File}

In Excel files, the data is stored inside **cells** where each cell is identified by its name (A1, B3, etc.) or the row and column index. The collection of cells makes a worksheet and an Excel file may contain single or multiple worksheets. Finally, all the worksheets collectively form a **workbook**. Aspose.Cells for .NET uses the same naming conventions to manipulate Excel files.

The following are the steps to read an Excel file and print its data using C#.

*   Load the Excel file using [Workbook][7] class.
*   Create an object of [WorksheetCollection][8] class and get reference of the worksheets using [Workbook.Worksheets][9].
*   Start a loop to go though all the worksheets in the collection and in each iteration, perform the following steps:
    *   Get reference of the worksheet in a [Worksheet][10] object.
    *   Get count of data rows and columns in the worksheet.
    *   Start a loop for rows.
    *   Start a nested loop for columns.
    *   Read data from each cell using [Worksheet.Cells\[i, j\].Value][11] property.

The following code sample shows how to read an Excel file in C#.

{{< gist aspose-com-gists d37524074e56c39cf484539a49f54c1f "read-excel-file.cs" >}}

The following is the output that we get in the console after running the code sample above.



{{< figure align=center src="images/Read-Excel-Files.jpg" alt="Reading data in the worksheets of Excel file in C#" caption="Reading an Excel File in C#">}}


## Read a Particular Worksheet in Excel in C# {#Read-a-Worksheet-in-an-Excel-Workbook}

You can also read only a particular worksheet in the Excel file by following the steps below.

*   Load the Excel file using [Workbook][12] class.
*   Get reference of desired worksheet in a [Worksheet][13] object using [Workbook.Worksheets\[index\]][14].
*   Get count of data rows and columns in the worksheet.
*   Start a loop for rows.
*   Start a nested loop for columns.
*   Read data from each cell using [Worksheet.Cells\[i, j\].Value][15] property.

The following code sample shows how to read data from a particular worksheet in C#.

{{< gist aspose-com-gists d37524074e56c39cf484539a49f54c1f "read-worksheet.cs" >}}

## Get a Free API License

You can use Aspose.Cells for .NET without evaluation limitations by getting a [free temporary license][16].

## Conclusion

In this article, you have learned how to read Excel files dynamically in C#. With the help of code samples, you have seen how to read data from a particular worksheet or all the worksheets in an Excel workbook. In addition, you can explore other features of Aspose.Cells for .NET using the [documentation][17]. In case you would have any queries, feel free to let us know via our [forum][18].

## See Also

*   [Create, Read, and Edit Excel Spreadsheets in ASP.NET MVC][19]
*   [Create Excel Files in C# without MS Office][20]




[1]: #Library-to-Read-Excel-Files
[2]: #Read-Data-from-an-Excel-File
[3]: #Read-a-Worksheet-in-an-Excel-Workbook
[4]: https://products.aspose.com/cells/net/
[5]: https://downloads.aspose.com/cells/net/
[6]: https://www.nuget.org/packages/Aspose.Cells
[7]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[8]: https://apireference.aspose.com/cells/net/aspose.cells/worksheetcollection
[9]: https://apireference.aspose.com/cells/net/aspose.cells/workbook/properties/worksheets
[10]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[11]: https://apireference.aspose.com/cells/net/aspose.cells/cell/properties/value
[12]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[13]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[14]: https://apireference.aspose.com/cells/net/aspose.cells/workbook/properties/worksheets
[15]: https://apireference.aspose.com/cells/net/aspose.cells/cell/properties/value
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/cells/net/
[18]: https://forum.aspose.com/
[19]: https://blog.aspose.com/2021/08/25/create-read-edit-excel-spreadsheet-in-asp-net-mvc/
[20]: https://blog.aspose.com/2020/01/21/create-excel-xls-xlsx-programmatically-in-csharp-net/




