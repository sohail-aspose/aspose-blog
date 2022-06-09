---
title: 'Split Text to Columns in Excel using C#'
seoTitle: "Split Text to Columns in Excel in C# | Split Text into Multiple Columns"
description: "Use .NET Excel API to split text to columns in Excel files using C#. Split text in a column into multiple columns programmatically in ASP.NET."
date: Sat, 24 Apr 2021 09:17:00 +0000
draft: false
url: /2021/04/24/split-text-to-columns-in-excel-using-csharp/
author: Usman Aziz
summary: 'Text to columns feature in MS Excel allows you to split text in a column into multiple columns. You can split the text on a blank space, a comma, or any other character. In order to automate the feature, this article covers **how to split text to columns in Excel files using C#**.'
tags: ['Csharp Split Text to Column in Excel', 'Split Text to Columns in Excel Csharp']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Text-to-Column-C.jpg" alt="Split Text to Columns in Excel C#">}}


Text to columns feature in MS Excel allows you to split text in a column into multiple columns. You can split the text on a blank space, a comma, or any other character. In order to automate the feature, this article covers **how to split text to columns in Excel files using C#**.

*   [API to Split Text to Columns in Excel][1]
*   [Split Text to Columns in Excel][2]

## C# API to Split Text to Columns in Excel {#API-to-Split-Text-to-Column-in-Excel}

In order to split text into columns in Excel files, we'll use [Aspose.Cells for .NET][3]. It is a spreadsheet manipulation API that lets you create, modify or convert Excel files in .NET applications. You can either [download][4] the API or install it using NuGet.

```
PM> Install-Package Aspose.Cells
```

## Split Text to Columns in Excel {#Split-Text-to-Columns-in-Excel}

The following are the steps to split text to columns in Excel using C#.

*   Load the Excel file using the [Workbook][5] class.
*   Get the reference of the [Worksheet][6] in which you want to perform text to columns operation.
*   Insert data into the worksheet (optional).
*   Create an instance of [TxtLoadOptions][7] class and set text separator character using [TxtLoadOptions.Separator][8] property.
*   Split text to columns using [Worksheet.Cells.TextToColumns(int row, int column, int totalRows, TxtLoadOptions options)][9] method.
*   Save the updated Excel file using [Workbook.Save(string)][10] method.

The following code sample shows how to split text to columns in Excel.

{{< gist aspose-com-gists 67152c52a3ecfd712fe060c0c0a9b4be "text-to-column.cs" >}}

### Output



{{< figure align=center src="images/Text-to-Column-in-Excel.jpg" alt="Split Text to Column in Excel">}}


## Get a Free API License {#Get-a-Free-API-License}

You can [get a temporary license][11] in order to use the API without evaluation limitations.

## Conclusion

In this article, you have learned how to split text to columns in Excel files using C#. The code sample has shown how easy it is to split the text to columns based on a particular character. You can explore more about Aspose.Cells for .NET using the [documentation][12]. In case you would have any queries, contact us via our [forum][13].

## See Also

*   [Create Excel Files in C# without MS Office][14]




[1]: #API-to-Split-Text-to-Column-in-Excel
[2]: #Split-Text-to-Columns-in-Excel
[3]: https://products.aspose.com/cells/net
[4]: https://downloads.aspose.com/cells/net
[5]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[6]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[7]: https://apireference.aspose.com/cells/net/aspose.cells/txtloadoptions
[8]: https://apireference.aspose.com/cells/net/aspose.cells/txtloadoptions/properties/separator
[9]: https://apireference.aspose.com/cells/net/aspose.cells/cells/methods/texttocolumns
[10]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/2
[11]: https://purchase.aspose.com/temporary-license
[12]: https://docs.aspose.com/cells/net
[13]: https://forum.aspose.com/
[14]: https://blog.aspose.com/2020/01/21/create-excel-xls-xlsx-programmatically-in-csharp-net/





