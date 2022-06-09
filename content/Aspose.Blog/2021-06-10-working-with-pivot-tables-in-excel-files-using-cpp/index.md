---
title: 'Working With Pivot Tables in Excel Files using C++'
seoTitle: "Working With Pivot Tables in Excel Files using C++"
description: "Working with Pivot Tables in Excel files using C++. Create Pivot Tables and sort, hide and update the data in pivot tables within your C++ applications."
date: Thu, 10 Jun 2021 17:05:21 +0000
draft: false
url: /2021/06/10/working-with-pivot-tables-in-excel-files-using-cpp/
author: Muhammad Ahmad
summary: 'Pivot tables rearrange data to represent it in a meaningful way. They provide different sorting options and provide sums, averages, or other statistics by grouping data together. It is an essential tool for data analysis and is a fundamental part of MS Excel. You might find yourself in scenarios where you need to create and manipulate pivot tables programmatically. To that end, this article will teach you **how to work with pivot tables in Excel files using C++**.'
tags: ['Create Pivot Table Excel C++', 'Hide Rows in Pivot Table Excel C++', 'Manipulate Pivot Table Data Excel C++', 'Sort Pivot Table Excel C++']
categories: ['Aspose.Cells Product Family']
---

Pivot tables rearrange data to represent it in a meaningful way. They provide different sorting options and provide sums, averages, or other statistics by grouping data together. It is an essential tool for data analysis and is a fundamental part of MS Excel. You might find yourself in scenarios where you need to create and manipulate pivot tables programmatically. To that end, this article will teach you **how to work with pivot tables in Excel files using C++**.

*   [C++ API for Working with Pivot Tables in Excel Files][1]
*   [Create a Pivot Table in an Excel File using C++][2]
*   [Sort Pivot Table in an Excel File using C++][3]
*   [Hide Rows in a Pivot Table using C++][4]
*   [Manipulate Pivot Table Data using C++][5]

## C++ API for Working with Pivot Tables in Excel Files {#CPP-API-for-Working-with-Pivot-Tables-in-Excel-Files}

[Aspose.Cells for C++][6] is a native C++ library that allows you to create, read and update Excel files without requiring Microsoft Excel to be installed. The API also supports working with pivot tables in Excel files. You can either install the API through [NuGet][7] or download it directly from the [Downloads][8] section.

```
PM> Install-Package Aspose.Cells.Cpp
```

## Create a Pivot Table in an Excel File using C++ {#Create-a-Pivot-Table-in-an-Excel-File-using-CPP}

In the following example, we will create a new Excel file, insert sample data into it and create a pivot table. The file generated in this example will be used as the source file for other examples. The following are the steps to create a pivot table in an Excel file.

*   Firstly, create an instance of the [IWorkbook][9] class to represent the new Excel file.
*   Access the worksheet where you want to insert the pivot table using [IWorkbook->GetIWorksheets()->GetObjectByIndex (Aspose::Cells::Systems::Int32 index)][10] method.
*   Add sample data for the pivot table.
*   Add pivot table using the [IWorksheet->GetIPivotTables()->Add(intrusive\_ptr<Aspose::Cells::Systems::String> sourceData, intrusive\_ptr<Aspose::Cells::Systems::String> destCellName, intrusive\_ptr<Aspose::Cells::Systems::String> tableName)][11] method.
*   To access the pivot table, use the [IWorksheet->GetIPivotTables()->GetObjectByIndex(Aspose::Cells::Systems::Int32 index)][12] method.
*   Manipulate the fields and set the style of the pivot table.
*   Finally, save the Excel file using the [IWorkbook->Save (intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][13] method.

The following sample code shows how to create a pivot table in an Excel file using C++.

{{< gist aspose-com-gists b0049afd158525919d84b34f8072d2b2 "Create-Pivot-Table.cpp" >}}



{{< figure align=center src="images/CreatePivotTableExcelCpp.png" alt="Image of the Pivot Table created by the sample code" caption="Image of the Pivot Table created by the sample code">}}


## Sort Pivot Table in an Excel File using C++ {#Sort-Pivot-Table-in-an-Excel-File-using-CPP}

In the following example, we will sort the first column of the pivot table in descending order. The following are the steps to sort data in a pivot table.

*   Firstly, load the sample Excel file using the [IWorkbook][14] class.
*   Retrieve the worksheet containing the pivot table using [IWorkbook->GetIWorksheets()->GetObjectByIndex (Aspose::Cells::Systems::Int32 index)][15] method.
*   Access the pivot table using [IWorksheet->GetIPivotTables()->GetObjectByIndex(Aspose::Cells::Systems::Int32 index)][16] method.
*   Get row field and sort the pivot table using the [IPivotField->SetAutoSort(bool value)][17] and [IPivotField->SetAscendSort(bool value)][18] methods.
*   Refresh the contents of the pivot table and calculate the data using the [IPivotTable->RefreshData()][19] and [IPivotTable->CalculateData()][20] methods respectively.
*   Finally, save the Excel file using the [IWorkbook->Save (intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][21] method.

The following sample code demonstrates how to sort a pivot table in an Excel file using C++.

{{< gist aspose-com-gists b0049afd158525919d84b34f8072d2b2 "Sort-Pivot-Table.cpp" >}}



{{< figure align=center src="images/SortedPivotTableExcelCpp.png" alt="Image of the sorted Pivot Table generated by the sample code" caption="Image of the sorted Pivot Table generated by the sample code">}}


## Hide Rows in a Pivot Table using C++ {#Hide-Rows-in-a-Pivot-Table-using-CPP}

With Aspose.Cells for C++ API, you can also hide the rows in a pivot table. In the following example, we will hide the row with the "Orange" row label. The following are the steps to hide rows in a pivot table.

*   Firstly, load the sample Excel file using the [IWorkbook][22] class.
*   Retrieve the worksheet containing the pivot table using [IWorkbook->GetIWorksheets()->GetObjectByIndex (Aspose::Cells::Systems::Int32 index)][23] method.
*   Access the pivot table using [IWorksheet->GetIPivotTables()->GetObjectByIndex(Aspose::Cells::Systems::Int32 index)][24] method.
*   Get the pivot table data body range using [IPivotTable->GetIDataBodyRange()][25] method.
*   Iterate through the rows of the pivot table and hide the rows meeting your criteria.
*   Refresh the contents of the pivot table and calculate the data using the [IPivotTable->RefreshData()][26] and [IPivotTable->CalculateData()][27] methods respectively.
*   Finally, save the Excel file using the [IWorkbook->Save (intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][28] method.

The following sample code shows how to hide rows in a pivot table using C++.

{{< gist aspose-com-gists b0049afd158525919d84b34f8072d2b2 "Hide-Rows-In-Pivot-Table.cpp" >}}



{{< figure align=center src="images/PivotTableWithHiddenRowExcelCpp.png" alt="Image of the pivot table with a hidden row" caption="Image of the pivot table with a hidden row">}}


## Manipulate Pivot Table Data using C++ {#Manipulate-Pivot-Table-Data-using-CPP}

You can also manipulate the data of an existing pivot table using Aspose.Cells for C++ API. In the following example, we will replace the text "Apple" in cell "A2" with "Orange" and reflect the change in the pivot table. The following are the steps to manipulate pivot table data.

*   Firstly, load the sample Excel file using the [IWorkbook][29] class.
*   Retrieve the worksheet containing the pivot table data using the [IWorkbook->GetIWorksheets()->GetObjectByIndex (Aspose::Cells::Systems::Int32 index)][30] method.
*   Update the data of the pivot table according to your requirements.
*   In order to access the pivot table, use [IWorksheet->GetIPivotTables()->GetObjectByIndex(Aspose::Cells::Systems::Int32 index)][31] method.
*   Refresh the contents of the pivot table and calculate the data using the [IPivotTable->RefreshData()][32] and [IPivotTable->CalculateData()][33] methods respectively.
*   Finally, save the Excel file using the [IWorkbook->Save (intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][34] method.

The following sample code shows how to update the data of a pivot table using C++.

{{< gist aspose-com-gists b0049afd158525919d84b34f8072d2b2 "Manipulate-Pivot-Table-Data.cpp" >}}



{{< figure align=center src="images/UpdatePivotTableDataExcelCpp.png" alt="Pivot Table showing the updated data" caption="Pivot Table showing the updated data">}}


## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][35].

## Conclusion

In this article, you have learned how to work with pivot tables in Excel files using C++. Specifically, you have learned how to create a pivot table and sort, hide and update the data in a pivot table using C++. Aspose.Cells for C++ is a vast API that provides a bunch of additional features for working with Excel files. You can explore the API in detail by visiting the [official documentation][36]. In case of any questions, please feel free to reach us on our [free support forum][37].

## See Also

*   [Copy or Move Excel Worksheets using C++][38]
*   [Inserting and Deleting Rows and Columns in Excel using C++][39]




[1]: #CPP-API-for-Working-with-Pivot-Tables-in-Excel-Files
[2]: #Create-a-Pivot-Table-in-an-Excel-File-using-CPP
[3]: #Sort-Pivot-Table-in-an-Excel-File-using-CPP
[4]: #Hide-Rows-in-a-Pivot-Table-using-CPP
[5]: #Manipulate-Pivot-Table-Data-using-CPP
[6]: https://products.aspose.com/cells/cpp
[7]: https://www.nuget.org/packages/Aspose.Cells.Cpp
[8]: https://downloads.aspose.com/cells/cpp
[9]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[10]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection#a5574d624796043233420d0e0459ccc43
[11]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.pivot.i_pivot_table_collection#a903a0eb3d7ef995c370f4a4385b25111
[12]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.pivot.i_pivot_table_collection#aa50afc0d0925c4011f7f284ca17ed4c7
[13]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[14]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[15]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection#a5574d624796043233420d0e0459ccc43
[16]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.pivot.i_pivot_table_collection#aa50afc0d0925c4011f7f284ca17ed4c7
[17]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.pivot.i_pivot_field#ae2a99ce5eaab4f3353b5b4322a3a7d79
[18]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.pivot.i_pivot_field#a4d7733619c15bf6b80f1abdf290a6b77
[19]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.pivot.i_pivot_table#ab6d71ded346508a1d4a93c59680ddaf6
[20]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.pivot.i_pivot_table#a3d6ffec8ce2a7a4ccb58e0452a1733dd
[21]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[22]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[23]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection#a5574d624796043233420d0e0459ccc43
[24]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.pivot.i_pivot_table_collection#aa50afc0d0925c4011f7f284ca17ed4c7
[25]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.pivot.i_pivot_table#ab089cf964d033a5854b7b0f734d83d65
[26]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.pivot.i_pivot_table#ab6d71ded346508a1d4a93c59680ddaf6
[27]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.pivot.i_pivot_table#a3d6ffec8ce2a7a4ccb58e0452a1733dd
[28]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[29]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[30]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection#a5574d624796043233420d0e0459ccc43
[31]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.pivot.i_pivot_table_collection#aa50afc0d0925c4011f7f284ca17ed4c7
[32]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.pivot.i_pivot_table#ab6d71ded346508a1d4a93c59680ddaf6
[33]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.pivot.i_pivot_table#a3d6ffec8ce2a7a4ccb58e0452a1733dd
[34]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[35]: https://purchase.aspose.com/temporary-license
[36]: https://docs.aspose.com/cells/cpp/
[37]: https://forum.aspose.com/c/cells/9
[38]: https://blog.aspose.com/2021/04/06/copy-or-move-excel-worksheets-using-cpp/
[39]: https://blog.aspose.com/2021/04/23/inserting-and-deleting-rows-and-columns-in-excel-using-cpp/





