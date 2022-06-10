---
title: 'Import Data from JSON to Excel Worksheet in C# .NET'
seoTitle: "JSON to Excel in C# | Convert JSON to Excel | Import JSON Data to Excel"
description: "JSON to Excel in C# programmatically. Convert JSON file to Excel in C#. Import JSON data to Excel worksheets. Convert JSON to XLS or XLSX in C#."
date: Fri, 03 Apr 2020 16:06:48 +0000
draft: false
url: /2020/04/03/import-data-from-json-to-excel-in-csharp-asp.net/
author: Usman Aziz
summary: ''
tags: ['Convert JSON to Excel CSharp', 'Import Data from JSON to Excel', 'JSON to Excel CSharp']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Convert-JSON-to-Excel-C.png" alt="Convert JSON to Excel C#">}}


**MS Excel** provides a variety of features to keep and organize tabular data in the form of worksheets. Along with data organization, you can perform various operations such as data sorting, graph plotting, mathematical computations and etc. [JSON][1], on the other hand, is a widely used format to store and transmit the data in the form of key-value pairs. Most often, it is used to transmit data from the server to the web pages. There could be the case when you receive the data in the form of JSON, i.e. from a web service, and want to save it into an Excel worksheet. In such a case, the optimal way is automating the process by importing data from **JSON to Excel** worksheets **programmatically**.

In order to deal with the above-mentioned scenario in ASP.NET or any C# based application, I'll show you how to import JSON data into Excel file. In this article, you will learn how to:

*   import data from JSON to Excel worksheet in C#
*   apply cell formatting when converting JSON to Excel in C#

In order to import data from JSON files, we'll leverage the capabilities of [Aspose.Cells for .NET][2]. It is a powerful API to manipulate spreadsheet files in .NET, .NET Core & Xamarin based applications. You can install the API's package from [NuGet][3] or download the DLL directly from the [Downloads][4] section.

## Import Data from JSON to Excel in C#

The following are the steps to import data from JSON to Excel XLSX:

*   Create a new [Workbook][5] object.
*   Read data from JSON using [System.IO.File.ReadAllText(string)][6] method.
*   Create an object of [JsonLayoutOptions][7] class to set additional options.
*   Import data from JSON to Excel using [JsonUtility.ImportData()][8] method.
*   Save the Excel file using [Workbook.Save(string)][9] method.

The following code sample shows how to import data from JSON to Excel in C#.

{{< gist aspose-com-gists 63a43ccabefb8f146067b64f50685de0 "JSON-to-Excel.cs" >}}

### Input JSON Data```
[
   {
       Name: "John Smith",
       Contract:
       [
           {
               Client:
               {
                   Name: "A Company"
               },
               Price: 1200000
           },
           {
               Client:
               {
                   Name: "B Ltd."
               },
               Price: 750000
           },
           {
               Client:
               {
                   Name: "C & D"
               },
               Price: 350000
           }
       ]
   },
   {
       Name: "Tony Anderson",
       Contract:
       [
           {
               Client:
               {
                   Name: "E Corp."
               },
               Price: 650000
           },
           {
               Client:
               {
                   Name: "F & Partners"
               },
               Price: 550000
           }
       ]
   },
   {
       Name: "Jimmy Adams",
       Contract:
       [
           {
               Client:
               {
                   Name: "MIT"
               },
               Price: 800000
           },
           {
               Client:
               {
                   Name: "SnB"
               },
               Price: 520000
           }
       ]
   },
]
```

### Output Excel Worksheet



{{< figure align=center src="images/JSON-to-Excel.png" alt="JSON to Excel">}}


## Import JSON to Excel with Formatting Styles in C#

You can also apply different styles to the Excel worksheet when importing the data from JSON file. The _CellsFactory_ class of Aspose.Cells for .NET provides a range of options to set various styling parameters such as font, color, alignment, border styles, etc. The following are the steps to import data from JSON to Excel along with the styling.

*   Create a new [Workbook][10] object.
*   Read the JSON file using [System.IO.File.ReadAllText(string)][11] method.
*   Create an object of the [CellsFactory][12] class.
*   Create style in [Style][13]'s object using [CellsFactory.CreateStyle()][14] method.
*   Set the desired properties such as _Style.Font.Color_.
*   Import data from JSON to Excel using [JsonUtility.ImportData()][15] method.
*   Save the Excel file using [Workbook.Save(string)][16] method.

The following code sample applies different styles when importing data from JSON to Excel in C#.

{{< gist aspose-com-gists 63a43ccabefb8f146067b64f50685de0 "JSON-to-Excel-styles.cs" >}}

### Output Excel Worksheet



{{< figure align=center src="images/JSON-to-Excel-C.png" alt="JSON to Excel C#">}}


## See Also

*   [Import Data from JSON to Excel in C#][17]

## Learn more about Aspose.Cells for .NET

You can explore more about Aspose.Cells for .NET using the [documentation][18] and the source code [examples][19].




[1]: https://en.wikipedia.org/wiki/JSON
[2]: https://products.aspose.com/cells/net
[3]: https://www.nuget.org/packages/Aspose.Cells
[4]: https://downloads.aspose.com/cells/net
[5]: https://apireference.aspose.com/net/cells/aspose.cells/workbook
[6]: https://docs.microsoft.com/en-us/dotnet/api/system.io.file.readalltext?view=netframework-4.8
[7]: https://apireference.aspose.com/net/cells/aspose.cells.utility/jsonlayoutoptions
[8]: https://apireference.aspose.com/net/cells/aspose.cells.utility/jsonutility/methods/importdata
[9]: https://apireference.aspose.com/net/cells/aspose.cells.workbook/save/methods/2
[10]: https://apireference.aspose.com/net/cells/aspose.cells/workbook
[11]: https://docs.microsoft.com/en-us/dotnet/api/system.io.file.readalltext?view=netframework-4.8
[12]: https://apireference.aspose.com/net/cells/aspose.cells/cellsfactory
[13]: https://apireference.aspose.com/net/cells/aspose.cells/style
[14]: https://apireference.aspose.com/net/cells/aspose.cells/cellsfactory/methods/createstyle
[15]: https://apireference.aspose.com/net/cells/aspose.cells.utility/jsonutility/methods/importdata
[16]: https://apireference.aspose.com/net/cells/aspose.cells.workbook/save/methods/2
[17]: https://blog.aspose.com/2019/04/20/import-data-from-json-using-aspose.cells-for-java-19.3/
[18]: https://docs.aspose.com/display/cellsnet/Introduction+of+Aspose.Cells+for+.NET
[19]: https://github.com/aspose-cells/Aspose.Cells-for-.NET





