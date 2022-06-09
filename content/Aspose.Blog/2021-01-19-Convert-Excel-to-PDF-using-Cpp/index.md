---
title: 'Convert Excel Files to PDF using C++'
seoTitle: "C++ Excel to PDF | Convert XLSX XLS to PDF in C++ | C++ Library"
description: "C++ Excel to PDF. Convert XLS to PDF and XLSX to PDF in C++. Set compliance level and creation date and time in Excel to PDF conversion using C++."
date: Tue, 19 Jan 2021 04:31:00 +0000
draft: false
url: /2021/01/19/Convert-Excel-to-PDF-using-Cpp/
author: Usman Aziz
summary: 'PDF format is widely used to exchange documents among the stakeholders. In various cases, the documents are converted to PDF format before they are shared. Thus, PDF is known to be a standard file format in such cases. In this article, we will target Excel to PDF conversion for C++ applications. Particularly, you will learn **how to convert Excel XLSX or XLS workbooks to PDF files using C++**.'
tags: ['Convert-Excel-Files-to-PDF-in-Cpp', 'Convert-Excel-to-PDF-with-Compliance-Level', 'Cpp-Excel-to-PDF-Converter-API']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Convert-Excel-to-PDF.jpg" alt="Excel to pdf C++">}}


PDF format is widely used to exchange documents among the stakeholders. In various cases, the documents are converted to PDF format before they are shared. Thus, PDF is known to be a standard file format in such cases. In this article, we will target Excel to PDF conversion programmatically. Particularly, you will learn **how to convert Excel XLSX or XLS workbooks to PDF files using C++**.

*   [C++ Excel to PDF Converter API][1]
*   [Convert Excel Files to PDF in C++][2]
*   [Convert Excel to PDF with Compliance Level][3]
*   [Set PDF Creation Date in Excel to PDF Conversion][4]
*   [Get Free License][5]

## C++ Excel to PDF Converter API {#C++-Excel-to-PDF-Converter-API}

[Aspose.Cells for C++][6] is designed to implement Excel automation features within C++ applications. Using the API, you can create new Excel files from scratch as well as manipulate the existing ones. The API's built-in spreadsheet converter lets you convert Excel files to other formats with high fidelity. You can either [download][7] the API package or install it from [NuGet][8].

```
Install-Package Aspose.Cells.Cpp
```

## Convert Excel Files to PDF in C++ {#Convert-Excel-Files-to-PDF-in-C++}

The following are the steps to convert Excel files to PDF using Aspose.Cells.

*   Load the Excel file using [intrusive\_ptr<Aspose::Cells::IWorkbook>][9] pointer.
*   Save the Excel file as a PDF using the [Save(StringPtr, SaveFormat\_Pdf)][10] method of [IWorkbook][11] class.

The following code sample shows how to convert Excel files to PDF using C++.

{{< gist aspose-com-gists 71ff4dee6a600bbec6ec5ac2e3800ea0 "excel-to-pdf.cpp" >}}

## C++ Excel to PDF with Compliance Level {#Convert-Excel-to-PDF-with-Compliance-Level}

Aspose.Cells for C++ also allows you to set the compliance level of the converted PDF file such as PDF/A. For this, the API provides an additional class named as [IPdfSaveOptions][12] that allows you to customize the Excel to PDF conversion with different options. The following are the steps to convert an Excel file to PDF with PDF/A compliance.

*   Load the Excel file using [intrusive\_ptr<Aspose::Cells::IWorkbook>][13] pointer.
*   Use [intrusive\_ptr<Aspose::Cells::IPdfSaveOptions>][14] pointer to create PDF save options.
*   Set compliance level using [IPdfSaveOptions->SetCompliance(Aspose::Cells::Rendering::PdfCompliance)][15] method.
*   Save the Excel file as PDF using [Save(StringPtr, IPdfSaveOptions)][16] method of [IWorkbook][17] class.

The following code sample shows how to set compliance level in Excel to PDF conversion.

{{< gist aspose-com-gists 71ff4dee6a600bbec6ec5ac2e3800ea0 "excel-to-pdf.cpp" >}}

## Set PDF Creation Date in Excel to PDF {#Set-PDF-Creation-Date-in-Excel-to-PDF-Conversion}

You can also set the creation date and time for the converted PDF file. For this, you can simply use [IPdfSaveOptions->SetCreatedTime(new Aspose::Cells::Systems::DateTime)][18] method. The following are the steps to perform this operation.

*   Load the Excel file using [intrusive\_ptr<Aspose::Cells::IWorkbook>][19] pointer.
*   Use [intrusive\_ptr<Aspose::Cells::IPdfSaveOptions>][20] pointer to create PDF save options.
*   Set date and time using [IPdfSaveOptions->SetCreatedTime(new Aspose::Cells::Systems::DateTime(2017, 5, 25))][21] method.
*   Save the Excel file as PDF using [Save(StringPtr, IPdfSaveOptions)][22] method of [IWorkbook][23] class.

The following code sample shows how to set the creation date and time in Excel to PDF conversion.

{{< gist aspose-com-gists 71ff4dee6a600bbec6ec5ac2e3800ea0 "excel-to-pdf.cpp" >}}

## Get a Free License {#Get-Free-License}

You can [get a free temporary license][24] in order to try the API without evaluation limitations.

## Conclusion

In this article, you have learned how to convert Excel files to PDF using C++. Furthermore, you have seen how to set the compliance level and the creation date for the converted PDF file. You can explore more about the API using [documentation][25].

## See Also

*   [Create MS Excel Spreadsheets in C++ without MS Office][26]




[1]: #C++-Excel-to-PDF-Converter-API
[2]: #Convert-Excel-Files-to-PDF-in-C++
[3]: #Convert-Excel-to-PDF-with-Compliance-Level
[4]: #Set-PDF-Creation-Date-in-Excel-to-PDF-Conversion
[5]: #Get-Free-License
[6]: https://products.aspose.com/cells/cpp
[7]: https://downloads.aspose.com/cells/cpp
[8]: http://nuget.org/packages/Aspose.Cells.cpp
[9]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[10]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a9460f52a2dec8f4bf623a4905167d997
[11]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[12]: https://apireference.aspose.com/cpp/cells/class/aspose.cells.i_pdf_save_options/
[13]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[14]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_pdf_save_options
[15]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_pdf_save_options#a2158ff23d7c071f8224b1cd063233c07
[16]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a5dc7de23f7ceba76a05dc1d49f51502e
[17]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[18]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_pdf_save_options#aa36725757f030716da7d827b16cb0cc4
[19]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[20]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_pdf_save_options
[21]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_pdf_save_options#aa36725757f030716da7d827b16cb0cc4
[22]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a5dc7de23f7ceba76a05dc1d49f51502e
[23]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[24]: https://purchase.aspose.com/temporary-license
[25]: https://docs.aspose.com/cells/cpp/getting-started/
[26]: https://blog.aspose.com/2020/05/15/create-ms-excel-spreadsheets-xls-xlsx-in-cpp-without-ms-office/





