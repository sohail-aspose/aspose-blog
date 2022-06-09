---
title: 'Import Data from JSON to Excel on Linux using .NET'
seoTitle: "Import Data from JSON to Excel in Linux | .NET API for Linux"
description: "Learn how to import data from JSON files to Excel worksheets on Linux. Apply styles while converting JSON files to Excel on Linux."
date: Thu, 16 Sep 2021 02:46:00 +0000
draft: false
url: /2021/09/16/import-data-from-json-to-excel-on-linux/
author: Usman Aziz
summary: '**MS Excel** is a rich spreadsheet manipulation software that allows you to organize the data in the form of worksheets and workbooks. Alongside, it provides features such as data sorting, graph plotting, mathematical computations and etc. On the other hand, [JSON][1] is a popular format to store structured data. In certain cases, JSON data needs to be converted to Excel worksheets. For such cases, this article shows **how to import data from JSON files to Excel worksheets on Linux**.'
tags: ['JSON to Excel Linux', 'JSON to XLS Linux', 'JSON to XLSX Linux']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Convert-JSON-to-Excel-C.png" alt="Convert JSON to Excel Linux">}}


**MS Excel** is a rich spreadsheet manipulation software that allows you to organize the data in the form of worksheets and workbooks. Alongside, it provides features such as data sorting, graph plotting, mathematical computations and etc. On the other hand, [JSON][2] is a popular format to store structured data. In certain cases, JSON data needs to be converted to Excel worksheets. For such cases, this article shows **how to import data from JSON files to Excel worksheets on Linux**.

## .NET JSON to Excel Converter API for Linux {#Excel-to-PDF-Converter-API-for-Linux}

For importing data from JSON files to Excel worksheets, we will use [Aspose.Cells for .NET][3]. It is a feature-rich API that allows you to create, manipulate, and convert Excel files. In order to use this API on Linux, you need to set up .NET environment, which can be done within a few steps. The following are the prerequisites that you would need to set up the environment.

*   [Visual Studio Code][4]
*   [.NET 5.0 SDK][5]
*   [C# Extension][6]

Once you have set up the environment and created the application, you can proceed to install Aspose.Cells for .NET via [NuGet][7] using [NuGet Package Manager extension][8] for Visual Studio Code.

Learn [how to create a console application on Linux][9] using Visual Studio Code.

## Import Data from JSON to Excel on Linux

The following are the steps to import data from JSON to Excel XLSX:

*   Create a new [Workbook][10] object.
*   Read data from JSON using [System.IO.File.ReadAllText(string)][11] method.
*   Create an object of [JsonLayoutOptions][12] class to set additional options.
*   Import data from JSON to Excel using [JsonUtility.ImportData()][13] method.
*   Save the Excel file using [Workbook.Save(string)][14] method.

The following code sample shows how to import data from JSON to Excel on Linux.

{{< gist aspose-com-gists a7ed590da1f74edfaa1dc79fbc4502bf "JSON-to-Excel.cs" >}}

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



{{< figure align=center src="images/JSON-to-Excel.png" alt="JSON to Excel Linux">}}


## Import JSON to Excel with Formatting Styles

While importing the data from the JSON file, you can apply styles to the output Excel file. The following are the steps to perform this operation.

*   Create a new [Workbook][15] object.
*   Read the JSON file using [System.IO.File.ReadAllText(string)][16] method.
*   Create an object of the [CellsFactory][17] class.
*   Create style in [Style][18]'s object using [CellsFactory.CreateStyle()][19] method.
*   Set the desired properties such as _Style.Font.Color_.
*   Import data from JSON to Excel using [JsonUtility.ImportData()][20] method.
*   Save the Excel file using [Workbook.Save(string)][21] method.

The following code sample shows how to apply styles while importing data from JSON to Excel on Linux.

{{< gist aspose-com-gists a7ed590da1f74edfaa1dc79fbc4502bf "JSON-to-Excel-styles.cs" >}}

### Output Excel Worksheet



{{< figure align=center src="images/JSON-to-Excel-C.png" alt="JSON to Excel Linux">}}


## Get a Free License {#Get-a-Free-License}

You can get a [temporary license][22] and use Aspose.Cells for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to import JSON data to Excel worksheets on Linux. In addition, you have seen how to apply styles in JSON to Excel conversion. Furthermore, you can explore more about Aspose.Cells for .NET using the [documentation][23]. Also, you can ask your questions via our [forum][24].

## See Also

*   [Convert Excel Files to PDF on Linux][25]
*   [CSV to Excel or Excel to CSV on Linux][26]




[1]: https://en.wikipedia.org/wiki/JSON
[2]: https://en.wikipedia.org/wiki/JSON
[3]: https://products.aspose.com/cells/net
[4]: https://code.visualstudio.com/
[5]: https://dotnet.microsoft.com/download
[6]: https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp
[7]: https://www.nuget.org/packages/Aspose.Cells
[8]: https://marketplace.visualstudio.com/items?itemName=jmrog.vscode-nuget-package-manager
[9]: https://docs.microsoft.com/en-us/dotnet/core/tutorials/with-visual-studio-code
[10]: https://apireference.aspose.com/net/cells/aspose.cells/workbook
[11]: https://docs.microsoft.com/en-us/dotnet/api/system.io.file.readalltext?view=netframework-4.8
[12]: https://apireference.aspose.com/net/cells/aspose.cells.utility/jsonlayoutoptions
[13]: https://apireference.aspose.com/net/cells/aspose.cells.utility/jsonutility/methods/importdata
[14]: https://apireference.aspose.com/net/cells/aspose.cells.workbook/save/methods/2
[15]: https://apireference.aspose.com/net/cells/aspose.cells/workbook
[16]: https://docs.microsoft.com/en-us/dotnet/api/system.io.file.readalltext?view=netframework-4.8
[17]: https://apireference.aspose.com/net/cells/aspose.cells/cellsfactory
[18]: https://apireference.aspose.com/net/cells/aspose.cells/style
[19]: https://apireference.aspose.com/net/cells/aspose.cells/cellsfactory/methods/createstyle
[20]: https://apireference.aspose.com/net/cells/aspose.cells.utility/jsonutility/methods/importdata
[21]: https://apireference.aspose.com/net/cells/aspose.cells.workbook/save/methods/2
[22]: https://purchase.aspose.com/temporary-license
[23]: https://docs.aspose.com/cells/net
[24]: https://forum.aspose.com/
[25]: https://blog.aspose.com/2021/10/12/convert-excel-files-to-pdf-on-linux/
[26]: https://blog.aspose.com/2021/10/21/csv-to-excel-or-excel-to-csv-on-linux/




