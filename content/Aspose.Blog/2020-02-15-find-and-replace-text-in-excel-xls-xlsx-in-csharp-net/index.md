---
title: 'Find and Replace Text in Excel Spreadsheets using C#'
seoTitle: ""
description: ""
date: Sat, 15 Feb 2020 02:50:46 +0000
draft: false
url: /2020/02/15/find-and-replace-text-in-excel-xls-xlsx-in-csharp-net/
author: Usman Aziz
summary: ''
tags: ['Find and Replace text in Excel', 'Replace text in Excel with Regex', 'find and replace text with regex in Excel']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Find-and-Replace-Text-in-Excel.png" alt="">}}


The **Excel** spreadsheets have minimized the efforts required to keep the huge data and perform complex calculations automatically. Excel automation was the next big achievement that has streamlined the way of creating Excel spreadsheets and performing a variety of operations on the data programmatically.

**Finding and replacing text in Excel** is one of the frequently performed operations in Excel automation. Therefore, in this article, I will show you how to **find and replace text** in large Excel spreadsheets programmatically in C# with a few lines of code. Ultimately, you will learn how to:

*   [Find and replace text in Excel Workbook in C#][1]
*   [Find and replace text in Excel Workbook using regular expression (Regex) in C#][2]

## API for Finding and Replacing Text in Excel Workbooks

[Aspose.Cells for .NET][3] is a powerful API that allows you to completely automate the process of creating, editing, parsing and converting the Excel spreadsheet programmatically. The API also provides easy ways of finding and replacing text based on the plain text as well as regular expressions (regex). You can either [download][4] the API or install it in your application via NuGet Package Manager or Package Manager Console.

### NuGet Package Manager



{{< figure align=center src="images/NPM-Aspose.Cells-for-.NET_.png" alt="Find and replace text with regex in Excel">}}


### Package Manager Console```
PM> Install-Package Aspose.Cells
```

## Find and Replace Text in Excel using C# {#Find-and-Replace-Text-in-Excel-using-CSharp}

The following is the simple recipe to find and replace text in an Excel workbook using _Aspose.Cells for .NET_.

*   Create an instance of [Workbook][5] class and initialize it with the path of the Excel file.
*   Create an instance of [ReplaceOptions][6] class and set options such as case sensitivity.
*   Call [Workbook.Replace(String, String, ReplaceOptions)][7] method to find and replace the text.
*   Save the updated Excel file using [Workbook.Save(String)][8] method.

The following code sample shows how to find and replace text in Excel using C#.

{{< gist aspose-com-gists bbb6f03f1f8945472afb885763e97437 "find-replace-text-in-Excel.cs" >}}

## Find and Replace Text with Regular Expression in Excel using C# {#Find-and-Replace-Text-with-Regular-Expression-in-Excel-using-CSharp}

You can also find and replace text that matches a particular pattern, such as Email IDs, SSN, etc. In order to do that, just set the [ReplaceOptions.RegexKey][9] property to _true_ and call [Workbook.Replace(String, String, ReplaceOptions)][10] method.

The following code sample shows how to find and replace the text with regex in the Excel workbook.

{{< gist aspose-com-gists bbb6f03f1f8945472afb885763e97437 "find-replace-text-in-Excel-with-Regex.cs" >}}

## Try Aspose.Cell for .NET for Free

Get a free [temporary license][11] of _Aspose.Cells for .NET_ and enjoy its powerful features.




[1]: #Find-and-Replace-Text-in-Excel-using-CSharp
[2]: #Find-and-Replace-Text-with-Regular-Expression-in-Excel-using-CSharp
[3]: https://products.aspose.com/cells
[4]: https://downloads.aspose.com/cells/net
[5]: https://apireference.aspose.com/net/cells/aspose.cells/workbook
[6]: https://apireference.aspose.com/net/cells/aspose.cells/replaceoptions
[7]: https://apireference.aspose.com/net/cells/aspose.cells.workbook/replace/methods/8
[8]: https://apireference.aspose.com/net/cells/aspose.cells.workbook/save/methods/2
[9]: https://apireference.aspose.com/net/cells/aspose.cells/replaceoptions/properties/regexkey
[10]: https://apireference.aspose.com/net/cells/aspose.cells.workbook/replace/methods/8
[11]: https://purchase.aspose.com/temporary-license





