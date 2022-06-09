---
title: 'Split Text into Columns in Excel Files using C++'
seoTitle: "Split Text into Columns in Excel Files using C++ | Text to Multiple Columns"
description: "Split text into columns in Excel files using C++. Split text in a single column to multiple columns using separators within your C++ applications."
date: Mon, 24 May 2021 18:40:00 +0000
draft: false
url: /2021/05/24/split-text-into-columns-in-excel-files-using-cpp/
author: Muhammad Ahmad
summary: 'Microsoft Excel allows splitting text into multiple columns using separators like blank space, comma, or other characters. This feature can be helpful in scenarios such as converting the comma-separated data exported from a database table to tabular form. To that end, this article will teach you **how to split text into columns in Excel files using C++**.'
tags: ['C++ Split Text To Columns in Excel', 'Split Text To Columns in Excel C++', 'Split Text to Multiple Columns C++']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Excel-File.png" alt="Split Text into Columns in Excel Files using C++">}}


Microsoft Excel allows splitting text into multiple columns using separators like blank space, comma, or other characters. This feature can be helpful in scenarios such as converting the comma-separated data exported from a database table to tabular form. To that end, this article will teach you **how to split text into columns in Excel files using C++**.

*   [C++ API for Splitting Text to Columns in Excel Files][1]
*   [Splitting Text into Columns in Excel Files using C++][2]

## C++ API for Splitting Text to Columns in Excel Files {#CPP-API-for-Splitting-Text-to-Columns-in-Excel-Files}

We will use the [Aspose.Cells for C++][3] API for splitting text into columns in Excel files. It is a native C++ library that allows you to create, read and modify Excel files without requiring Microsoft Excel to be installed. You can either install the API through [NuGet][4] or download it directly from the [Downloads][5] section.

```
PM> Install-Package Aspose.Cells.Cpp
```

## Split Text into Columns in Excel Files using C++ {#Split-Text-into-Columns-in-Excel-Files-using-CPP}

The following are the steps to split text into columns in Excel files.

*   Create an instance of the [IWorkbook][6] class.
*   Access the worksheet where you want to split the text using the [IWorkbook->GetIWorksheets()->GetObjectByIndex (Aspose::Cells::Systems::Int32 index)][7] method.
*   Insert sample data into the worksheet.
*   Create an instance of the [ITxtLoadOptions][8] class.
*   Specify the character that will be used to split the text using the [ITxtLoadOptions->SetSeparator(Aspose::Cells::Systems::Char value)][9] method.
*   Split the text into columns using the [IWorksheet->GetICells()->TextToColumns(Aspose::Cells::Systems::Int32 row, Aspose::Cells::Systems::Int32 column, Aspose::Cells::Systems::Int32 totalRows, intrusive\_ptr<Aspose::Cells::ITxtLoadOptions> options][10] method.
*   Save the Excel file using the [IWorkbook->Save (intrusive\_ptr<Aspose::Cells::Systems::String> fileName)][11] method.

The following sample code demonstrates how to split text into columns in Excel files using C++.

{{< gist aspose-com-gists 93312ed586022489c842096a4558422e "Text-To-Column.cpp" >}}



{{< figure align=center src="images/SplitTextIntoColumnsExcelCpp.png" alt="Image of the output Excel file showing the text split into two columns" caption="Image of the output Excel file showing the text split into two columns">}}


## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][12].

## Conclusion

In this article, you have learned how to split text into multiple columns in Excel files using C++. You have seen the complete code snippet along with the steps required to achieve this. Aspose.Cells for C++ is a robust API that provides many additional features for automating your Excel-related tasks. You can explore the API in detail by visiting the [official documentation][13]. In case of any questions, please feel free to reach us on our [free support forum][14].

## See Also

*   [Merge or Unmerge Cells in an Excel Worksheet using C++][15]
*   [Find and Replace Text in Excel Spreadsheets using C++][16]




[1]: #CPP-API-for-Splitting-Text-to-Columns-in-Excel-Files
[2]: #Split-Text-into-Columns-in-Excel-Files-using-CPP
[3]: https://products.aspose.com/cells/cpp
[4]: https://www.nuget.org/packages/Aspose.Cells.Cpp
[5]: https://downloads.aspose.com/cells/cpp
[6]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[7]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection#a5574d624796043233420d0e0459ccc43
[8]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_txt_load_options
[9]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_txt_load_options#a596fbb88ed665faa32afefa81c568d6f
[10]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_cells#a411abb46ccd3084faa58188661808eed)
[11]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349
[12]: https://purchase.aspose.com/temporary-license
[13]: https://docs.aspose.com/pdf/cpp/developer-guide/
[14]: https://forum.aspose.com/c/pdf/10
[15]: https://blog.aspose.com/2021/05/25/merge-or-unmerge-cells-in-an-excel-worksheet-using-cpp/
[16]: https://blog.aspose.com/2021/02/11/find-and-replace-text-in-excel-spreadsheets-using-cpp/





