---
title: 'Add Comments in Excel Worksheets using Python'
seoTitle: "Add Comments in Excel using Python | Format Comments in Cells"
description: "Use Python Excel API to add comments to the Excel worksheets using Python. Format the cell comments in Excel worksheets programmatically."
date: Tue, 15 Jun 2021 03:10:00 +0000
draft: false
url: /2021/06/15/add-comments-in-excel-worksheets-using-python/
author: Usman Aziz
summary: 'MS Excel supports adding comments to the cells in the worksheets to provide additional information. In various cases, comments are used to explain a formula. Moreover, MS Excel allows you to define the font size, height, width, etc. of the comments. In this article, you will learn **how to add comments to the Excel worksheets programmatically using Python**.'
tags: ['API to Add Comments in Excel Python', 'Add Comments in an Excel Worksheet Python', 'Apply Formatting to Comments in Excel Python']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Add-Comments-in-Excel.jpg" alt="Add Comments in Excel Worksheet Python">}}


MS Excel supports adding comments to the cells in the worksheets to provide additional information. In various cases, comments are used to explain a formula. Moreover, MS Excel allows you to define the font size, height, width, etc. of the comments. In this article, you will learn **how to add comments to the Excel worksheets programmatically using Python**.

*   [API to Add Comments in Excel][1]
*   [Add Comments in an Excel Worksheet][2]
*   [Apply Formatting to Comments in Excel][3]

## Python API to Add Comments in Excel {#API-to-Add-or-Format-Comments-in-Excel}

In order to add comments to the cells in Excel worksheets, we will use [Aspose.Cells for Python via Java][4]. The API lets you create, modify, and convert Excel files from within your Python applications. You can either [download][5] the API or install it using the following pip command.

*   `pip install aspose-cells`

## Add Comments to an Excel Worksheet in Python {#Add-Comments-in-an-Excel-Worksheet}

The following are the steps to add a comment to a cell in an Excel worksheet using Python.

*   Load the Excel file using [Workbook][6] class.
*   Get reference of the desired [Worksheet][7] using [Workbook.getWorksheets().get(index)][8] method.
*   Add comment to the desired cell using [Worksheet.getComments().add(string cellName)][9] method and get the reference of the comment in a [Comment][10] object.
*   Set comment's note using [Comment.setNote()][11] method.
*   Save the updated Excel file using [Workbook.save(string)][12] method.

The following code sample shows how to add a comment in an Excel worksheet using Python.

{{< gist aspose-com-gists a84c46e782e6befe28d8ab7ee34fbf38 "add-comment-in-worksheet.py" >}}

## Apply Formatting to Comments in Excel {#Apply-Formatting-to-Comments-in-Excel}

The following are the steps to apply formatting to the comments in Excel using Python.

*   Load the Excel file using [Workbook][13] class.
*   Get reference of the desired [Worksheet][14] using [Workbook.getWorksheets().get(index)][15] method.
*   Add comment to the cell using [Worksheet.getComments().add(string cellName)][16] method and get the reference of the comment in a [Comment][17] object.
*   Set comment's note using [Comment.setNote()][18] method.
*   Set desired formatting of the comment using Comment object.
*   Save the updated Excel file using [Workbook.save(string)][19] method.

The following code sample shows how to set the formatting of the comments in Excel.

{{< gist aspose-com-gists a84c46e782e6befe28d8ab7ee34fbf38 "format-comment-in-worksheet.py" >}}

## Get a Free License {#Get-a-Free-License}

You can use Aspose.Cells for Python via Java without evaluation limitations using a [temporary license][20].

## Conclusion

In this article, you have learned how to add comments to the cells in Excel worksheets using Python. Furthermore, you have seen how to apply formatting to the comments programmatically. You can explore other features of the API using the [documentation][21]. In case you would have any queries, feel free to post to our [forum][22].

## See Also

*   [Create Excel Files in Python][23]




[1]: #API-to-Add-or-Format-Comments-in-Excel
[2]: #Add-Comments-in-an-Excel-Worksheet
[3]: #Apply-Formatting-to-Comments-in-Excel
[4]: https://products.aspose.com/cells/python-java
[5]: https://downloads.aspose.com/cells/pythonjava
[6]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[7]: https://apireference.aspose.com/cells/python/asposecells.api/Worksheet
[8]: https://apireference.aspose.com/cells/python/asposecells.api/worksheetcollection#Item%20(java.lang.String)
[9]: https://apireference.aspose.com/cells/python/asposecells.api/commentcollection#add(java.lang.String)
[10]: https://apireference.aspose.com/cells/python/asposecells.api/Comment
[11]: https://apireference.aspose.com/cells/python/asposecells.api/comment#Note
[12]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String)
[13]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[14]: https://apireference.aspose.com/cells/python/asposecells.api/Worksheet
[15]: https://apireference.aspose.com/cells/python/asposecells.api/worksheetcollection#Item%20(java.lang.String)
[16]: https://apireference.aspose.com/cells/python/asposecells.api/commentcollection#add(java.lang.String)
[17]: https://apireference.aspose.com/cells/python/asposecells.api/Comment
[18]: https://apireference.aspose.com/cells/python/asposecells.api/comment#Note
[19]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String)
[20]: https://purchase.aspose.com/temporary-license
[21]: https://docs.aspose.com/cells/pythonjava
[22]: https://forum.aspose.com/
[23]: https://blog.aspose.com/2020/08/19/create-excel-xls-xlsx-using-python-excel-api/





