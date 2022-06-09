---
title: 'Merge or Unmerge Cells in Excel Worksheet with C#'
seoTitle: ""
description: ""
date: Wed, 24 Jun 2020 23:08:52 +0000
draft: false
url: /2020/06/24/merge-unmerge-cells-excel-csharp/
author: Farhan Raza
summary: ''
tags: ['Split cells', 'merge cells', 'merge cells in excel', 'merge cells in named range', 'merge range of cells', 'unmerge cells', 'unmerge cells in excel']
categories: ['Aspose.Cells Product Family']
---

In this article, you will learn about how to merge or unmerge Excel cells in a worksheet. Generally, merging cells refers to one or more cells joined together to form a large cell. However, the adjacent cells can be merged vertically or horizontally. Whereas, converting a large cell into multiple cells is known as unmerging or splitting cells in Excel worksheet. Let us explore the following use cases:

*   [Merge Excel Cells in Worksheet with C#][1]
*   [Unmerge Excel Cells in Worksheet with C#][2]
*   [Merge a Range of Excel Cells in Worksheet with C#][3]
*   [Unmerge a Range of Excel Cells in Worksheet with C#][4]
*   [Merge Excel Cells of Named Range in Worksheet with C#][5]

## Merge Excel Cells in Worksheet with C# {#section1}

You can easily merge cells in excel worksheet with [Aspose.Cells for .NET][6] API using C#. In this example, we will be creating a new excel worksheet from scratch and then merge a few cells by following below steps:

1.  Create a [Workbook][7] object
2.  Get first worskeet
3.  [Merge][8] specific cells
4.  Put value in merged cell
5.  Apply styles on the cell
6.  Save output excel worksheet

Below code snippet shows how to merge cells in Excel worksheet with C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "MergeCells.cs" >}}

The output file generated from this code snippet will contain merged cells as in the screenshot below:



{{< figure align=center src="images/Merge_Cells.png" alt="Merge Cells">}}


## Unmerge Excel Cells in Worksheet with C# {#section2}

We have learned how to merge cells in Excel file. Let us take this process another step further. Here we will be considering to unmerge cells in Excel worksheet by following the steps below:

1.  Load source Excel file
2.  Create [Worksheet][9] object and access first sheet
3.  [Unmerge][10] the cells
4.  Save output file

The code snippet below is based on these steps and shows how to unmerge cells in Excel file with C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "UnmergeCells.cs" >}}

The following image shows how do the unmerged cells look when you run the above code in your environment:



{{< figure align=center src="images/Unmerge_Cells.png" alt="Unmerge Cells">}}


## Merge a Range of Excel Cells in Worksheet with C# {#section3}

Sometimes there are several cells specified under different ranges of cells. You might want to merge a specific range of cells in Excel sheet. In such scenarios, please follow the steps listed below:

1.  Create a [Workbook][11] object
2.  Access the first [worksheet][12]
3.  Input data in a Cell
4.  Create and [Merge][13] the Range
5.  Save output excel file

The code snippet below shows how to merge range of cells into one larger cell in Excel file using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "Merge_Range.cs" >}}

## Unmerge a Range of Excel Cells in Worksheet with C# {#section4}

We have explored merging a range of cells in Excel in the previous example. Let us move on to unmerging the merged cells by following the steps below:

1.  Load source [Workbook][14]
2.  Access specific [Worksheet][15]
3.  Create a [Range][16] object
4.  Call [UnMerge][17] method
5.  Save output Excel file

The code snippet below follows these steps and shows how to unmerge a range of cells in Excel worksheet using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "Unmerge_Range.cs" >}}

## Merge Excel Cells of Named Range in Worksheet with C# {#section5}

Sometimes the Excel files contain several named ranges because it is easy to identify and manipulate accordingly. Therefore, you can also merge any named range by specifying its name. Resultantly, all the cells in that named range will be merged into one bigger cell. You need to follow these steps:

1.  Load source Excel [Workbook][18]
2.  Access the [Worksheet][19] containing the named range
3.  Define and Apply style
4.  [Merge][20] Named Range
5.  Save output file

The code snippet below explains how to merge cells in a named range in C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "Merge_Named_Range.cs" >}}

The output of the above code snippet will be the same as the following image:



{{< figure align=center src="images/Merge_Named_Range.png" alt="Merge Named Range">}}


## Conclusion

Merging or unmerging cells in Excel Workbooks and Worksheets is an important and useful feature. We have compiled different possible use cases in this article along with all the steps and images. Now you can easily follow these steps and merge or unmerge cells, ranges, or named ranges in Excel files. In case of any query or concern, you may please contact us via [Free Support Forum][21].

## See Also

[Import Data from JSON to Excel Worksheet in C# .NET][22]




[1]: #section1
[2]: #section2
[3]: #section3
[4]: #section4
[5]: #section5
[6]: https://products.aspose.com/cells/net
[7]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[8]: https://apireference.aspose.com/cells/net/aspose.cells/cells/methods/merge/index
[9]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[10]: https://apireference.aspose.com/cells/net/aspose.cells/cells/methods/unmerge
[11]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[12]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[13]: https://apireference.aspose.com/cells/net/aspose.cells/range/methods/merge
[14]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[15]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[16]: https://apireference.aspose.com/cells/net/aspose.cells/range
[17]: https://apireference.aspose.com/cells/net/aspose.cells/range/methods/unmerge
[18]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[19]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[20]: https://apireference.aspose.com/cells/net/aspose.cells/range/methods/merge
[21]: https://forum.aspose.com/c/cells
[22]: https://blog.aspose.com/2020/04/03/import-data-from-json-to-excel-in-csharp-asp.net/





