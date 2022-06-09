---
title: 'How to Insert and Delete Rows and Columns in Excel in Python'
seoTitle: "Python: How to Insert or Delete Rows and Columns in Excel | Python Lib"
description: "Use Python Excel API to insert or delete rows and columns in Excel XLSX XLS using Python. Insert or delete single or multiple rows or columns."
date: Tue, 13 Apr 2021 11:50:00 +0000
draft: false
url: /2021/04/13/insert-and-delete-rows-and-columns-in-excel-using-python/
author: Usman Aziz
summary: 'While working with spreadsheet manipulation, you may often need to insert or delete rows and columns within your worksheets. In accordance with that, this article covers how to manipulate rows and columns in worksheets programmatically. Particularly, you will learn **how to insert or delete single or multiple rows and columns in an Excel worksheet using Python**.'
tags: ['Delete Columns in Excel using Python', 'Delete Rows in Excel using Python', 'Insert Columns in Excel using Python', 'Insert Rows in Worksheet using Python', 'Python API to Manipulate Excel Files']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Create-Excel-Files-in-Python.jpg" alt="Insert remove rows or columns in Excel in Python">}}


While working with spreadsheet manipulation, you may often need to insert or delete rows and columns within your worksheets. In accordance with that, this article covers how to manipulate rows and columns in worksheets programmatically. Particularly, you will learn **how to insert or delete rows and columns in an Excel worksheet in Python**.

*   [Python API to Insert or Delete Rows and Columns in Excel][1]
*   [Insert Rows in a Worksheet using Python][2]
*   [Insert Columns in Excel Worksheet using Python][3]
*   [Delete Rows in Excel Worksheet using Python][4]
*   [Delete Columns in Excel Worksheet using Python][5]
*   [Get a Free API License][6]

## Python Library to Insert or Delete Excel Rows and Columns {#Python-API-to-Manipulate-Excel-Files}

In order to insert or delete rows and columns in XLSX/XLS worksheets, we'll use [Aspose.Cells for Python via Java][7] API. It is a powerful spreadsheet manipulation API that provides a wide range of features for Excel automation. You can install the API using the following pip command.

*   `pip install aspose-cells`

## How to Insert Rows in Excel using Python {#Insert-Rows-in-Worksheet-using-Python}

The following are the steps to insert rows in an Excel worksheet in Python.

*   First, load the Excel file using the [Workbook][8] class.
*   Access the desired worksheet by index using [Workbook.getWorksheets().get(index)][9] method.
*   Insert rows using [Worksheet.getCells().insertRows(rowIndex, totalRows)][10] method in which the first parameter is the row index and the second parameter is the number of rows you want to insert.
*   Finally, save the updated file using [Workbook.save(string)][11] method.

The following code sample shows how to insert rows in an Excel worksheet using Python.

{{< gist aspose-com-gists db8bf666a8cfa3faf857e1ad608149f3 "insert-row.py" >}}

## How to Insert Columns in Excel in Python {#Insert-Columns-in-Excel-using-Python}

The following are the steps to insert columns in Excel worksheet using Python.

*   First, load the Excel file using the [Workbook][12] class.
*   Access the desired worksheet by index using [Workbook.getWorksheets().get(index)][13] method.
*   Insert columns using [Worksheet.getCells().insertColumns(columnIndex, totalColumns)][14] method in which the first parameter is the column index and the second parameter is the number of columns you want to insert.
*   Finally, save the updated file using [Workbook.save(string)][15] method.

The following code sample shows how to insert columns in an Excel worksheet using Python.

{{< gist aspose-com-gists db8bf666a8cfa3faf857e1ad608149f3 "insert-column.py" >}}

## Delete Rows in an Excel XLSX in Python {#Delete-Rows-in-Excel-using-Python}

The following are the steps to delete rows from an Excel worksheet using Python.

*   First, load the Excel file using the [Workbook][16] class.
*   Access the desired worksheet by index using [Workbook.getWorksheets().get(index)][17] method.
*   Delete rows using [Worksheet.getCells().deleteRows(rowIndex, totalRows)][18] method in which the first parameter is the row index and the second parameter is the number of rows you want to delete.
*   Finally, save the updated file using [Workbook.save(string)][19] method.

The following code sample shows how to delete rows from an Excel worksheet in Python.

{{< gist aspose-com-gists db8bf666a8cfa3faf857e1ad608149f3 "delete-row.py" >}}

## Delete Columns in Excel XLSX in Python {#Delete-Columns-in-Excel-using-Python}

The following are the steps to delete columns from an Excel worksheet using Python.

*   First, load the Excel file using the [Workbook][20] class.
*   Access the desired worksheet by index using [Workbook.getWorksheets().get(index)][21] method.
*   Delete columns using [Worksheet.getCells().insertColumns(columnIndex, totalColumns, updateReference)][22] method. The first parameter is the column index, the second parameter is the number of columns you want to delete and the third parameter indicates if references need to be updated in other worksheets.
*   Finally, save the updated file using [Workbook.save(string)][23] method.

The following code sample shows how to delete columns from an Excel worksheet using Python.

{{< gist aspose-com-gists db8bf666a8cfa3faf857e1ad608149f3 "delete-column.py" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [get a free temporary license][24] in order to use the API without evaluation limitations.

## Conclusion

In this article, you have learned how to work with rows and columns in Excel. Particularly, you have seen how to insert or delete rows and columns in Excel worksheets using Python. In addition, you can explore more about the Python Excel API using the [documentation][25]. Furthermore, you can share your queries with us via our [forum][26].

## See Also

*   [Create MS Excel Files using Python – Python Excel API][27]




[1]: #Python-API-to-Manipulate-Excel-Files
[2]: #Insert-Rows-in-Worksheet-using-Python
[3]: #Insert-Columns-in-Excel-using-Python
[4]: #Delete-Rows-in-Excel-using-Python
[5]: #Delete-Columns-in-Excel-using-Python
[6]: #Get-a-Free-API-License
[7]: https://products.aspose.com/cells/python-java/
[8]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[9]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#Worksheets
[10]: https://apireference.aspose.com/cells/python/asposecells.api/cells#insertRows(int,%20int)
[11]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String)
[12]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[13]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#Worksheets
[14]: https://apireference.aspose.com/cells/python/asposecells.api/cells#insertColumns(int,%20int)
[15]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String)
[16]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[17]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#Worksheets
[18]: https://apireference.aspose.com/cells/python/asposecells.api/cells#deleteRows(int,%20int)
[19]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String)
[20]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[21]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#Worksheets
[22]: https://apireference.aspose.com/cells/python/asposecells.api/cells#deleteColumns(int,%20int,%20boolean)
[23]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String)
[24]: https://purchase.aspose.com/temporary-license
[25]: https://docs.aspose.com/cells/pythonjava/
[26]: https://forum.aspose.com/
[27]: https://blog.aspose.com/2020/08/19/create-excel-xls-xlsx-using-python-excel-api/





