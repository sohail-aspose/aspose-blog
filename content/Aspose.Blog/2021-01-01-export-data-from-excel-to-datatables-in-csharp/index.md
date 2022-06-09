---
title: 'Convert Excel Data to DataTables in C#'
seoTitle: "Convert Excel to DataTable in C# | Export XLSX XLS to DataTable C#"
description: "Convert data from Excel worksheets to DataTable using C#. Convert Excel XLSX or XLS to ADO.NET datatable from within .NET applications."
date: Fri, 01 Jan 2021 02:06:00 +0000
draft: false
url: /2021/01/01/export-data-from-excel-to-datatables-in-csharp/
author: Usman Aziz
summary: 'MS Excel spreadsheets are widely used to keep the small, medium, or large-sized data. In various cases, spreadsheets act as a database to store the application data. There could be situations when you need to read the data stored in the Excel files from within your web or desktop applications. For such cases, this article covers **how to export data from Excel worksheets to DataTables in C#**.'
tags: ['Csharp-API-to-Export-Excel-Data-to-DataTable', 'Excel-to-DataTable-in-Csharp']
categories: ['Aspose.Cells Product Family']
---

MS Excel spreadsheets are widely used to keep the small, medium, or large-sized data. In various cases, spreadsheets act as a database to store the application data. In such situations, you may need to read the data stored in the Excel files from within your web or desktop applications. For such cases, this article covers **how to convert Excel data to DataTables in C#**.

*   [C# API to Export Excel Data to DataTable][1]
*   [Excel to DataTable in C#][2]
*   [Convert Strongly-Typed Excel Data to DataTable][3]
*   [Convert Non-Strongly Typed Excel Data to DataTable][4]
*   [Get a Free License][5]

## C# Excel to DataTable Conversion API {#CSharp-API-for-Excel-to-DataTable}

[Aspose.Cells for .NET][6] is a class library that lets you implement Excel automation features within the .NET applications. In addition, the API allows you to export data from Excel worksheets to ADO.NET DataTable within a few steps. You can either [download][7] the API or install it via [NuGet][8].

```
PM> Install-Package Aspose.Cells
```

## Convert Excel to DataTable in C# {#Excel-to-DataTable-in-CSharp}

There could be two possible scenarios when exporting data from Excel worksheets to DataTables: the data could be strongly typed or non-strongly typed. In both cases, you can perform Excel to DataTable conversion accordingly. Let's have a look at how to deal with either of the above-mentioned scenarios.

### Convert Strongly-Typed Excel Data to DataTable in C# {#Export-Strongly-Typed-Excel-Data-to-DataTable}

Strongly typed data means the values in a single column belong to a particular data type. For such cases, you can export Excel data to DataTable in C# using the following steps.

*   Use [Workbook][9] class to load the Excel file.
*   Get the worksheet you want to export in a [Worksheet][10] object.
*   Use [Worksheet.Cells.ExportDataTable(int, int, int, int, bool)][11] method to export data to a [DataTable][12] object.
*   Use [DataTable][13] as the data source.

The following code sample shows how to export Excel to DataTable.

{{< gist aspose-com-gists 550f80c22e22768be6c5418bbdd0c89b "export-excel-to-datatable.cs" >}}

### Convert Non-Strongly Typed Excel Data to DataTable in C# {#Export-Non-Strongly-Typed-Excel-Data-to-DataTable}

Now, let's have a look at the other case when values in the worksheet are not strongly typed. It means they do not belong to a particular data type. The following are the steps to export Excel data to DataTable in this case.

*   Use [Workbook][14] class to load the Excel file.
*   Select the worksheet you want to export in a [Worksheet][15] object.
*   Use [Worksheet.Cells.ExportDataTableAsString(int, int, int, int, bool)][16] method to export data to a [DataTable][17] object.
*   Use [DataTable][18] as the data source.

The following code sample shows how to export non-strongly typed data from Excel to DataTable in C#.

{{< gist aspose-com-gists 550f80c22e22768be6c5418bbdd0c89b "export-excel-to-datatable-non-strongly.cs" >}}

## Get a Free License {#Get-a-Free-License}

You can [get a free temporary license][19] in order to try the API without evaluation limitations.

## Conclusion

In this article, you have learned how to export or convert Excel data to ADO.NET DataTables using C#. The step-by-step tutorial and code samples have shown how to deal with strongly typed and non-strongly typed data in the worksheets. You can explore more about the C# Excel API using [documentation][20].

## See Also

*   [Convert JSON to CSV and CSV to JSON using C#][21]




[1]: #CSharp-API-for-Excel-to-DataTable
[2]: #Excel-to-DataTable-in-CSharp
[3]: #Export-Strongly-Typed-Excel-Data-to-DataTable
[4]: #Export-Non-Strongly-Typed-Excel-Data-to-DataTable
[5]: #Get-a-Free-License
[6]: https://products.aspose.com/cells/net
[7]: https://downloads.aspose.com/cells/net
[8]: https://nuget.org/packages/Aspose.Cells
[9]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[10]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[11]: https://apireference.aspose.com/cells/net/aspose.cells.cells/exportdatatable/methods/2
[12]: https://docs.microsoft.com/en-us/dotnet/api/system.data.datatable
[13]: https://docs.microsoft.com/en-us/dotnet/api/system.data.datatable
[14]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[15]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[16]: https://apireference.aspose.com/cells/net/aspose.cells.cells/exportdatatableasstring/methods/1
[17]: https://docs.microsoft.com/en-us/dotnet/api/system.data.datatable
[18]: https://docs.microsoft.com/en-us/dotnet/api/system.data.datatable
[19]: https://purchase.aspose.com/temporary-license
[20]: https://docs.aspose.com/cells/net/developer-guide/
[21]: https://blog.aspose.com/2020/11/24/convert-csv-json-charp-vb-net/





