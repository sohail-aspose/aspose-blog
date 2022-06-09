---
title: 'Export Excel Files to Stream using C#'
seoTitle: "Export Excel Files to Stream using C# | C# .NET Excel API"
description: "Use .NET Excel API to export Excel XLSX and XLS files to stream using C# or VB.NET. Load Excel files from stream programmatically."
date: Mon, 18 Oct 2021 17:00:27 +0000
draft: false
url: /2021/10/18/export-excel-to-stream-csharp/
author: Usman Aziz
summary: 'In various cases, you may need to export or save the Excel XLSX/XLS files to memory streams. For such cases, this article covers **how to export Excel files to FileStream objects dynamically using C#**. Moreover, you will learn how to load an Excel file from stream.'
tags: ['excel to stream csharp', 'xls to stream csharp', 'xlsx to stream csharp']
categories: ['Aspose.Cells Product Family']
---

In various cases, you may need to export or save the Excel XLSX/XLS files to memory streams. For such cases, this article covers **how to export Excel files to FileStream objects dynamically using C#**. Moreover, you will learn how to load an Excel file from stream.

*   [C# API to Export Excel Files to Stream][1]
*   [Export Excel File to Stream][2]
*   [Load Excel File from Stream][3]

## C# API to Export Excel Files to Stream {#API-to-Export-Excel-Files-to-Stream}

In order to export an Excel file to stream, we'll use [Aspose.Cells for .NET][4]. It is a feature-rich API that lets you create and manipulate Excel files. You can either [download][5] the API's DLL or install it via [NuGet][6].

```
PM> Install-Package Aspose.Cells
```

## Export an Excel File to Stream in C# {#Export-Excel-File-to-Stream}

The following are the steps to export an Excel file to stream using C#.

*   Load the Excel file using [Workbook][7] class.
*   Create a new [FileStream][8] object.
*   Export Excel file to stream using [Workbook.Save(FileStream, SaveFormat)][9] method.

The following code sample shows how to export an Excel XLSX file to a FileStream object.

{{< gist aspose-com-gists 55db5ebdaec2236e66a64dad5608fa26 "export-excel-to-stream.cs" >}}

## Load Excel File from Stream {#Load-Excel-File-from-Stream}

Aspose.Cells for .NET also allows you to load the Excel files from stream. The following are the steps to achieve this.

*   Create a new [FileStream][10] object and load the Excel file into it.
*   Create a new [Workbook][11] object and initialize it with the _FileStream_ object.
*   Perform the desired operations on the Excel file using _Workbook_ object.

The following code sample shows how to load an Excel file from a FileStream.

{{< gist aspose-com-gists 55db5ebdaec2236e66a64dad5608fa26 "load-excel-from-stream.cs" >}}

## Get a Free License {#Get-a-Free-License}

You can get a free [temporary license][12] and use the API without evaluation limitations.

## Conclusion

In this article, you have learned how to export Excel files to stream using C#. Moreover, you have seen how to load the Excel files from the stream dynamically. In addition, you can explore other features of Aspose.Cells for .NET using the [documentation][13]. Also, you can ask your questions via our [forum][14].

## See Also

*   [Create, Read, and Edit Excel Spreadsheets in ASP.NET MVC][15]
*   [Create Excel Files in C# without MS Office][16]




[1]: #API-to-Export-Excel-Files-to-Stream
[2]: #Export-Excel-File-to-Stream
[3]: #Load-Excel-File-from-Stream
[4]: https://products.aspose.com/cells/net
[5]: https://downloads.aspose.com/cells/net
[6]: https://www.nuget.org/packages/Aspose.Cells
[7]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[8]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream
[9]: https://apireference.aspose.com/cells/net/aspose.cells/workbook/methods/save
[10]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream
[11]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[12]: https://purchase.aspose.com/temporary-license
[13]: https://docs.aspose.com/cells/net
[14]: https://forum.aspose.com/
[15]: https://blog.aspose.com/2021/08/25/create-read-edit-excel-spreadsheet-in-asp-net-mvc/
[16]: https://blog.aspose.com/2020/01/21/create-excel-xls-xlsx-programmatically-in-csharp-net/




