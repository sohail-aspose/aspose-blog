---
title: 'Convert JSON to CSV Programmatically using C#'
seoTitle: "Covert JSON to CSV in C# | C# .NET API | Source Code"
description: "Use .NET Spreadsheet API to convert JSON data or files to CSV format using C# or VB.NET. Automate JSON to CSV conversion in your .NET applications."
date: Mon, 04 Oct 2021 09:14:00 +0000
draft: false
url: /2021/10/04/convert-json-to-csv-using-csharp/
author: Usman Aziz
summary: '[JSON][1] is an immensely used format to store structured data. In various cases, JSON files are used to transmit data between applications. Alongside, [CSV][2] is also used to store the data as comma separated values. In this article, you will learn how to import data from JSON files to CSV programmatically. Particularly, the article will cover **how to convert JSON data to CSV using C#**.'
tags: ['Convert JSON Data or File to CSV CSharp', 'Csharp API for JSON to CSV Conversion', 'JSON to CSV Csharp']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Convert-JSON-to-CSV.jpg" alt="JSON to CSV in C#">}}


[JSON][3] is an immensely used format to store structured data. In various cases, JSON files are used to transmit data between applications. Alongside, [CSV][4] is also used to store the data as comma separated values. In this article, you will learn how to import data from JSON files to CSV programmatically. Particularly, the article will cover **how to convert JSON data to CSV using C#**.

*   [API for JSON to CSV Conversion][5]
*   [Convert JSON Data or File to CSV][6]

## C# API for JSON to CSV Conversion {#API-for-JSON-to-CSV-Conversion}

In order to convert JSON data to CSV, we will use [Aspose.Cells for .NET][7]. It is a powerful API for creating, modifying, and converting spreadsheet files from within .NET applications. You can either [download][8] the API or install it using [NuGet][9].

```
PM> Install-Package Aspose.Cells
```

## Convert a JSON Data or File to CSV {#Convert-JSON-Data-or-File-to-CSV}

The following are the steps to convert JSON data to CSV format using C#.

*   Create a new [Workbook][10] object.
*   Get reference of the first worksheet using [Workbook.Worksheets\[0\]][11] collection.
*   Create an object of [JsonLayoutOptions][12] class to set additional options.
*   Import data from JSON to CSV using [JsonUtility.ImportData()][13] method.
*   Save the CSV file using [Workbook.Save(string, SaveFormat.CSV)][14] method.

The following code sample shows how to convert JSON data to CSV format.

{{< gist aspose-com-gists a22c8d99c0265e8bf2e30473c6ecb824 "json-to-csv.cs" >}}

### JSON Data

The following is the JSON data that we used in the above code sample.

```
[{"nodeId":1,"reputation":1134},{"nodeId":2,"reputation":547},{"nodeId":3,"reputation":1703},{"nodeId":4,"reputation":-199},{"nodeId":5,"reputation":-306},{"nodeId":6,"reputation":-49},{"nodeId":7,"reputation":1527},{"nodeId":8,"reputation":1223}]'
```

### Converted CSV

The following is the converted CSV file.



{{< figure align=center src="images/JSON-to-CSV.jpg" alt="JSON to CSV">}}


## Get a Free License {#Get-a-Free-License}

Get a [temporary license][15] and use Aspose.Cells for .NET without evaluation limitations.

## Conclusion

JSON and CSV files are widely used to store and exchange data within applications. Accordingly, this article covered how to convert JSON data or files to CSV using C#. Besides, you can also explore Aspose.Cells for .NET using the [documentation][16]. Also, you can ask your questions via our [forum][17].

## See Also

*   [Create, Read, and Edit Excel Spreadsheets in ASP.NET MVC][18]
*   [Create Excel Files in C# without MS Office][19]




[1]: https://docs.fileformat.com/web/json/
[2]: https://docs.fileformat.com/spreadsheet/csv/
[3]: https://docs.fileformat.com/web/json/
[4]: https://docs.fileformat.com/spreadsheet/csv/
[5]: #API-for-JSON-to-CSV-Conversion
[6]: #Convert-JSON-Data-or-File-to-CSV
[7]: https://products.aspose.com/cells/net
[8]: https://downloads.aspose.com/cells/net
[9]: https://www.nuget.org/packages/Aspose.Cells
[10]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[11]: https://apireference.aspose.com/cells/net/aspose.cells/workbook/properties/worksheets
[12]: https://apireference.aspose.com/cells/net/aspose.cells.utility/jsonlayoutoptions
[13]: https://apireference.aspose.com/cells/net/aspose.cells.utility/jsonutility/methods/importdata
[14]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/3
[15]: https://purchase.aspose.com/temporary-license
[16]: https://docs.aspose.com/cells/net
[17]: https://forum.aspose.com/
[18]: https://blog.aspose.com/2021/08/25/create-read-edit-excel-spreadsheet-in-asp-net-mvc/
[19]: https://blog.aspose.com/2020/01/21/create-excel-xls-xlsx-programmatically-in-csharp-net/




