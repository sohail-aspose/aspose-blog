---
title: 'Add Comments in Excel Worksheets using C#'
seoTitle: "Add Comments in Excel using C# .NET | Format Comments in Excel"
description: "Use .NET Excel API to add comments to the Excel worksheets using C# or VB.NET. Add image to the comment and format comments programmatically."
date: Mon, 12 Jul 2021 11:02:00 +0000
draft: false
url: /2021/07/12/add-comments-in-excel-using-csharp/
author: Usman Aziz
summary: 'Comments in Excel worksheets are used to add additional information or to explain a formula. These comments can be formatted as well by defining the font size, height, width, etc. In this article, you will learn **how to add comments to the Excel worksheets using C#**. Furthermore, the article will also demonstrate how to apply formatting and add images to the comments programmatically.'
tags: ['Add Comments in an Excel Worksheet csharp', 'Add Image to a Comment in Excel csharp', 'Apply Formatting to Comments in Excel csharp']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Add-Comments-in-Excel.jpg" alt="Add Comments in Excel Worksheet C#">}}


Comments in Excel worksheets are used to add additional information or to explain a formula. These comments can be formatted as well by defining the font size, height, width, etc. In this article, you will learn **how to add comments to the Excel worksheets using C#**. Furthermore, the article will also demonstrate how to apply formatting and add images to the comments programmatically.

*   [C# API to Add Comments in Excel][1]
*   [Add Comments in an Excel Worksheet][2]
*   [Add Image to a Comment in Excel][3]
*   [Apply Formatting to Comments in Excel][4]

## C# API to Add Comments in Excel {#API-to-Add-or-Format-Comments-in-Excel}

In order to add comments in Excel worksheets, we will use [Aspose.Cells for .NET][5]. It is a powerful spreadsheet manipulation API that lets you create Excel files from scratch. Also, it supports modifying and converting existing Excel files seamlessly. You can either [download][6] the API or install it using [NuGet][7].

```
PM> Install-Package Aspose.Cells
```

## Add Comments to an Excel Worksheet in C# {#Add-Comments-in-an-Excel-Worksheet}

The following are the steps to add comments to an Excel worksheet in C#.

*   Load the Excel file using [Workbook][8] class.
*   Get reference of the desired [Worksheet][9] from [Workbook.Worksheets][10] collection.
*   Add comment to the worksheet using [Worksheet.Comments.Add(string)][11] method and get the reference of the comment in a [Comment][12] object.
*   Set comment's note using [Comment.Note][13] property.
*   Save the updated Excel file using [Workbook.Save(string)][14] method.

The following code sample shows how to add a comment in an Excel worksheet using C#.

{{< gist aspose-com-gists 369691c88694c34fdc36b4db051cc2d1 "add-comment-in-worksheet.cs" >}}

## Add Image to a Comment in Excel using C# {#Add-Image-to-a-Comment-in-Excel}

You can also add an image to the comment in the Excel worksheet following the below steps.

*   Load the Excel file using [Workbook][15] class.
*   Get reference of the [CommentCollection][16] in the desired worksheet using [Workbook.Worksheets\[index\].Comments][17] property.
*   Add a new comment to the collection and get its reference in [Comment][18] object.
*   Set comment's note using [Comment.Note][19] property.
*   Load the image from file into a _Bitmap_ object.
*   Save the Bitmap into a _MemoryStream_ object.
*   Add image to the comment using [Comment.CommentShape.Fill.ImageData][20] property.
*   Save the updated Excel file using [Workbook.Save(string)][21] method.

The following code sample shows how to add image to a comment in Excel using C#.

{{< gist aspose-com-gists 369691c88694c34fdc36b4db051cc2d1 "add-image-to-comment.cs" >}}

## Apply Formatting to Comments in Excel using C# {#Apply-Formatting-to-Comments-in-Excel}

The following are the steps to apply formatting to the comments in Excel using C#.

*   Load the Excel file using [Workbook][22] class.
*   Get reference of the desired [Worksheet][23] from [Workbook.Worksheets][24] collection.
*   Add comment to the worksheet using [Worksheet.Comments.Add(string)][25] method and get the reference of the comment in a [Comment][26] object.
*   Set comment's note using [Comment.Note][27] property.
*   Set the desired formatting options of the comment.
*   Save the updated Excel file using [Workbook.Save(string)][28] method.

The following code sample shows how to set formatting of the comments in Excel using C#.

{{< gist aspose-com-gists 369691c88694c34fdc36b4db051cc2d1 "format-comment-in-worksheet.cs" >}}

## Get a Free License {#Get-a-Free-License}

You can use Aspose.Cells for .NET without evaluation limitations using a [temporary license][29].

## Conclusion

In this article, you have learned how to add comments to Excel worksheets using C#. Furthermore, you have seen how to add image to a comment programmatically. You can easily integrate the provided code within your .NET, .NET Core, or Xamarin based applications. In addition, you can explore the [documentation][30] of Aspose.Cells for .NET. In case you would have any queries, feel free to post to our [forum][31].

## See Also

*   [Create MS Excel Files in C# without MS Office][32]
*   [Convert Excel to PDF in C#][33]




[1]: #API-to-Add-or-Format-Comments-in-Excel
[2]: #Add-Comments-in-an-Excel-Worksheet
[3]: #Add-Image-to-a-Comment-in-Excel
[4]: #Apply-Formatting-to-Comments-in-Excel
[5]: https://products.aspose.com/cells/net
[6]: https://downloads.aspose.com/cells/net
[7]: https://nuget.org/packages/Aspose.Cells
[8]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[9]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[10]: https://apireference.aspose.com/cells/net/aspose.cells/workbook/properties/worksheets
[11]: https://apireference.aspose.com/cells/net/aspose.cells.commentcollection/add/methods/1
[12]: https://apireference.aspose.com/cells/net/aspose.cells/comment
[13]: https://apireference.aspose.com/cells/net/aspose.cells/comment/properties/note
[14]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/2
[15]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[16]: https://apireference.aspose.com/cells/net/aspose.cells/commentcollection
[17]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet/properties/comments
[18]: https://apireference.aspose.com/cells/net/aspose.cells/comment
[19]: https://apireference.aspose.com/cells/net/aspose.cells/comment/properties/note
[20]: https://apireference.aspose.com/cells/net/aspose.cells.drawing/fillformat/properties/imagedata
[21]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/2
[22]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[23]: https://apireference.aspose.com/cells/net/aspose.cells/worksheet
[24]: https://apireference.aspose.com/cells/net/aspose.cells/workbook/properties/worksheets
[25]: https://apireference.aspose.com/cells/net/aspose.cells.commentcollection/add/methods/1
[26]: https://apireference.aspose.com/cells/net/aspose.cells/comment
[27]: https://apireference.aspose.com/cells/net/aspose.cells/comment/properties/note
[28]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/2
[29]: https://purchase.aspose.com/temporary-license
[30]: https://docs.aspose.com/cells/net
[31]: https://forum.aspose.com/
[32]: https://blog.aspose.com/2020/01/21/create-excel-xls-xlsx-programmatically-in-csharp-net/
[33]: https://blog.aspose.com/2019/11/29/convert-xls-and-xlsx-to-pdf-in-csharp/





