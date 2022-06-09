---
title: 'Split Text to Multiple Columns in Excel using Python'
seoTitle: "Python: Split Text to Column in Excel | Split Column into Multiple Columns"
description: "Use Python Excel API to split text to column in Excel using Python. Split text in one column into multiple columns programmatically in Python."
date: Thu, 24 Jun 2021 09:36:03 +0000
draft: false
url: /2021/06/24/split-text-to-column-in-excel-using-python/
author: Usman Aziz
summary: 'In various cases, you may need to split text in a column into multiple columns in an Excel worksheet. The splitting criteria could be a blank space, a comma, a special character, etc. In this article, you will learn **how to split a text into columns in an Excel worksheet using Python**. It automates the **Text to Columns feature of MS Excel**.'
tags: ['Excel Text to Column in Python', 'Python Text to Column in Excel', 'Split Text to Columns in Excel using Python']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Text-to-Column-Python.jpg" alt="Excel Text to Column Python">}}


In various cases, you may need to split text in a column into multiple columns in an Excel worksheet. The splitting criteria could be a blank space, a comma, a special character, etc. In this article, you will learn **how to split a text into columns in an Excel worksheet using Python**. It automates the **Text to Columns feature of MS Excel**.

*   [Python API for Excel's Text to Columns][1]
*   [Split Text to Columns in Excel using Python][2]

## Python API for Excel's Text to Columns {#Python-API-for-Excel-Text-to-Column}

In order to split text in one column into multiple columns in an Excel worksheet, we'll use [Aspose.Cells for Python via Java][3]. It is a powerful and feature-rich API that lets you create, modify and convert Excel files using Python. You can install the API using the following pip command.

*   `pip install aspose-cells`

## Split Text to Columns in Excel using Python {#Split-Text-to-Columns-in-Excel-using-Python}

The following are the steps to split text to columns in Excel using Python.

*   First, load the Excel file using the [Workbook][4] class.
*   Get the reference to the worksheet where you want to split the text.
*   Add values to the cells (optional).
*   Create an instance of [TxtLoadOptions][5] class and specify the splitting character using [TxtLoadOptions.setSeparator(value)][6] method.
*   Split text to column using [Worksheet.getCells().textToColumns(int row, int column, int totalRows, TxtLoadOptions options)][7] method.
*   Finally, save the Excel file using [Workbook.save(fileName, SaveFormat.XLSX)][8] method.

The following code sample shows how to perform Excel's text to columns operation in Python.

{{< gist aspose-com-gists 60527a892deb091dd4dc7ddf14b55bf0 "text-to-column.py" >}}

### Output



{{< figure align=center src="images/Text-to-Column-in-Excel.jpg" alt="Excel Text to Column Python">}}


## Get a Free API License {#Get-a-Free-API-License}

You can [get a temporary license][9] in order to use the API without evaluation limitations.

## Conclusion

In this article, you have learned how to split text to columns in Excel using Python. More precisely, you have seen how to split the text in a column into multiple columns in Excel using Python. You can explore more about Aspose.Cells for Python via Java using the [documentation][10]. In case you would have any queries, contact us via our [forum][11].

## See Also

*   [Create MS Excel Files using Python – Python Excel API][12]




[1]: #Python-API-for-Excel-Text-to-Column
[2]: #Split-Text-to-Columns-in-Excel-using-Python
[3]: https://products.aspose.com/cells/python-java/
[4]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[5]: https://apireference.aspose.com/cells/python/asposecells.api/TxtLoadOptions
[6]: https://apireference.aspose.com/cells/python/asposecells.api/txtloadoptions#Separator
[7]: https://apireference.aspose.com/cells/python/asposecells.api/cells#textToColumns(int,%20int,%20int,%20com.aspose.cells.TxtLoadOptions)
[8]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String,%20int)
[9]: https://purchase.aspose.com/temporary-license
[10]: https://docs.aspose.com/cells/pythonjava/
[11]: https://forum.aspose.com/
[12]: https://blog.aspose.com/2020/08/19/create-excel-xls-xlsx-using-python-excel-api/





