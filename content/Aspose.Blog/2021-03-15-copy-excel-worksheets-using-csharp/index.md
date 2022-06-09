---
title: 'Copy or Move Excel Worksheets using C#'
seoTitle: "Copy Excel Worksheets using C# | Move Worksheets in Excel in C#"
description: "Move or copy Excel worksheets using C#. Copy worksheet within an Excel workbook or different workbooks using C#. Move sheets in a workbook."
date: Mon, 15 Mar 2021 16:23:50 +0000
draft: false
url: /2021/03/15/copy-excel-worksheets-using-csharp/
author: Usman Aziz
summary: 'In certain cases, you may need to copy worksheets within an Excel workbook or from one workbook to another. On the other hand, moving worksheets to change their position within a workbook is also required in different scenarios. In order to perform the above-mentioned tasks programmatically, this article shows **how to copy worksheets within Excel workbooks using C#**. Furthermore, it also covers how to change the position of a worksheet in an Excel workbook.'
tags: ['Copy Worksheet within an Excel Workbook csharp', 'Copy a Worksheet from One Workbook to Another csharp', 'Csharp API to Copy Excel Worksheets', 'Move Worksheet from One Place to Another csharp']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Copy-Worksheets.jpg" alt="Copy Excel Worksheets in C#">}}


In certain cases, you may need to copy worksheets within an Excel workbook or from one workbook to another. On the other hand, moving worksheets to change their position within a workbook is also required in different scenarios. In order to perform the above-mentioned tasks programmatically, this article shows **how to copy Excel worksheets within workbooks using C#**. Furthermore, it also covers how to change the position of a worksheet in an Excel workbook.

*   [C# API to Copy Excel Worksheets][1]
*   [Copy Worksheets within an Excel Workbook][2]
*   [Copy Worksheets from One Workbook to Another][3]
*   [Move Worksheets from One Position to Another][4]
*   [Get a Free API License][5]

## C# API to Copy Excel Worksheets {#API-to-Copy-Excel-Worksheets}

In order to copy worksheets in Excel files, we'll leverage the powerful spreadsheet manipulation capabilities of [Aspose.Cells for .NET][6]. The API provides you with a wide range of features to generate and process Excel files from within your .NET applications. You can either [download][7] the API's binaries or install it using [NuGet][8].

```
PM> Install-Package Aspose.Cells
```

## Copy Excel Worksheets using C# {#Copy-Worksheet-within-an-Excel-Workbook}

The following are the steps to copy an Excel worksheet within a workbook using C#.

*   Load Excel file using [Workbook][9] class.
*   Retrieve worksheets in a [WorksheetCollection][10] object from [Workbook.Worksheets][11] property.
*   Use [WorksheetCollection.AddCopy(string)][12] method to copy the worksheet by providing its name.
*   Save the updated workbook using [Workbook.Save(string)][13] method.

The following code sample shows how to copy an Excel worksheet in a workbook.

{{< gist aspose-com-gists 7e9f7233ef97c85a88c76341dd8b4337 "copy-worksheet.cs" >}}

## Copy Excel Worksheets from One Workbook to Another {#Copy-a-Worksheet-from-One-Workbook-to-Another}

Now, let's have a look at how to copy a worksheet from one Excel workbook to another. The following are the steps to perform this operation.

*   Create an object of the [Workbook][14] class and load the source Excel file.
*   Create another object of the [Workbook][15] class and load the destination Excel file.
*   Copy worksheet from source to destination workbook using [destinationWorkbook.Worksheets\[int\].Copy(sourceWorkbook.Worksheets\[int\])][16] method.
*   Save the destination workbook using [Workbook.Save(string)][17] method.

The following code sample shows how to copy a worksheet from one workbook to another in C#.

{{< gist aspose-com-gists 7e9f7233ef97c85a88c76341dd8b4337 "copy-worksheet-between-workbooks.cs" >}}

## Move Worksheet from One Position to Another in C# {#Move-Worksheet-from-One-Place-to-Another}

There could be the case when you need to rearrange the positions of the worksheets in a workbook. You can do it by moving the worksheets to the desired positions by specifying the index. The following are the steps to move an Excel worksheet from one position to another.

*   Load Excel file using [Workbook][18] class.
*   Retrieve worksheets in a [WorksheetCollection][19] object using [Workbook.Worksheets][20] property.
*   Access the desired worksheet from worksheet collection into a [Worksheet][21] object.
*   Use [Worksheet.MoveTo(int)][22] method to move the worksheet to the specified index.
*   Save the updated workbook using [Workbook.Save(string)][23] method.

The following code sample shows how to move an Excel worksheet from one position to another using C#.

{{< gist aspose-com-gists 7e9f7233ef97c85a88c76341dd8b4337 "move-worksheet.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try and evaluate Aspose.Cells for .NET for free by requesting a [temporary license][24].

## Conclusion

In this article, you have learned how to copy Excel worksheets within a workbook or from one workbook to another using C#. Furthermore, you have seen how to move an Excel worksheet from one position to another within a workbook. You can explore other features of Aspose.Cells for .NET using the [documentation][25]. In case you would have any queries, feel free to post to our [forum][26].

## See Also

*   [Create MS Excel Files in C# without MS Office][27]




[1]: #API-to-Copy-Excel-Worksheets
[2]: #Copy-Worksheet-within-an-Excel-Workbook
[3]: #Copy-a-Worksheet-from-One-Workbook-to-Another
[4]: #Move-Worksheet-from-One-Place-to-Another
[5]: #Get-a-Free-API-License
[6]: https://products.aspose.com/cells/net
[7]: https://downloads.aspose.com/cells/net
[8]: https://nuget.org/packages/Aspose.Cells
[9]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[10]: https://apireference.aspose.com/cells/net/aspose.cells/worksheetcollection
[11]: https://apireference.aspose.com/cells/net/aspose.cells/workbook/properties/worksheets
[12]: https://apireference.aspose.com/cells/net/aspose.cells.worksheetcollection/addcopy/methods/1
[13]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/2
[14]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[15]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[16]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet/methods/copy
[17]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/2
[18]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[19]: https://apireference.aspose.com/cells/net/aspose.cells/worksheetcollection
[20]: https://apireference.aspose.com/cells/net/aspose.cells/workbook/properties/worksheets
[21]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[22]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet/methods/moveto
[23]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/2
[24]: https://purchase.aspose.com/temporary-license
[25]: https://docs.aspose.com/cells/net/getting-started/
[26]: https://forum.aspose.com/
[27]: https://blog.aspose.com/2020/01/21/create-excel-xls-xlsx-programmatically-in-csharp-net/





