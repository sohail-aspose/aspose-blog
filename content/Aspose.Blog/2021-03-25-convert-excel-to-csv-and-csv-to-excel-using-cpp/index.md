---
title: 'Convert Excel to CSV and CSV to Excel using C++'
seoTitle: "Convert Excel to CSV and CSV to Excel using C++"
description: "Convert Excel XLS/XLSX to CSV format and CSV files to Excel format Programmatically using C++. Convert specific Excel worksheets to CSV files."
date: Thu, 25 Mar 2021 15:10:01 +0000
draft: false
url: /2021/03/25/convert-excel-to-csv-and-csv-to-excel-using-cpp/
author: Muhammad Ahmad
summary: 'Excel is a popular format for sharing information. You may find yourself in situations where you have data in an Excel([XLS][1]/[XLSX][2] file that you need to import to a database. For this, you would need to convert the Excel file to [CSV][3] format. On the other hand, you may have data in CSV format exported from a database that you need to manipulate further in an Excel file. For such cases, you would need to convert the CSV file to Excel format. In this article, you will learn how to perform both these conversions programmatically using C++.'
tags: ['CSV to Excel C++', 'CSV to XLSX C++', 'Convert CSV To Excel using C++', 'Convert Excel to CSV using C++', 'Excel to CSV C++', 'XLSX to CSV C++']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/ExcelToCsvAndCsvToExcel-1024x404.jpg" alt="Convert Excel to CSV and CSV to Excel using C++">}}


Excel is a popular format for sharing information. You may find yourself in situations where you have data in an Excel([XLS][4]/[XLSX][5] file that you need to import to a database. For this, you would need to convert the Excel file to [CSV][6] format. On the other hand, you may have data in CSV format exported from a database that you need to manipulate further in an Excel file. For such cases, you would need to convert the CSV file to Excel format. In this article, you will learn how to perform both these conversions programmatically using C++.

*   [C++ API to Convert Excel Files to CSV and CSV files to Excel Format][7]
*   [Converting Excel files to CSV format using C++][8]
*   [Convert Excel Worksheets to CSV files][9]
*   [Converting CSV files to Excel format using C++][10]
*   [Get a Free License][11]

## C++ API to Convert Excel Files to CSV and CSV files to Excel Format {#CPP-API-to-Convert-Excel-Files-to-CSV-and-CSV-files-to-Excel-Format}

[Aspose.Cells for C++][12] is a native C++ library that allows you to create, read and modify Excel files. Furthermore, the API supports converting Excel files to CSV format and vice-versa. You can either install the API through [NuGet][13] or download it directly from the [Downloads][14] section.

```
PM> Install-Package Aspose.Cells.Cpp
```

## Converting Excel files to CSV format using C++ {#Converting-Excel-files-to-CSV-format-using-CPP}

Converting Excel files to CSV format is a breeze with Aspose.Cells for C++ API. The following are the steps to convert Excel files to CSV format using C++.

*   Load the Excel file using the [IWorkbook][15] class.
*   Save the file as CSV using the [IWorkbook->Save (intrusive\_ptr<Aspose::Cells::Systems::String> fileName, Aspose::Cells::SaveFormat saveFormat)][16] method.

The following is the sample code to convert Excel files to CSV format.

{{< gist aspose-com-gists f46aa511e63213a2f2b888ab9b51c44c "Convert-Excel-To-CSV.cpp" >}}

## Convert Excel Worksheets to CSV files {#Convert-Excel-Worksheets-to-CSV-files}

The previous example converts only the first worksheet if the Excel file contains multiple worksheets. In case you want to convert multiple worksheets to CSV format, you can follow the following steps.

*   Load the Excel file using the [IWorkbook][17] class.
*   Retrieve the worksheets using the [IWorkbook->GetIWorksheets()][18] method.
*   Loop through the retrieved worksheets.
*   Within the loop, you can specify your custom logic to convert specific worksheets to CSV files. In this demonstration, all the worksheets are converted to CSV files.
*   Retrieve the worksheet to be converted using [IWorkbook->GetIWorksheets()->GetObjectByIndex (Aspose::Cells::Systems::Int32 index)][19] method.
*   Create an instance of the [IWorkbook][20] class to represent a new CSV file.
*   Copy the previously retrieved worksheet to the new wokrbook instance using the [IWorkbook->GetIWorksheets()->GetObjectByIndex(0)->Copy (intrusive\_ptr<Aspose::Cells::IWorksheet> sourceSheet)][21] method.
*   Save the new workbook as CSV using the [IWorkbook->Save (intrusive\_ptr<Aspose::Cells::Systems::String> fileName, Aspose::Cells::SaveFormat saveFormat)][22] method.

The following is the sample code to convert Excel worksheets to CSV files using C++.

{{< gist aspose-com-gists f46aa511e63213a2f2b888ab9b51c44c "Convert-Excel-To-Multiple-CSV.cpp" >}}

## Converting CSV files to Excel format using C++ {#Converting-CSV-files-to-Excel-format-using-CPP}

The following are the steps to convert CSV files to Excel format using C++.

*   Create an instance of the [ILoadOptions][23] class.
*   Create an object of the [IWorkbook][24] class using the [ILoadOptions][25] instance created earlier.
*   Save the file in Excel format using the [IWorkbook->Save (intrusive\_ptr<Aspose::Cells::Systems::String> fileName, Aspose::Cells::SaveFormat saveFormat)][26] method.

The following is the sample code to convert CSV files to Excel format using C++.

{{< gist aspose-com-gists f46aa511e63213a2f2b888ab9b51c44c "Convert-CSV-To-Excel.cpp" >}}

## Get a Free License {#Get-a-Free-License}

You can try the API without evaluation limitations by requesting [a free temporary license][27].

## Conclusion

In this article, you have learned how to convert Excel files to CSV format and CSV files to Excel (XLS/XLSX) format using C++. Aspose.Cells for C++ is a vast API that provides many additional features for working with Excel files. You can explore the API in detail by using the [official documentation][28]. In case of any questions, please feel free to reach us on our [free support forum][29].

## See Also

*   [Convert Excel to HTML using C++][30]
*   [Convert Excel Files to Images using C++][31]




[1]: https://docs.fileformat.com/spreadsheet/xls/
[2]: https://docs.fileformat.com/spreadsheet/xlsx/)
[3]: https://docs.fileformat.com/spreadsheet/csv/
[4]: https://docs.fileformat.com/spreadsheet/xls/
[5]: https://docs.fileformat.com/spreadsheet/xlsx/)
[6]: https://docs.fileformat.com/spreadsheet/csv/
[7]: #CPP-API-to-Convert-Excel-Files-to-CSV-and-CSV-files-to-Excel-Format
[8]: #Converting-Excel-files-to-CSV-format-using-CPP
[9]: #Convert-Excel-Worksheets-to-CSV-files
[10]: #Converting-CSV-files-to-Excel-format-using-CPP
[11]: #Get-a-Free-License
[12]: https://products.aspose.com/cells/cpp
[13]: https://www.nuget.org/packages/Aspose.Cells.Cpp
[14]: https://downloads.aspose.com/cells/cpp
[15]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[16]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a9460f52a2dec8f4bf623a4905167d997
[17]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[18]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a72a58bea6003036e79282f54e0bfcffc
[19]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection#a5574d624796043233420d0e0459ccc43
[20]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[21]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet#ae95f6a0ec074f5583d6ff5b487facbab
[22]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a9460f52a2dec8f4bf623a4905167d997
[23]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_load_options
[24]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[25]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_load_options
[26]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a9460f52a2dec8f4bf623a4905167d997
[27]: https://purchase.aspose.com/temporary-license
[28]: https://docs.aspose.com/cells/cpp/
[29]: https://forum.aspose.com/c/cells/9
[30]: https://blog.aspose.com/2021/02/06/convert-excel-to-html-using-cpp/
[31]: https://blog.aspose.com/2021/01/28/convert-excel-files-to-images-using-cpp/





