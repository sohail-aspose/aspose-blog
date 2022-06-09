---
title: 'Add Watermark to Excel Worksheets using C#'
seoTitle: "Add Watermark to Excel Worksheet in C# .NET | .NET Excel API by Aspose"
description: "Use .NET Excel API to add watermark to Excel worksheets using C# or VB.NET. Source code to customize the locking properties of the watermark."
date: Tue, 06 Jul 2021 16:40:00 +0000
draft: false
url: /2021/07/06/add-watermark-to-excel-worksheets-using-csharp/
author: Usman Aziz
summary: 'Watermarks are one of the ways to protect Excel files from being used illegally. Often, a watermark defines the ownership of the copyrighted content. In this article, you will learn about adding watermarks to Excel files programmatically. Particularly, the article will cover **how to add watermark to Excel worksheets using C#**.'
tags: ['Add a Watermark to Excel Worksheet Csharp', 'Csharp API to Add Watermarks to Excel Files', 'Dotnet watermark API for Excel']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Add-Watermark-to-Excel-Sheets.jpg" alt="Add Watermark to Excel Sheet in C#">}}


Watermarks are one of the ways to protect Excel files from being used illegally. Often, a watermark defines the ownership of the copyrighted content. In this article, you will learn about adding watermarks to Excel files programmatically. Particularly, the article will cover **how to add watermark to Excel worksheets using C#**.

*   [C# API to Add Watermarks to Excel Files][1]
*   [Add a Watermark to Excel Worksheet][2]

## C# API to Add Watermarks to Excel Files {#API-to-Add-Watermarks-to-Excel-Files}

In order to add watermark to Excel worksheets, we will use [Aspose.Cells for .NET][3]. It is a powerful yet easy-to-use API that lets you create, modify or convert Excel files. You can either [download][4] the API's DLL or install it via [NuGet][5].

```
PM> Install-Package Aspose.Cells
```

## Add a Watermark to Excel Worksheet in C# {#Add-a-Watermark-to-Excel-Worksheet}

The following are the steps to add a watermark in an Excel worksheet using C#.

*   Load the Excel file using [Workbook][6] class by providing its path.
*   Get reference of the [Worksheet][7] to which you want to add the watermark.
*   Create a watermark by adding a new [Shape][8] to the worksheet and set the its text and properties.
*   Set [Shape.IsLocked][9] property to true to lock the watermark.
*   Set other lock types using [Shape.SetLockedProperty(ShapeLockType, bool)][10] method.
*   Save the updated Excel file using [Workbook.Save(String)][11] method.

The following code sample shows how to add a watermark to an Excel worksheet.

{{< gist aspose-com-gists 92fce9ded784de01a7b6ea77e45334f4 "add-watermark-to-Excel.cs" >}}

### Output

The following is the screenshot of the Excel worksheet after adding the watermark.



{{< figure align=center src="images/Add-Watermark-to-Excel-Worksheet.jpg" alt="Adding Watermark in Excel Worksheet">}}


## Get a Free License {#Get-a-Free-License}

You can use Aspose.Cells for .NET without evaluation limitations using a [temporary license][12].

## Conclusion

In this article, you have learned how to add watermark to Excel worksheets using C#. You can easily integrate the provided code within your .NET, .NET Core, or Xamarin based applications. In addition, you can explore the [documentation][13] of Aspose.Cells for .NET. You can also post your queries on our [forum][14].

## See Also

*   [Create MS Excel Files in C# without MS Office][15]
*   [Convert Excel to PDF in C#][16]




[1]: #API-to-Add-Watermarks-to-Excel-Files
[2]: #Add-a-Watermark-to-Excel-Worksheet
[3]: https://products.aspose.com/cells/net
[4]: https://downloads.aspose.com/cells/net
[5]: https://nuget.org/packages/Aspose.Cells
[6]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[7]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[8]: https://apireference.aspose.com/cells/net/aspose.cells.drawing/shape
[9]: https://apireference.aspose.com/cells/net/aspose.cells.drawing/shape/properties/islocked
[10]: https://apireference.aspose.com/cells/net/aspose.cells.drawing/shape/methods/setlockedproperty
[11]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/2
[12]: https://purchase.aspose.com/temporary-license
[13]: https://docs.aspose.com/cells/net
[14]: https://forum.aspose.com/
[15]: https://blog.aspose.com/2020/01/21/create-excel-xls-xlsx-programmatically-in-csharp-net/
[16]: https://blog.aspose.com/2019/11/29/convert-xls-and-xlsx-to-pdf-in-csharp/





