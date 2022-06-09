---
title: 'Convert Excel XLSX and XLS to SVG using C#'
seoTitle: "Convert Excel XLSX XLS to SVG in C# | XLSX to SVG | XLS to SVG"
description: "Use .NET Excel API to convert the Excel XLSX or XLS files to SVG using C# or VB.NET. Perform Excel to SVG conversion from within your .NET applications."
date: Fri, 15 Oct 2021 17:06:35 +0000
draft: false
url: /2021/10/15/convert-excel-to-svg-using-csharp/
author: Usman Aziz
summary: 'Excel files are widely used to keep and organize small as well as large sized data. Moreover, you can perform various operations on the data stored in Excel worksheets. In certain cases, you may need to convert the Excel workbooks to other formats to embed their content within the web applications. For such cases, this article covers **how to convert Excel [XLSX][1]/[XLS][2] files to [SVG][3] format using C#**.'
tags: ['Excel to SVG Converter CSharp', 'xls to svg csharp', 'xlsx to svg csharp']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Excel-to-SVG.jpg" alt="Excel to SVG C#">}}


Excel files are widely used to keep and organize small as well as large sized data. Moreover, you can perform various operations on the data stored in Excel worksheets. In certain cases, you may need to convert the Excel worksheets to other formats, for example to embed their content within the web applications. For such cases, this article covers **how to convert Excel [XLSX][4] or [XLS][5] files to [SVG][6] format using C#**.

*   [C# Excel to SVG Converter][7]
*   [Convert Excel XLSX or XLS to SVG][8]

## C# Excel to SVG Converter {#Excel-to-SVG-Converter}

In order to convert Excel XLSX or XLS files to SVG, we will use [Aspose.Cells for .NET][9]. It is a powerful API for creating, modifying, and converting spreadsheet files from within .NET applications. You can either [download][10] the API or install it using [NuGet][11].

```
PM> Install-Package Aspose.Cells
```

## Convert Excel XLSX or XLS to SVG {#Convert-Excel-XLSX-or-XLS-to-SVG}

The following are the steps to convert an Excel XLSX or XLS file to SVG using C#.

1.  Load Excel file using [Workbook][12] class.
2.  Select the desired worksheet or loop through all the worksheets in [Workbook.Worksheets][13] collection.
3.  Create an object of [ImageOrPrintOptions][14] class and set rendering options.
4.  Create an object of [SheetRenderer][15] class for the worksheet.
5.  Convert Excel to SVG using [SheetRenderer.ToImage(int32, string)][16] method.

The following code sample shows how to convert an Excel XLSX file to SVG.

{{< gist aspose-com-gists 5048ca45afa67017c1271181930e213a "excel-to-svg.cs" >}}

## Get a Free License {#Get-a-Free-License}

Get a [temporary license][17] and use Aspose.Cells for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to convert Excel XLSX or XLS files to SVG using C#. You can perform this conversion to embed the content of the Excel worksheets into your applications. Besides, you can also explore other features of Aspose.Cells for .NET using the [documentation][18]. Also, you can ask your questions via our [forum][19].

## See Also

*   [Create, Read, and Edit Excel Spreadsheets in ASP.NET MVC][20]
*   [Create Excel Files in C# without MS Office][21]




[1]: https://docs.fileformat.com/spreadsheet/xlsx/
[2]: https://docs.fileformat.com/spreadsheet/xl/
[3]: https://docs.fileformat.com/page-description-language/svg/
[4]: https://docs.fileformat.com/spreadsheet/xlsx/
[5]: https://docs.fileformat.com/spreadsheet/xl/
[6]: https://docs.fileformat.com/page-description-language/svg/
[7]: #Excel-to-SVG-Converter
[8]: #Convert-Excel-XLSX-or-XLS-to-SVG
[9]: https://products.aspose.com/cells/net
[10]: https://downloads.aspose.com/cells/net
[11]: https://www.nuget.org/packages/Aspose.Cells
[12]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[13]: https://apireference.aspose.com/cells/net/aspose.cells/workbook/properties/worksheets
[14]: https://apireference.aspose.com/cells/net/aspose.cells.rendering/imageorprintoptions
[15]: https://apireference.aspose.com/cells/net/aspose.cells.rendering/sheetrender
[16]: https://apireference.aspose.com/cells/net/aspose.cells.rendering.sheetrender/toimage/methods/4
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/cells/net
[19]: https://forum.aspose.com/
[20]: https://blog.aspose.com/2021/08/25/create-read-edit-excel-spreadsheet-in-asp-net-mvc/
[21]: https://blog.aspose.com/2020/01/21/create-excel-xls-xlsx-programmatically-in-csharp-net/




