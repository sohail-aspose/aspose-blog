---
title: 'Find and Replace Text in Excel using Python'
seoTitle: "Find and Replace Text in Excel in Python | Search Text using Regex"
description: "Use Python spreadsheet API to find and replace text in Excel files in Python. Search text in XLSX or XLS files using plain text or regular expression."
date: Thu, 03 Jun 2021 04:44:19 +0000
draft: false
url: /2021/06/03/find-and-replace-text-in-excel-using-python/
author: Usman Aziz
summary: 'Excel spreadsheets often contain thousands of records in multiple sheets. In such cases, finding and replacing a particular text manually could be a hectic task. Therefore, MS Excel provides the find and replace option to update the desired text with a single click. In this article, you will learn **how to find and replace text in Excel files programmatically in Python**.'
tags: ['Find and Replace Text in Excel using regex', 'Find and replace text in Excel file', 'Python API to Find and Replace Text in Excel Files']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Find-and-Replace-Text-in-Excel.png" alt="Find and Replace Text in Excel Python">}}


Excel spreadsheets often contain thousands of records in multiple sheets. In such cases, finding and replacing a particular text manually could be a hectic task. Therefore, MS Excel provides the find and replace option to update the desired text with a single click. In this article, you will learn **how to find and replace text in Excel files programmatically in Python**.

*   [Python API to Find and Replace Text in Excel Files][1]
*   [Find and Replace Text in Excel File][2]
*   [Find and Replace Text in Excel using Regex][3]

## Python API to Find and Replace Text in Excel {#Python-API-to-Find-and-Replace-Text-in-Excel-Files}

[Aspose.Cells for Python via Java][4] is a powerful spreadsheet manipulation API that lets you create new and process existing Excel documents. The Excel automation features provided by the API also include finding and replacing the text seamlessly. You can install the API using the following pip command.

*   `pip install aspose-cells`

## Find and Replace Text in Excel {#Find-and-Replace-Text-in-Excel-File}

The following are the steps to find and replace text in Excel files.

*   Load the Excel file using the [Workbook][5] class.
*   Create an object of [ReplaceOptions][6] class and set options such as case sensitivity and content matching.
*   Replace the text in Excel workbook using [Workbook.replace(searchTerm, replaceTerm, ReplaceOptions)][7] method.
*   Save the updated Excel file using [Workbook.save(fileName)][8] method.

The following code sample shows how to find and replace text in Excel using Python.

{{< gist aspose-com-gists 68b5573d0ce309f0565840916804e78a "find-replace-text-in-Excel.py" >}}

## Find and Replace Text in Excel using Regex {#Find-and-Replace-Text-using-Regular-Expression}

You can also find and replace text in an Excel file that matches a particular pattern. The following steps show how to use a regular expression to find and replace text in an Excel file.

*   Load the Excel file using the [Workbook][9] class.
*   Create an object of [ReplaceOptions][10] class and set options such as case sensitivity and content matching.
*   Indicate that the search term is a regular expression using [ReplaceOptions.setRegexKey(True)][11] method.
*   Replace the text in Excel workbook using [Workbook.replace(searchTerm, replaceTerm, ReplaceOptions)][12] method.
*   Save the updated Excel file using [Workbook.save(fileName)][13] method.

The following Python code sample shows how to search and replace text in Excel using regular expression.

{{< gist aspose-com-gists 68b5573d0ce309f0565840916804e78a "find-replace-text-in-Excel-regex.py" >}}

## Get a Free API License

You can use the API without evaluation limitations by requesting a [free temporary license][14].

## Conclusion

In this article, you have learned how to find and replace text in Excel files using Python. Furthermore, you have seen how to search text that matches a particular pattern in the Excel files. You can explore more about the Python spreadsheet API using the [documentation][15]. In case you would have any questions or queries, feel free to let us know via our [forum][16].

## See Also

*   [Create MS Excel Files using Python][17]
*   [Convert Excel to PDF in Python][18]




[1]: #Python-API-to-Find-and-Replace-Text-in-Excel-Files
[2]: #Find-and-Replace-Text-in-Excel-File
[3]: #Find-and-Replace-Text-using-Regular-Expression
[4]: https://products.aspose.com/cells/python-java
[5]: https://apireference.aspose.com/cells/python/asposecells.api/workbook
[6]: https://apireference.aspose.com/cells/python/asposecells.api/ReplaceOptions
[7]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#replace(java.lang.String,%20java.lang.String,%20com.aspose.cells.ReplaceOptions)
[8]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String)
[9]: https://apireference.aspose.com/cells/python/asposecells.api/workbook
[10]: https://apireference.aspose.com/cells/python/asposecells.api/ReplaceOptions
[11]: https://apireference.aspose.com/cells/python/asposecells.api/replaceoptions#RegexKey
[12]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#replace(java.lang.String,%20java.lang.String,%20com.aspose.cells.ReplaceOptions)
[13]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String)
[14]: https://purchase.aspose.com/temporary-license
[15]: https://docs.aspose.com/cells/pythonjava/
[16]: https://forum.aspose.com/
[17]: https://blog.aspose.com/2020/08/19/create-excel-xls-xlsx-using-python-excel-api/
[18]: https://blog.aspose.com/2021/04/02/convert-excel-files-to-pdf-in-python/





