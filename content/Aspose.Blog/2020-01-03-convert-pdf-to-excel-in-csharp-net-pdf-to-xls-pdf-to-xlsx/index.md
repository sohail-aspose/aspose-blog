---
title: 'How to Convert PDF to Excel in C# .NET - PDF to XLS or XLSX'
seoTitle: "Convert PDF to Excel in C# | PDF to XLS | PDF to XLSX | .NET API"
description: "Convert PDF to Excel in C#. Convert PDF to XLS, PDF to XLSX. Export tabular data from PDF to Excel in C#. PDF to Excel Converter class library for .NET."
date: Fri, 03 Jan 2020 18:00:44 +0000
draft: false
url: /2020/01/03/convert-pdf-to-excel-in-csharp-net-pdf-to-xls-pdf-to-xlsx/
author: Usman Aziz
summary: ''
tags: ['Aspose.Pdf for .NET', 'convert pdf to excel', 'export table from pdf to excel', 'extract table from pdf to excel', 'pdf to excel', 'pdf to excel in .net', 'pdf to excel in csharp', 'pdf to xls', 'pdf to xlsx']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/PDF-to-Excel-Conversion.png" alt="PDF to Excel in C# .NET">}}


**PDF to Excel** conversion is an important use case when you need to export the tabular data from PDF documents to Excel spreadsheets. Copying/exporting the data from PDF to Excel manually could be a time-consuming task when you are dealing with a bunch of documents. So why not automate this process and minimize the time and effort? In this article, you will learn how to **convert PDF to Excel** programmatically using **C# .NET**.

## Converting PDF to Excel in C# .NET

This article covers the following PDF to Excel conversions using C#.

*   Converting PDF to XLS format.
*   Converting PDF to XLSX format.
*   Inserting a blank first column in converted Excel worksheet.
*   Minimizing the number of worksheets in the converted Excel spreadsheet.

For PDF to Excel conversion in C#, we'll use [Aspose.PDF for .NET][1] API that supports creating and manipulating PDF documents as well as converting PDF files to other formats. You can either [download][2] DLL of the API or install it using one of the following ways.

### Install via NuGet Package Manager

*   Open/create the project in Visual Studio.
*   Go to NuGet Package Manager and search Aspose.PDF.
*   Install the API.



{{< figure align=center src="images/Aspose.PDF-NPM.png" alt="">}}


### Install via Package Manager Console```
PM> Install-Package Aspose.PDF
```

## Converting PDF to XLS in C#

In order to convert a PDF document to the XLS spreadsheet, you can simply load the PDF file and save it with the ".xls" extension. The following code sample shows how to convert PDF to Excel in XLS format using C#.

{{< gist aspose-com-gists 063356f993b8fdd63f1c81267e6eb9dc "convert-pdf-to-excel-xls-csharp.cs" >}}

### PDF Document



{{< figure align=center src="images/Convert-pdf-to-excel-C.png" alt="">}}


### Converted Excel Spreadsheet



{{< figure align=center src="images/Convert-pdf-to-excel-C-2.png" alt="">}}


## Converting PDF to XLSX in C#

By default, Aspose.PDF converts the PDF document to XLS format. In case you want to get the converted Excel spreadsheet in XLSX format, you can specify it using [ExcelSaveOptions][3] class. The following code sample shows how to convert a PDF document to Excel with XLSX format using C#.

{{< gist aspose-com-gists 063356f993b8fdd63f1c81267e6eb9dc "convert-pdf-to-excel-xlsx-csharp.cs" >}}

## Convert PDF to Excel with a Blank First Column

You can also insert a blank first column in the converted Excel spreadsheet. This can be done using [ExcelSaveOptions.InsertBlankColumnAtFirst][4] option as shown in the following code sample.

{{< gist aspose-com-gists 063356f993b8fdd63f1c81267e6eb9dc "convert-pdf-to-excel-blank-column.cs" >}}

## Convert PDF to Excel with Minimized Number of Worksheets

By default, every page in the input PDF document is converted into a separate worksheet. For the large PDF documents with a number of pages, the converted Excel spreadsheet will also contain a number of worksheets. In such a case, you can customize the PDF to Excel conversion and minimize the number of worksheets in the converted spreadsheet using [ExcelSaveOptions.MinimizeTheNumberOfWorksheets][5] option.

The following code sample shows how to minimize the number of worksheets in PDF to Excel conversion using C#.

{{< gist aspose-com-gists 063356f993b8fdd63f1c81267e6eb9dc "convert-pdf-to-excel-minimized-worksheets.cs" >}}

Read more about Aspose.PDF for .NET [here][6].

Related Article(s)

*   [Convert PDF Documents to Excel XLS/XLSX using Java][7]
*   [Converting Word Documents to PDF Programmatically in C# .NET][8]




[1]: https://products.aspose.com/pdf/net
[2]: https://downloads.aspose.com/pdf/net
[3]: https://apireference.aspose.com/net/pdf/aspose.pdf/excelsaveoptions
[4]: https://apireference.aspose.com/net/pdf/aspose.pdf/excelsaveoptions/properties/insertblankcolumnatfirst
[5]: https://apireference.aspose.com/net/pdf/aspose.pdf/excelsaveoptions/properties/minimizethenumberofworksheets
[6]: https://docs.aspose.com/display/pdfnet/Product+Overview
[7]: https://blog.aspose.com/2020/06/24/convert-pdf-to-excel-xls-xlsx-using-java/
[8]: https://blog.aspose.com/2020/01/02/convert-word-doc-docx-to-pdf-in-csharp-net-core/





