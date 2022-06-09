---
title: 'Add or Remove AutoFilter in Excel File (XLSX/XLS) using C#'
seoTitle: ""
description: ""
date: Wed, 16 Sep 2020 11:22:46 +0000
draft: false
url: /2020/09/16/add-remove-autofilter-in-excel-file-csharp/
author: Farhan Raza
summary: 'XLSX and XLS file formats are frequently used to manipulate huge data. Likewise, AutoFilters are used to organize data in Excel files. You can easily add or remove data filters in Excel files with Aspose.Cells for .NET API. Filters can be used to quantify some data to extract some meaningful information. For example, an organization wants to filter the months with low sales, in order to devise and improve their strategies.'
tags: ['add autofilter in xlsx', 'autofilter in excel', 'remove autofilter']
categories: ['Aspose.Cells Product Family']
---

[XLSX][1] and [XLS][2] file formats are frequently used to manipulate huge data. Likewise, AutoFilters are used to organize data in Excel files. You can easily add or remove AutoFilter in Excel files with [Aspose.Cells for .NET][3] API. Filters can be used to quantify some data to extract some meaningful information. For example, an organization wants to filter the months with low sales, in order to devise and improve their strategies. In this article, we will explore data filtering using auto filters in C#:

*   [Add or Remove AutoFilter in Excel Files - API Installation][4]
*   [Apply AutoFilter on Cells in Excel Files using C#][5]
*   [Add Date AutoFilter in XLSX using C#][6]
*   [Add Dynamic Date AutoFilter in XLSX using C#][7]
*   [Apply Custom Number AutoFilter in XLSX with C#][8]
*   [Add Custom AutoFilter with Contains using C#][9]
*   [Remove or Delete AutoFilter in Excel using C#][10]

## Add or Remove AutoFilter in Excel Files - API Installation {#section1}

[Aspose.Cells for .NET][11] API efficiently lets you work with Excel spreadsheets. You can create, edit, or manipulate XLS, XLSX, and other supported formats programmatically with minimal code. You can download and install the MSI or ZIP package from the [Downloads section][12], or simply install it via the [NuGet][13] gallery in your solution. For example, you can easily install it in your environment using the following command:

\> _Install-Package Aspose.Cells -Version 20.9.0_

After installing the API successfully, let us proceed with some of the important and useful use cases:

## Apply AutoFilter on Cells in Excel Files using C# {#section2}

You can apply AutoFilter on a specific range of cells in Excel files. This allows you to sort the values in ascending or descending order as well as other number filters when the cells contain numerical values. You need to follow the following steps for applying AutoFilter in Excel files using C#:

1.  Open an Excel file and access the [Worksheet][14]
2.  Create [AutoFilter][15] by specifying specific cell range
3.  Save output XLS/XLSX file

The code snippet shows how to apply AutoFilter on cells in Excel file using C#:

{{< gist aspose-com-gists d4ed7d6727eb31ca859668af927ffa2c "ApplyAutofilter.cs" >}}

You can notice the AutoFilter added in source XLSX file in the screenshot below:



{{< figure align=center src="images/AutoFilter-Excel-Csharp.png" alt="AutoFilter-Excel-Csharp">}}


## Add Date AutoFilter in XLSX using C# {#section3}

Data in Excel files often contain information related to dates. Sometimes you might need to explore information based on different time periods that can be identified by the dates. For example, let us consider the case where we need to filter data related to January 2018 then you need to follow the following steps:

1.  Load input spreadsheet
2.  Accessing a worksheet
3.  Add Date Filter and save the output file

The following code sample follows these steps and shows how to add Date AutoFilter in Excel files using C#:

{{< gist aspose-com-gists d4ed7d6727eb31ca859668af927ffa2c "DateAutoFilter.cs" >}}

## Add Dynamic Date AutoFilter in XLSX using C# {#section4}

As we have already discussed the scenario of filtering data based on dates. However, the date scenario can be a little more generic as well, in some scenarios. For example, we need the data to be filtered out for January month irrespective of which year. Such requirements can easily be handled with a dynamic date filter by using the steps below:

1.  Load input XLSX file
2.  Access a worksheet
3.  Set [DynamicFilter][16] for January month
4.  Save output Excel sheet

This example is in continuation of the above example, where the code snippet below shows how to add a dynamic date AutoFilter in an Excel file using C#:

{{< gist aspose-com-gists d4ed7d6727eb31ca859668af927ffa2c "DynamicDateAutoFilter.cs" >}}

## Apply Custom Number AutoFilter in XLSX with C# {#section5}

You can filter data based on a custom range of numbers using Aspose.Cells for .NET API. For instance, when a company needs to access how many of its employees have achieved sales targets. Likewise, there could be a lot of possibilities where this filtering technique can help. Let us assume a case where we need to filter all data where the numbers are within the range of 5 and 10 inclusively, then you need to follow the below steps:

1.  Instantiate a [Workbook][17] object and load the input file
2.  Add custom number filter in a specific worksheet
3.  Save output Excel file

Based on these steps, the following code shows how to add custom number AutoFilter using C#:

{{< gist aspose-com-gists d4ed7d6727eb31ca859668af927ffa2c "CustomNumberAutoFilter.cs" >}}

## Add Custom AutoFilter with Contains using C# {#section6}

Moving another step further from custom number AutoFilter, let us learn how to add Custom AutoFilter which can be used to track specific text using Contains Filter Operator. It can be useful to search for words where any text is partially or fully present in the data. You should follow the following steps to achieve these requirements:

1.  Load input Excel file with data
2.  Specify [AutoFilter][18] range and the [FilterOperatorType][19]
3.  Save output XLSX file

The code snippet below shows how to add Custom AutoFilter with Contains using C#:

{{< gist aspose-com-gists d4ed7d6727eb31ca859668af927ffa2c "ContainAutoFilter.cs" >}}

## Remove or Delete AutoFilter in Excel using C# {#section7}

As we have learned different scenarios of adding AutoFilters in Excel files using C#, let us check out the other way around. The use case of removing or deleting the AutoFilters from Excel is equally important and pivotal. You need to follow the steps below for removing all AutoFilters from an XLSX file:

1.  Load input XLSX file
2.  Iterate through each worksheet and remove [AutoFilters][20]
3.  Save output file

The following code snippet shows how to remove AutoFilters from Excel files using C#:

{{< gist aspose-com-gists d4ed7d6727eb31ca859668af927ffa2c "RemoveAutoFilter.cs" >}}

## Conclusion

Aspose.Cells for .NET API offers you different out of the box features. Adding, removing, or deleting an AutoFilter using C# in .NET Framework is simple and easy. We have discussed several possibilities in detail. In case you have any doubts or concerns, please feel free to contact us at [Free Support Forum][21].

## See Also

[Convert CSV to Excel or Excel to CSV File using Java][22]




[1]: https://docs.fileformat.com/spreadsheet/xlsx/
[2]: https://docs.fileformat.com/spreadsheet/xls/
[3]: https://products.aspose.com/cells/net
[4]: #section1
[5]: #section2
[6]: #section3
[7]: #section4
[8]: #section5
[9]: #section6
[10]: #section7
[11]: https://products.aspose.com/cells
[12]: https://downloads.aspose.com/cells/net
[13]: http://nuget.org/packages/Aspose.Cells
[14]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[15]: https://apireference.aspose.com/cells/net/aspose.cells/autofilter
[16]: https://apireference.aspose.com/cells/net/aspose.cells/dynamicfilter
[17]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[18]: https://apireference.aspose.com/cells/net/aspose.cells/autofilter
[19]: https://apireference.aspose.com/cells/net/aspose.cells/filteroperatortype
[20]: https://apireference.aspose.com/cells/net/aspose.cells/autofilter
[21]: https://forum.aspose.com/c/cells
[22]: https://blog.aspose.com/2020/09/10/convert-csv-excel-java/





