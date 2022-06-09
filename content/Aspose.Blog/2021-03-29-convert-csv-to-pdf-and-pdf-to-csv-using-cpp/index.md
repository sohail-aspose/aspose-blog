---
title: 'Convert CSV to PDF and PDF to CSV using C++'
seoTitle: "Convert CSV to PDF and PDF to CSV using C++ | PDF Pages to CSV"
description: "Convert CSV to PDF format and PDF files to CSV format Programmatically using C++. Convert specific PDF pages to CSV files."
date: Mon, 29 Mar 2021 12:51:06 +0000
draft: false
url: /2021/03/29/convert-csv-to-pdf-and-pdf-to-csv-using-cpp/
author: Muhammad Ahmad
summary: '[PDF][1] files are a standard format for exchanging documents over the internet. There might be situations where you need to process the data in the PDF file and add that to a database. For such scenarios, converting the PDF document to [CSV][2] format might prove to be helpful. On the other hand, you might have some tabular data in CSV format that you want to share in a read-only manner with someone. You can achieve this by converting the CSV files to PDF format. In this article, you will learn how to interconvert [PDF][3] and [CSV][4] files programmatically using C++.'
tags: ['CSV to PDF C++', 'Convert CSV to PDF using C++', 'Convert PDF to CSV using C++', 'PDF pages to CSV C++', 'PDF to CSV C++']
categories: ['Aspose.PDF Product Family', 'Aspose.Cells Product Family']
---



{{< figure align=center src="images/PDFToCSVAndCSVToPDF-1024x404.jpg" alt="Convert PDF to CSV and CSV to PDF using C++">}}


[PDF][5] files are a standard format for exchanging documents over the internet. There might be situations where you need to process the data in the PDF file and add that to a database. For such scenarios, converting the PDF document to [CSV][6] format might prove to be helpful. On the other hand, you might have some tabular data in CSV format that you want to share in a read-only manner with someone. You can achieve this by converting the CSV files to PDF format. In this article, you will learn **how to interconvert PDF and CSV files programmatically using C++**.

*   [C++ API to Convert CSV to PDF and PDF to CSV Format][7]
*   [Convert CSV Files to PDF Format][8]
*   [Converting a PDF File to CSV Format][9]
*   [Convert Selected PDF Pages to a CSV File][10]
*   [Converting PDF Pages to Individual CSV Files][11]
*   [Get a Free License][12]

## C++ API to Convert CSV to PDF and PDF to CSV Format {#CPP-API-to-Convert-CSV-to-PDF-and-PDF-to-CSV-Format}

To achieve these conversions, you will need [Aspose.Cells for C++][13] and [Aspose.PDF for C++][14] APIs. The former is a C++ library for creating, reading, and modifying Excel files, whereas the latter is an API for working with PDF files. We will use Aspose.Cells for C++ API to convert CSV files to PDF format and Aspose.PDF for C++ API to convert PDF files to CSV format. You can either install the APIs through NuGet or download them directly from the [Downloads][15] section.

```
PM> Install-Package Aspose.Cells.Cpp
PM> Install-Package Aspose.PDF.Cpp
```

## Convert CSV Files to PDF Format {#Convert-CSV-Files-to-PDF-Format}

The following are the steps to convert CSV files to PDF format.

*   Create an instance of the [ILoadOptions][16] class.
*   Load the CSV file by creating an object of the [IWorkbook][17] class using the [ILoadOptions][18] instance created earlier.
*   Save the file in PDF format using the [IWorkbook->Save (intrusive\_ptr<Aspose::Cells::Systems::String> fileName, Aspose::Cells::SaveFormat saveFormat)][19] method.

The following is the sample code to convert CSV files to PDF format using C++.

{{< gist aspose-com-gists c6dbbba95ae31ff9c526b37ca170b929 "Convert-CSV-To-PDF.cpp" >}}

## Converting a PDF File to CSV Format {#Converting-a-PDF-File-to-CSV-Format}

The following are the steps to convert a PDF file to CSV format.

*   Load the PDF file using the [Document][20] class.
*   Create an instance of the [ExcelSaveOptions][21] class.
*   Set the format to CSV using [ExcelSaveOptions->set\_Format (ExcelSaveOptions::ExcelFormat value)][22] method.
*   Save the CSV file using the [Document->Save (System::String outputFileName, System::SharedPtr<SaveOptions> options)][23] method.

The following is the sample code to convert a PDF file to CSV format using C++.

{{< gist aspose-com-gists c6dbbba95ae31ff9c526b37ca170b929 "Convert-PDF-To-CSV.cpp" >}}

## Convert Selected PDF Pages to a CSV File {#Convert-Selected-PDF-Pages-to-a-CSV-File}

Aspose.PDF for C++ also provides you the ability to include specific PDF pages in the converted CSV file. To achieve this, you can follow the following steps.

*   Load the PDF file using the [Document][24] class.
*   Create an instance of the [ExcelSaveOptions][25] class.
*   Set the format to CSV using [ExcelSaveOptions->set\_Format (ExcelSaveOptions::ExcelFormat value)][26] method.
*   Create a new object of the [Document][27] class to represent the CSV file.
*   Loop through the pages of the PDF file using the [Document->get\_Pages()][28] method.
*   Within the loop, specify the condition for selecting the desired pages.
*   Add the pages to the newly created [Document][29] object using the [Document->get\_Pages()->Add (System::SharedPtr<Page> const & entity)][30] method.
*   Save the CSV file using the [Document->Save (System::String outputFileName, System::SharedPtr<SaveOptions> options)][31] method outside the loop.

The following is the sample code to include selected PDF pages in the CSV file.

{{< gist aspose-com-gists c6dbbba95ae31ff9c526b37ca170b929 "Convert-PDF-Pages-To-CSV.cpp" >}}

## Converting PDF Pages to Individual CSV Files {#Converting-PDF-Pages-to-Individual-CSV-Files}

With Aspose.PDF for C++, you can also convert PDF pages to individual CSV files. To achieve this, you can follow the following steps.

*   Load the PDF file using the [Document][32] class.
*   Create an instance of the [ExcelSaveOptions][33] class.
*   Set the format to CSV using [ExcelSaveOptions->set\_Format (ExcelSaveOptions::ExcelFormat value)][34] method.
*   Loop through the pages of the PDF file using the [Document->get\_Pages()][35] method.
*   Within the loop, create a new object of the [Document][36] class to represent the CSV file.
*   Add the pages to the newly created [Document][37] object using the [Document->get\_Pages()->Add (System::SharedPtr<Page> const & entity)][38] method.
*   Save the CSV file using the [Document->Save (System::String outputFileName, System::SharedPtr<SaveOptions> options)][39] method.

The following is the sample code to convert PDF pages to individual CSV files using C++.

{{< gist aspose-com-gists c6dbbba95ae31ff9c526b37ca170b929 "Convert-PDF-Pages-To-Separate-CSV-Files.cpp" >}}

## Get a Free License {#Get-a-Free-License}

You can try the API without evaluation limitations by requesting [a free temporary license][40].

## Conclusion

In this article, you have learned how to convert CSV files to PDF and PDF files to CSV format. Furthermore, you have seen how to add specific pages to the generated CSV file or convert PDF pages to individual CSV files. Aspose.Cells for C++ and Aspose.PDF for C++ are powerful APIs for working with Excel and PDF files, respectively. You can explore the APIs in detail by visiting their official documentation. In case of any questions, please feel free to reach us on our [free support forum][41].

*   [Aspose.Cells for C++ Documentation][42]
*   [Aspose.PDF for C++ Documentation][43]

## See Also

*   [Split a PDF File using C++][44]
*   [Convert Excel to CSV and CSV to Excel using C++][45]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/spreadsheet/csv/
[3]: https://docs.fileformat.com/pdf/
[4]: https://docs.fileformat.com/spreadsheet/csv/
[5]: https://docs.fileformat.com/pdf/
[6]: https://docs.fileformat.com/spreadsheet/csv/
[7]: #CPP-API-to-Convert-CSV-to-PDF-and-PDF-to-CSV-Format
[8]: #Convert-CSV-Files-to-PDF-Format
[9]: #Converting-a-PDF-File-to-CSV-Format
[10]: #Convert-Selected-PDF-Pages-to-a-CSV-File
[11]: #Converting-PDF-Pages-to-Individual-CSV-Files
[12]: #Get-a-Free-License
[13]: https://products.aspose.com/cells/cpp
[14]: https://products.aspose.com/pdf/cpp
[15]: https://downloads.aspose.com/total
[16]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_load_options
[17]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[18]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_load_options
[19]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a9460f52a2dec8f4bf623a4905167d997
[20]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[21]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.excel_save_options
[22]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.excel_save_options#a3822b816f92910c174a01fe799119d6e
[23]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a6383c010776212483f51cc41235924db
[24]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[25]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.excel_save_options
[26]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.excel_save_options#a3822b816f92910c174a01fe799119d6e
[27]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[28]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a481178a0c2c6277ae9b6b931d63e4122
[29]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[30]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.page_collection#a376029388847231999acb783d5e10d52
[31]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a6383c010776212483f51cc41235924db
[32]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[33]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.excel_save_options
[34]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.excel_save_options#a3822b816f92910c174a01fe799119d6e
[35]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a481178a0c2c6277ae9b6b931d63e4122
[36]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[37]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[38]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.page_collection#a376029388847231999acb783d5e10d52
[39]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a6383c010776212483f51cc41235924db
[40]: https://purchase.aspose.com/temporary-license
[41]: https://forum.aspose.com/
[42]: https://docs.aspose.com/cells/cpp/
[43]: https://docs.aspose.com/pdf/cpp/
[44]: https://blog.aspose.com/2021/03/19/split-a-pdf-file-using-cpp/
[45]: https://blog.aspose.com/2021/03/25/convert-excel-to-csv-and-csv-to-excel-using-cpp/





