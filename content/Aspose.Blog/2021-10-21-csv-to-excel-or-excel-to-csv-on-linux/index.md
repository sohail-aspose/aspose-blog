---
title: 'Linux: CSV to Excel or Excel to CSV using .NET'
seoTitle: "Linux: CSV to Excel, Excel to CSV | .NET Excel API for Linux"
description: "Convert CSV files to Excel or Excel files to CSV on Linux using .NET API. Convert CSV to XLSX/XLS or XLSX/XLS to CSV from within .NET 5 applications."
date: Thu, 21 Oct 2021 02:12:00 +0000
draft: false
url: /2021/10/21/csv-to-excel-or-excel-to-csv-on-linux/
author: Usman Aziz
summary: '[CSV][1] files are widely used to store the data in the form of comma-separated values. However, in certain cases, you need to export data from CSV files to Excel spreadsheets or vice versa. For such cases, this article covers **how to export data from CSV to Excel and Excel to CSV on Linux**.'
tags: ['Excel to csv on linux', 'csv to excel on linux', 'csv to xlsx on linux', 'xlsx to csv on linux']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/convert-csv-excel-xls-xlsx-csharp.png" alt="CSV to Excel or Excel to CSV">}}


[CSV][2] files are widely used to store the data in the form of comma-separated values. However, in certain cases, you need to export data from CSV files to Excel spreadsheets or vice versa. For such cases, this article covers **how to export data from CSV to Excel and Excel to CSV on Linux**.

*   [CSV to Excel or Excel to CSV Converter][3]
*   [Convert CSV to Excel][4]
*   [Convert Excel to CSV][5]

## CSV to Excel or Excel to CSV Converter for Linux {#CSV-to-Excel-or-Excel-to-CSV-Converter-for-Linux}

To export data from CSV to Excel or Excel to CSV, we will use [Aspose.Cells for .NET][6]. It is a powerful API for creating and manipulating Excel files from within the .NET applications. You can either [download][7] the API or install it via [NuGet][8].

If you are new to .NET development on Linux, read [how to create a console application on Linux][9] using [Visual Studio Code][10]. For the installation of Aspose.Cells for .NET in your application, you can use the [NuGet Package Manager extension][11] for Visual Studio Code.

## Convert CSV to Excel XLSX/XLS on Linux {#Convert-CSV-to-Excel-on-Linux}

The following are the steps to convert a CSV file to Excel XLSX/XLS on Linux.

1.  Create an instance of [LoadOptions][12] class and specify the input format.
2.  Create an instance of Workbook class and initialize it with CSV file's path and _LoadOptions_ object.
3.  Convert CSV to Excel using [Workbook.Save(string, SaveFormat.Xlsx)][13] method.

The following code sample shows how to convert a CSV file to Excel XLSX.

{{< gist aspose-com-gists e96bce4be59509ab59eb7a3bb530006d "csv-to-excel.cs" >}}

## Convert Excel to CSV on Linux {#Convert-Excel-to-CSV-on-Linux}

The following are the steps to convert an Excel XLSX/XLS file to CSV format.

1.  Create an instance of [Workbook][14] class and initialize it with Excel file's path.
2.  Convert Excel to CSV using [Workbook.Save(string, SaveFormat.Csv)][15] method.

The following code sample shows how to convert an Excel XLSX file to CSV.

{{< gist aspose-com-gists e96bce4be59509ab59eb7a3bb530006d "excel-to-csv.cs" >}}

## Get a Free License {#Get-a-Free-License}

You can use Aspose.Cells for .NET without evaluation limitations using a [temporary license][16].

## Conclusion

In this article, you have learned how to convert CSV files to Excel XLSX/XLS on Linux. Moreover, you have seen how to export data from Excel spreadsheets to CSV files. You can explore more about Aspose.Cells for .NET using the [documentation][17]. In case you would have any queries, you can ask us via our [forum][18].

## See Also

*   [Convert Excel Files to PDF on Linux using .NET][19]
*   [Import Data from JSON to Excel on Linux using .NET][20]




[1]: https://docs.fileformat.com/spreadsheet/csv/
[2]: https://docs.fileformat.com/spreadsheet/csv/
[3]: #CSV-to-Excel-or-Excel-to-CSV-Converter-for-Linux
[4]: #Convert-CSV-to-Excel-on-Linux
[5]: #Convert-Excel-to-CSV-on-Linux
[6]: https://products.aspose.com/cells/net
[7]: https://downloads.aspose.com/cells/net
[8]: https://www.nuget.org/packages/Aspose.Cells
[9]: https://docs.microsoft.com/en-us/dotnet/core/tutorials/with-visual-studio-code
[10]: https://code.visualstudio.com/
[11]: https://marketplace.visualstudio.com/items?itemName=jmrog.vscode-nuget-package-manager
[12]: https://apireference.aspose.com/cells/net/aspose.cells/loadoptions
[13]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/3
[14]: https://apireference.aspose.com/net/cells/aspose.cells/workbook
[15]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/3
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/cells/net/developer-guide/
[18]: https://forum.aspose.com/
[19]: https://blog.aspose.com/2021/10/12/convert-excel-files-to-pdf-on-linux/
[20]: https://blog.aspose.com/2021/09/16/import-data-from-json-to-excel-on-linux/




