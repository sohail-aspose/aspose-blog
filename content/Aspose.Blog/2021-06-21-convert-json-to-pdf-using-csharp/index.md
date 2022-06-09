---
title: 'Convert JSON to PDF using C#'
seoTitle: "Convert JSON to PDF in C# | JSON to PDF in .NET, .NET Core, Xamarin"
description: "Use .NET Excel API to convert JSON data to PDF using C#. Import JSON data and convert it to PDF from within ASP.NET, .NET Core or Xamarin."
date: Mon, 21 Jun 2021 09:28:00 +0000
draft: false
url: /2021/06/21/convert-json-to-pdf-using-csharp/
author: Usman Aziz
summary: 'In various cases, you may need to convert the JSON files to PDF for sharing, printing, or other purposes. To achieve it programmatically, this article covers **how to convert JSON to PDF using C#**.'
tags: ['Convert JSON Data to PDF in csharp', 'csharp API for JSON to PDF Conversion', 'json to pdf csharp']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/JSON-to-PDF.jpg" alt="JSON to PDF C#">}}


In various cases, you may need to convert the [JSON][1] files to [PDF][2] for sharing, printing, or other purposes. To achieve it programmatically, this article covers **how to convert JSON to PDF using C#**.

*   [API for JSON to PDF Conversion][3]
*   [Convert JSON Data to PDF][4]

## C# API for JSON to PDF Conversion {#API-for-JSON-to-PDF-Conversion}

In order to convert JSON files to PDF format, we will use [Aspose.Cells for .NET][5]. It is a powerful API that allows you to generate spreadsheet documents from scratch. In addition, it lets you process and convert existing Excel files from within your .NET applications. You can either [download][6] the API or install it using [NuGet][7].

```
PM> Install-Package Aspose.Cells
```

## Convert JSON to PDF in C# {#Convert-JSON-to-PDF-in-Csharp}

The following are the steps to convert a JSON file to PDF using C#.

1.  Create an instance of the [Workbook][8] class.
2.  Select the default [Worksheet][9] from the [Worksheets][10] collection.
3.  Load JSON data from file using [File.ReadAllText(string)][11] method.
4.  Create an instance of [JsonLayoutOptions][12] and set options.
5.  Import data from JSON to worksheet using [JsonUtility.ImportData][13] method with reference to [Worksheet][14] object and JSON data.
6.  Convert JSON to PDF by saving the workbook as PDF using [Workbook.Save(string, SaveFormat.Auto)][15] method.

The following code sample shows how to convert a JSON file to PDF.

{{< gist aspose-com-gists c2069dec63948fd44fcdfb23ad3914d3 "json-to-pdf.cs" >}}

## Get a Free License {#Get-a-Free-License}

You can use Aspose.Cells for .NET without evaluation limitations using a [temporary license][16].

## Conclusion

In this article, you have learned how to import JSON data and convert it to PDF using C#. You can use the provided code sample within your .NET, .NET Core, Mono or Xamarin based applications. In addition, you can explore the [documentation][17] of Aspose.Cells for .NET. Also, you can post your queries on our [forum][18].

## See Also

*   [Convert PDF to TXT or TXT to PDF using C#][19]
*   [Convert Excel to PDF in C#][20]




[1]: https://docs.fileformat.com/web/json/
[2]: https://docs.fileformat.com/pdf/
[3]: #API-for-JSON-to-PDF-Conversion
[4]: #Convert-JSON-to-PDF-in-Csharp
[5]: https://products.aspose.com/cells/net
[6]: https://downloads.aspose.com/cells/net
[7]: https://www.nuget.org/packages/Aspose.cells
[8]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[9]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[10]: https://apireference.aspose.com/cells/net/aspose.cells/workbook/properties/worksheets
[11]: https://docs.microsoft.com/en-us/dotnet/api/system.io.file.readalltext
[12]: https://apireference.aspose.com/cells/net/aspose.cells.utility/jsonlayoutoptions
[13]: https://apireference.aspose.com/cells/net/aspose.cells.utility/jsonutility/methods/importdata
[14]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[15]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/3
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/cells/net
[18]: https://forum.aspose.com/
[19]: https://blog.aspose.com/2020/09/28/convert-pdf-text-csharp-vb.net/
[20]: https://blog.aspose.com/2019/11/29/convert-xls-and-xlsx-to-pdf-in-csharp/





