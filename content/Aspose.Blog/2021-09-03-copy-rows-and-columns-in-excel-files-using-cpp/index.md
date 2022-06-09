---
title: 'Copy Rows and Columns in Excel Files using C++'
seoTitle: "Copy Rows and Columns in Excel Files using C++ | Aspose.Cells for C++"
description: "Copy single or multiple rows and columns in an Excel file using the simple and easy to use Aspose.Cells for C++ API within your C++ applications."
date: Fri, 03 Sep 2021 11:45:11 +0000
draft: false
url: /2021/09/03/copy-rows-and-columns-in-excel-files-using-cpp/
author: Muhammad Ahmad
summary: 'Copying rows and columns is a common task that is performed while working with Excel files. There might be situations where you need to copy rows or columns in Excel files programmatically. For such cases, this article will teach you **how to copy rows and columns in Excel files using C++**.'
tags: ['Copy a single column in an Excel file using C++', 'Copy a single row in an Excel file using C++', 'Copy multiple columns in an Excel file using C++', 'Copy multiple rows in an Excel file using C++']
categories: ['Aspose.Cells Product Family']
---

Copying rows and columns is a common task that is performed while working with Excel files. There might be situations where you need to copy rows or columns in Excel files programmatically. For such cases, this article will teach you **how to copy rows and columns in Excel files using C++**.

*   [C++ API for Copying Rows and Columns in Excel Files][1]
*   [Copy a Single Row in an Excel File using C++][2]
*   [Copying Multiple Rows in an Excel File using C++][3]
*   [Copy a Single Column in an Excel File using C++][4]
*   [Copying Multiple Columns in an Excel File using C++][5]

## C++ API for Copying Rows and Columns in Excel Files {#CPP-API-for-Copying-Rows-and-Columns-in-Excel-Files}

[Aspose.Cells for C++][6] is a native C++ library that allows you to create, read and modify Excel files without requiring Microsoft Excel to be installed. The API also provides the ability to copy rows and columns in Excel files. You can either install the API through [NuGet][7] or download it directly from the [Downloads][8] section.

```
PM> Install-Package Aspose.Cells.Cpp
```

## Copy a Single Row in an Excel File using C++ {#Copy-a-Single-Row-in-an-Excel-File-using-CPP}

The following is the image of the source Excel file that we will use in the following examples.



{{< figure align=center src="images/CopyRowsAndColumnsSource.jpg" alt="Source Worksheet">}}


The following are the steps to copy a single row in an Excel file using C++.

*   Load the Excel file using the [IWorkbook][9] class.
*   Retrieve the worksheet where you want to copy the row.
*   Copy the row using the [CopyIRow(intrusive\_ptr<Aspose::Cells::ICells> sourceCells, Aspose::Cells::Systems::Int32 sourceRowIndex, Aspose::Cells::Systems::Int32 destinationRowIndex)][10] method.
*   Save the Excel file using the [IWorkbook->Save(intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][11] method.

The following sample code shows how to copy a row in an Excel file using C++.

{{< gist aspose-com-gists 91953e5b36223b2b43268c46d5b32394 "Copy_Row.cpp" >}}



{{< figure align=center src="images/CopyRow.jpg" alt="Image showing the copied row" caption="Image showing the copied row">}}


## Copying Multiple Rows in an Excel File using C++ {#Copying-Multiple-Rows-in-an-Excel-File-using-CPP}

In order to copy multiple rows, we will use the [CopyIRows][12] method that accepts an additional parameter indicating the total number of rows to be copied. To copy multiple rows, follow the steps given below.

*   Load the Excel file using the [IWorkbook][13] class.
*   Retrieve the worksheet where you want to copy the rows.
*   Copy the rows using the [CopyIRows(intrusive\_ptr<Aspose::Cells::ICells> sourceCells, Aspose::Cells::Systems::Int32 sourceRowIndex, Aspose::Cells::Systems::Int32 destinationRowIndex, Aspose::Cells::Systems::Int32 rowNumber)][14] method.
*   Save the Excel file using the [IWorkbook->Save(intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][15] method.

The following sample code shows how to copy multiple rows in an Excel file using C++.

{{< gist aspose-com-gists 91953e5b36223b2b43268c46d5b32394 "Copy_Rows.cpp" >}}



{{< figure align=center src="images/CopyRows.jpg" alt="Image showing the copied rows" caption="Image showing the copied rows">}}


## Copy a Single Column in an Excel File using C++ {#Copy-a-Single-Column-in-an-Excel-File-using-CPP}

The following are the steps to copy a single column in an Excel file using C++.

*   Load the Excel file using the [IWorkbook][16] class.
*   Retrieve the worksheet where you want to copy the column.
*   Copy the column using the [CopyIColumn(intrusive\_ptr<Aspose::Cells::ICells> sourceCells, Aspose::Cells::Systems::Int32 sourceColumnIndex, Aspose::Cells::Systems::Int32 destinationColumnIndex)][17] method.
*   Save the Excel file using the [IWorkbook->Save(intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][18] method.

The following sample code shows how to copy a single column in an Excel file using C++.

{{< gist aspose-com-gists 91953e5b36223b2b43268c46d5b32394 "Copy_Column.cpp" >}}



{{< figure align=center src="images/CopyColumn.jpg" alt="Image showing the copied column" caption="Image showing the copied column">}}


## Copying Multiple Columns in an Excel File using C++ {#Copying-Multiple-Columns-in-an-Excel-File-using-CPP}

In order to copy multiple columns, we will use the [CopyIColumns][19] method that accepts an additional parameter indicating the total number of columns to be copied. To copy multiple columns, follow the steps given below.

*   Load the Excel file using the [IWorkbook][20] class.
*   Retrieve the worksheet where you want to copy the columns.
*   Copy the columns using the [CopyIColumns(intrusive\_ptr<Aspose::Cells::ICells> sourceCells, Aspose::Cells::Systems::Int32 sourceColumnIndex, Aspose::Cells::Systems::Int32 destinationColumnIndex, Aspose::Cells::Systems::Int32 columnNumber)][21] method.
*   Save the Excel file using the [IWorkbook->Save(intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][22] method.

The following sample code shows how to copy multiple columns in an Excel file using C++.

{{< gist aspose-com-gists 91953e5b36223b2b43268c46d5b32394 "Copy_Columns.cpp" >}}



{{< figure align=center src="images/CopyColumns.jpg" alt="Image showing the copied columns" caption="Image showing the copied columns">}}


## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][23].

## Conclusion

In this article, you have learned how to copy rows and columns in an Excel file using C++. The shared code samples show how to copy single and multiple rows and columns in an Excel file. We used the Aspose.Cells for C++ API to achieve this. It is a robust API that provides many additional features for working with Excel files. You can explore the API in detail by visiting the [official documentation][24]. In case of any queries, please feel free to reach us at our [free support forum][25].

## See Also

*   [Merge or Unmerge Cells in an Excel Worksheet using C++][26]
*   [Split Text into Columns in Excel Files using C++][27]




[1]: #CPP-API-for-Copying-Rows-and-Columns-in-Excel-Files
[2]: #Copy-a-Single-Row-in-an-Excel-File-using-CPP
[3]: #Copying-Multiple-Rows-in-an-Excel-File-using-CPP
[4]: #Copy-a-Single-Column-in-an-Excel-File-using-CPP
[5]: #Copying-Multiple-Columns-in-an-Excel-File-using-CPP
[6]: https://products.aspose.com/cells/cpp
[7]: https://www.nuget.org/packages/Aspose.Cells.Cpp
[8]: https://downloads.aspose.com/cells/cpp
[9]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[10]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_cells#a5c5075af8f98eb817ee9838afa62f0b7
[11]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[12]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_cells#a04fde6c9de007756eed12d837a7fbef0
[13]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[14]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_cells#a04fde6c9de007756eed12d837a7fbef0
[15]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[16]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[17]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_cells#a69fc560196eb5efdd8cf37d772b6a313
[18]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[19]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_cells#ab015f0fb4beb877d406238666c368ac9
[20]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[21]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_cells#ab015f0fb4beb877d406238666c368ac9
[22]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[23]: https://purchase.aspose.com/temporary-license
[24]: https://docs.aspose.com/cells/cpp/
[25]: https://forum.aspose.com/c/cells/9
[26]: https://blog.aspose.com/2021/05/25/merge-or-unmerge-cells-in-an-excel-worksheet-using-cpp/
[27]: https://blog.aspose.com/2021/05/24/split-text-into-columns-in-excel-files-using-cpp/




