---
title: 'Copy Rows and Columns in Excel using C#'
seoTitle: "Copy Rows and Columns in Excel in C# .NET | Aspose.Cells for .NET"
description: "Use .NET Excel API to copy rows and columns in Excel worksheets using C#. Copy rows or columns within different Excel workbooks programmatically."
date: Thu, 15 Jul 2021 11:49:00 +0000
draft: false
url: /2021/07/15/copy-rows-and-columns-in-excel-using-csharp/
author: Usman Aziz
summary: 'In certain cases, you need to copy rows and columns in an Excel file without copying the entire worksheet. To perform this operation programmatically, this article covers **how to copy rows or columns in an Excel worksheet using C#**.'
tags: ['Copy Columns in Excel Worksheet using Csharp', 'Copy Rows in Excel Worksheet Csharp', 'Csharp API to Copy Rows and Columns in Excel']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Excel-File.jpg" alt="Copy Rows and Columns in Excel using C#">}}


In certain cases, you need to copy rows and columns in an Excel file without copying the entire worksheet. To perform this operation programmatically, this article covers **how to copy rows or columns in an Excel worksheet using C#**.

*   [C# API to Copy Rows and Columns in Excel][1]
*   [Copy Rows in Excel Worksheet using C#][2]
*   [Copy Columns in Excel Worksheet using C#][3]

## C# API to Copy Rows and Columns in Excel {#API-to-Copy-Rows-and-Columns-in-Excel}

[Aspose.Cells for .NET][4] is a class library that lets you implement Excel automation features within the .NET applications. The API provides simple ways to copy rows and columns within or between the Excel workbooks. You can either [download][5] the API or install it via [NuGet][6].

```
PM> Install-Package Aspose.Cells
```

## Copy Rows in Excel Worksheet using C# {#Copy-Rows-in-Excel-Worksheet}

The following are the steps to copy a row in an Excel worksheet using C#.

*   First, load the Excel file using [Workbook][7] class.
*   Get the desired [Worksheet][8] from [Workbook.Worksheets][9] collection.
*   Copy desired row by specifying the source and target row index in [Worksheet.Cells.CopyRow(Workheet.Cells, sourceRowIndex, targetRowIndex)][10] method.
*   Finally, save the updated Excel file using [Workbook.Save(string)][11] method.

The following code sample shows how to copy a row in Excel worksheet in C#.

{{< gist aspose-com-gists badef5dcc0845289eb79e3fed242c6cd "copy-rows.cs" >}}

## Copy Columns in Excel Worksheet using C# {#Copy-Columns-in-Excel-Worksheet}

The following are the steps to copy a column in an Excel worksheet using C#.

*   First, load the Excel file using [Workbook][12] class.
*   Get the desired [Worksheet][13] from [Workbook.Worksheets][14] collection.
*   Copy desired column by specifying the source and target column index in [Worksheet.Cells.CopyColumn(Workheet.Cells, sourceColumnIndex, targetColumnIndex)][15] method.
*   Finally, save the updated Excel file using [Workbook.Save(string)][16] method.

The following code sample shows how to copy a column in an Excel worksheet using C#.

{{< gist aspose-com-gists badef5dcc0845289eb79e3fed242c6cd "copy-columns.cs" >}}

## Get a Free License {#Get-a-Free-License}

You can use Aspose.Cells for .NET without evaluation limitations using a [temporary license][17].

## Conclusion

In this article, you have learned how to copy rows and columns in Excel worksheets using C#. You can use the provided code samples to copy rows or columns within different Excel workbooks as well. In addition, you can explore the [documentation][18] of Aspose.Cells for .NET. In case you would have any queries, feel free to post to our [forum][19].

## See Also

*   [Create MS Excel Files in C# without MS Office][20]
*   [Convert Excel to PDF in C#][21]




[1]: #API-to-Copy-Rows-and-Columns-in-Excel
[2]: #Copy-Rows-in-Excel-Worksheet
[3]: #Copy-Columns-in-Excel-Worksheet
[4]: https://products.aspose.com/cells/net
[5]: https://downloads.aspose.com/cells/net
[6]: https://nuget.org/packages/Aspose.Cells
[7]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[8]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[9]: https://apireference.aspose.com/cells/net/aspose.cells/workbook/properties/worksheets
[10]: https://apireference.aspose.com/cells/net/aspose.cells/cells/methods/copyrow
[11]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/2
[12]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[13]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[14]: https://apireference.aspose.com/cells/net/aspose.cells/workbook/properties/worksheets
[15]: https://apireference.aspose.com/cells/net/aspose.cells/cells/methods/copycolumn
[16]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/2
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/cells/net
[19]: https://forum.aspose.com/
[20]: https://blog.aspose.com/2020/01/21/create-excel-xls-xlsx-programmatically-in-csharp-net/
[21]: https://blog.aspose.com/2019/11/29/convert-xls-and-xlsx-to-pdf-in-csharp/





