---
title: 'Read Data in Excel Files using Python'
seoTitle: "Read an Excel File in Python | Read Data from Excel Worksheet in Python"
description: "Use Python Excel library to read an Excel file in XLSX/XLS/CVS and other formats using Python. Read data from a single or all worksheets in Excel file."
date: Thu, 09 Dec 2021 13:24:39 +0000
draft: false
url: /2021/12/09/read-excel-files-using-python/
author: Usman Aziz
summary: 'MS Excel provides a convenient way of keeping and sharing data in the form of rows and columns. More often, Excel files are used to store huge datasets having hundreds and thousands of records. While working with Excel files in Python, you may need to read data from each cell in the worksheets. To achieve that, this article shows **how to read an Excel file in Python**. You will learn how to read data from a single worksheet or all the worksheets in an Excel workbook.'
tags: ['read data from excel files in python', 'read excel file in python', 'read spreadsheet data in python', 'read xls file in python', 'read xlsx file in python']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Excel-File.jpg" alt="Read data in Excel files using Python">}}


MS Excel provides a convenient way of keeping and sharing data in the form of rows and columns. More often, Excel files are used to store huge datasets having hundreds and thousands of records. While working with Excel files in Python, you may need to read data from each cell in the worksheets. To achieve that, this article shows **how to read an Excel file in Python**. You will learn how to read data from a single worksheet or all the worksheets in an Excel workbook.

*   [Python Library to Read Excel Files][1]
*   [Read Data from an Excel File][2]
*   [Read a Worksheet in an Excel Workbook][3]

## Python Library to Read Excel Files {#Python-Library-to-Read-Excel-Files}

To read data from the workbooks, we will use [Aspose.Cells for Python via Java][4]. It is a powerful and feature-rich Python library to create MS Excel files. Moreover, it allows you to read and manipulate existing Excel files seamlessly. You can [download][5] the library or install it using the following pip command.

```
pip install aspose-cells
```

## Read an Excel File in Python {#Read-Data-from-an-Excel-File}

Before we start reading the data, let's have an overview of how the data is managed in an Excel file. An Excel file is termed as workbook that acts as a container. Each workbook contains one or more worksheets and every worksheet is composed of a number of cells. These cells are uniquely identified by the rows and columns. So, in order to read data from a cell, you need to know its row and column index.

The following are the steps to read an Excel file and print its data in Python.

*   Load the Excel file using [Workbook][6] class.
*   Get reference of the [WorksheetCollection][7] using [Workbook.getWorksheets()][8] method.
*   Loop through worksheets in the collection and in each iteration, perform following steps:
    *   Get reference of the worksheet in an object.
    *   Get count of data rows and columns in the worksheet.
    *   Start a loop for rows.
    *   Start a nested loop for columns.
    *   Read data from each cell using [Worksheet.getCells().get(rowIndex, columnIndex).getValue()][9] method.

The following code sample shows how to read an Excel file in Python.

{{< gist aspose-com-gists 149106ad8c13c30e1d7c386917442147 "read-excel-file.py" >}}

The following is the output we get after running the code sample above.



{{< figure align=center src="images/Read-Excel-Files.jpg" alt="Reading data in the worksheets of Excel file in Python" caption="Reading an Excel File in Python">}}


## Read a Particular Worksheet in Excel in Python {#Read-a-Worksheet-in-an-Excel-Workbook}

You can also read a particular worksheet in the Excel file by following the steps below.

*   Load the Excel file using [Workbook][10] class.
*   Get reference of desired worksheet using [Workbook.getWorksheets().get(index)][11] method.
*   Get count of data rows and columns in the worksheet.
*   Start a loop for rows.
*   Start a nested loop for columns.
*   Read data from each cell using [Worksheet.getCells().get(rowIndex, columnIndex).getValue()][12] method.

The following code sample shows how to read data from a particular worksheet in Python.

{{< gist aspose-com-gists 149106ad8c13c30e1d7c386917442147 "read-worksheet.py" >}}

## Get a Free API License

You can use Aspose.Cells for Python via Java without evaluation limitations by requesting a [free temporary license][13].

## Conclusion

In this article, you have learned how to read Excel files in Python. Moreover, you have seen how to read data from a particular worksheet or all the worksheets in an Excel workbook. You can explore more about the Python spreadsheet library using the [documentation][14]. In case you would have any questions or queries, feel free to let us know via our [forum][15].

## See Also

*   [Create MS Excel Files using Python][16]
*   [Convert Excel to PDF in Python][17]




[1]: #Python-Library-to-Read-Excel-Files
[2]: #Read-Data-from-an-Excel-File
[3]: #Read-a-Worksheet-in-an-Excel-Workbook
[4]: https://products.aspose.com/cells/python-java
[5]: https://downloads.aspose.com/cells/python
[6]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[7]: https://apireference.aspose.com/cells/python/asposecells.api/WorksheetCollection
[8]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#Worksheets
[9]: https://apireference.aspose.com/cells/python/asposecells.api/cell#Value
[10]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[11]: https://apireference.aspose.com/cells/python/asposecells.api/worksheetcollection#Item%20(int)
[12]: https://apireference.aspose.com/cells/python/asposecells.api/cell#Value
[13]: https://purchase.aspose.com/temporary-license
[14]: https://docs.aspose.com/cells/pythonjava/
[15]: https://forum.aspose.com/
[16]: https://blog.aspose.com/2020/08/19/create-excel-xls-xlsx-using-python-excel-api/
[17]: https://blog.aspose.com/2021/04/02/convert-excel-files-to-pdf-in-python/




