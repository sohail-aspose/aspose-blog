---
title: 'Merge or Unmerge Cells in an Excel Worksheet using C++'
seoTitle: "Merge or Unmerge Cells in an Excel Worksheet using C++"
description: "Merge and unmerge cells in an Excel worksheet using C++. Merge Cells, Ranges, and Named Ranges within your C++ applications."
date: Tue, 25 May 2021 16:44:41 +0000
draft: false
url: /2021/05/25/merge-or-unmerge-cells-in-an-excel-worksheet-using-cpp/
author: Muhammad Ahmad
summary: 'Merging and unmerging cells is a simple and commonly used feature of Microsoft Excel. Merging cells might prove to be helpful in scenarios, for example, when you have a worksheet with multiple columns that share the same heading. You can merge the cells above the columns to give them a common heading. In case merged cells are no longer required, you can unmerge them just as easily. You might need to perform these tasks within your C++ applications. For that, this article will teach you **how to merge and unmerge cells in Excel worksheets programmatically using C++**.'
tags: ['Merge Cells in an Excel Worksheet C++', 'Merge Named Range in an Excel Worksheet C++', 'Merge Range of Cells in an Excel Worksheet C++', 'Unmerge Cells in an Excel Worksheet C++', 'Unmerge Range of Cells in an Excel Worksheet C++']
categories: ['Aspose.Cells Product Family']
---

Merging and unmerging cells is a simple and commonly used feature of Microsoft Excel. Merging cells might prove to be helpful in scenarios, for example, when you have a worksheet with multiple columns that share the same heading. You can merge the cells above the columns to give them a common heading. In case merged cells are no longer required, you can unmerge them just as easily. You might need to perform these tasks within your C++ applications. For that, this article will teach you **how to merge and unmerge cells in Excel worksheets programmatically using C++**.

*   [C++ API for Merging and Unmerging Cells][1]
*   [Merge Cells in an Excel Worksheet using C++][2]
*   [Unmerge Cells in an Excel Worksheet using C++][3]
*   [Merge a Range of Cells in an Excel Worksheet using C++][4]
*   [Unmerge a Range of Cells in an Excel Worksheet using C++][5]
*   [Merge Cells of a Named Range in an Excel Worksheet using C++][6]

## C++ API for Merging and Unmerging Cells {#CPP-API-for-Merging-and-Unmerging-Cells}

[Aspose.Cells for C++][7] is a native C++ library that allows you to create, read and modify Excel files without requiring Microsoft Excel to be installed. The API also supports merging and unmerging cells in an Excel worksheet. You can either install the API through [NuGet][8] or download it directly from the [Downloads][9] section.

```
PM> Install-Package Aspose.Cells.Cpp
```

## Merge Cells in an Excel Worksheet using C++ {#Merge-Cells-in-an-Excel-Worksheet-using-CPP}

In this example, we will create an empty Excel worksheet and merge a few cells by following the steps given below.

*   Firstly, create an instance of the [IWorkbook][10] class.
*   Retrieve the worksheet using the [IWorkbook->GetIWorksheets()->GetObjectByIndex (Aspose::Cells::Systems::Int32 index)][11] method.
*   Retrieve the cells using the [IWorksheet->GetICells()][12] method.
*   Merge the cells using the [ICells->Merge(Aspose::Cells::Systems::Int32 firstRow, Aspose::Cells::Systems::Int32 firstColumn, Aspose::Cells::Systems::Int32 totalRows, Aspose::Cells::Systems::Int32 totalColumns)][13] method.
*   Apply styles to the merged cells.
*   Finally, save the output Excel file using the [IWorkbook->Save (intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][14] method.

The following sample code shows how to merge cells in an Excel worksheet using C++.

{{< gist aspose-com-gists 6572f976bb5e5fe78b7781210b9c4597 "Merge-Cells.cpp" >}}



{{< figure align=center src="images/MergeCellsExcelCpp.png" alt="Image of the output Excel file generated by the sample code" caption="Image of the output Excel file generated by the sample code">}}


## Unmerge Cells in an Excel Worksheet using C++ {#Unmerge-Cells-in-an-Excel-Worksheet-using-CPP}

The following are the steps to unmerge cells in an Excel worksheet.

*   Load the Excel file using the [IWorkbook][15] class.
*   Retrieve the worksheet containing merged cells using the [IWorkbook->GetIWorksheets()->GetObjectByIndex (Aspose::Cells::Systems::Int32 index)][16] method.
*   Retrieve the cells using the [IWorksheet->GetICells()][17] method.
*   Unmerge cells using the [ICells->UnMerge(Aspose::Cells::Systems::Int32 firstRow, Aspose::Cells::Systems::Int32 firstColumn, Aspose::Cells::Systems::Int32 totalRows, Aspose::Cells::Systems::Int32 totalColumns)][18] method.
*   Finally, save the output Excel file using the [IWorkbook->Save (intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][19] method.

The following sample code demonstrates how to unmerge cells in an Excel worksheet using C++.

{{< gist aspose-com-gists 6572f976bb5e5fe78b7781210b9c4597 "UnMerge-Cells.cpp" >}}



{{< figure align=center src="images/UnMergeCellsExcelCpp.png" alt="Image of the output Excel file generated by the sample code" caption="Image of the output Excel file generated by the sample code">}}


## Merge a Range of Cells in an Excel Worksheet using C++ {#Merge-a-Range-of-Cells-in-an-Excel-Worksheet-using-CPP}

The following are the steps to merge a range of cells in an Excel worksheet.

*   Firstly, create an instance of the [IWorkbook][20] class.
*   Retrieve the desired worksheet using the [IWorkbook->GetIWorksheets()->GetObjectByIndex (Aspose::Cells::Systems::Int32 index)][21] method.
*   Insert data into the cell.
*   Create the range using the [IWorksheet->GetICells()->CreateIRange(intrusive\_ptr<Aspose::Cells::Systems::String> address)][22] method.
*   Merge the range using the [IRange->Merge()][23] method.
*   Finally, save the output Excel file using the [IWorkbook->Save (intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][24] method.

The following sample code shows how to merge a range of cells in an Excel worksheet using C++.

{{< gist aspose-com-gists 6572f976bb5e5fe78b7781210b9c4597 "Merge-Range-Of-Cells.cpp" >}}



{{< figure align=center src="images/MergeRangeOfCellsExcelCpp.png" alt="Image of the output Excel file generated by the sample code" caption="Image of the output Excel file generated by the sample code">}}


## Unmerge a Range of Cells in an Excel Worksheet using C++ {#Unmerge-a-Range-of-Cells-in-an-Excel-Worksheet-using-CPP}

The following are the steps to unmerge a range of cells in an Excel worksheet.

*   Load the Excel file using the [IWorkbook][25] class.
*   Retrieve the worksheet containing merged cells using the [IWorkbook->GetIWorksheets()->GetObjectByIndex (Aspose::Cells::Systems::Int32 index)][26] method.
*   Create the range using the [IWorksheet->GetICells()->CreateIRange(intrusive\_ptr<Aspose::Cells::Systems::String> address)][27] method.
*   Unmerge the range using the [IRange->UnMerge()][28] method.
*   Finally, save the output Excel file using the [IWorkbook->Save (intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][29] method.

The following sample code shows how to unmerge a range of cells in an Excel worksheet using C++.

{{< gist aspose-com-gists 6572f976bb5e5fe78b7781210b9c4597 "UnMerge-Range-Of-Cells.cpp" >}}



{{< figure align=center src="images/UnMergeRangeOfCellsExcelCpp.png" alt="Image of the output Excel file generated by the sample code" caption="Image of the output Excel file generated by the sample code">}}


## Merge Cells of a Named Range in an Excel Worksheet using C++ {#Merge-Cells-of-a-Named-Range-in-an-Excel-Worksheet-using-CPP}

Aspose.Cells for C++ also provides you the ability to merge the cells of a named range. To achieve this, please follow the steps given below.

*   Load the Excel file using the [IWorkbook][30] class.
*   Retrieve the worksheet using the [IWorkbook->GetIWorksheets()->GetObjectByIndex (Aspose::Cells::Systems::Int32 index)][31] method.
*   Create the range using the [IWorksheet->GetICells()->CreateIRange(intrusive\_ptr<Aspose::Cells::Systems::String> address)][32] method.
*   Set the name of the range using the [IRange->SetName(intrusive\_ptr<Aspose::Cells::Systems::String> value)][33] method.
*   Create and apply styles to the named range.
*   Merge the cells of the named range using the [IRange->Merge()][34] method.
*   Finally, save the output Excel file using the [IWorkbook->Save (intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][35] method.

The following sample code demonstrates how to merge the cells of a named range using C++.

{{< gist aspose-com-gists 6572f976bb5e5fe78b7781210b9c4597 "Merge-Named-Range.cpp" >}}



{{< figure align=center src="images/MergeNamedRangeExcelCpp.png" alt="Image of the output Excel file generated by the sample code" caption="Image of the output Excel file generated by the sample code">}}


## Get a Free License

You can try the API without evaluation limitations by requesting [a free temporary license][36].

## Conclusion

In this article, you have learned how to merge and unmerge cells in an Excel worksheet using C++. Furthermore, you have seen how to merge and unmerge ranges and named ranges using Aspose.Cells for C++ API. The API provides many additional features for working with Excel files that you can explore in detail by visiting the [official documentation][37]. In case of any questions, please feel free to reach us on our [free support forum][38].

## See Also

*   [Convert Excel to CSV and CSV to Excel using C++][39]
*   [Find and Replace Text in Excel Spreadsheets using C++][40]




[1]: #CPP-API-for-Merging-and-Unmerging-Cells
[2]: #Merge-Cells-in-an-Excel-Worksheet-using-CPP
[3]: #Unmerge-Cells-in-an-Excel-Worksheet-using-CPP
[4]: #Merge-a-Range-of-Cells-in-an-Excel-Worksheet-using-CPP
[5]: #Unmerge-a-Range-of-Cells-in-an-Excel-Worksheet-using-CPP
[6]: #Merge-Cells-of-a-Named-Range-in-an-Excel-Worksheet-using-CPP
[7]: https://products.aspose.com/cells/cpp
[8]: https://www.nuget.org/packages/Aspose.Cells.Cpp
[9]: https://downloads.aspose.com/cells/cpp
[10]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[11]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection#a5574d624796043233420d0e0459ccc43
[12]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet#a4ea63a44932c562552550c4f174e6bdd
[13]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_cells#a429276dbdc0773835e7571afd8d763ce
[14]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[15]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[16]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection#a5574d624796043233420d0e0459ccc43
[17]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet#a4ea63a44932c562552550c4f174e6bdd
[18]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_cells#a90e17ec1c770f76223ae3dd911e0bfe3
[19]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[20]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[21]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection#a5574d624796043233420d0e0459ccc43
[22]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_cells#a8fb8288b6295fb9a3f856ede20c35537
[23]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_range#a0bf51fb9718e82fd8e854a9659de1e5f
[24]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[25]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[26]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection#a5574d624796043233420d0e0459ccc43
[27]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_cells#a8fb8288b6295fb9a3f856ede20c35537
[28]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_range#a1edc9ef6b22a4d14a0a8f3083937441d
[29]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[30]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[31]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection#a5574d624796043233420d0e0459ccc43
[32]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_cells#a8fb8288b6295fb9a3f856ede20c35537
[33]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_range#a78480b6b6db0f24cffc8acc2b06552eb
[34]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_range#a0bf51fb9718e82fd8e854a9659de1e5f
[35]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[36]: https://purchase.aspose.com/temporary-license
[37]: https://docs.aspose.com/cells/cpp/
[38]: https://forum.aspose.com/c/cells/9
[39]: https://blog.aspose.com/2021/03/25/convert-excel-to-csv-and-csv-to-excel-using-cpp/
[40]: https://blog.aspose.com/2021/02/11/find-and-replace-text-in-excel-spreadsheets-using-cpp/




