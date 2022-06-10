---
title: 'Convert MS Excel Files to HTML using Python'
seoTitle: "Convert Excel File to HTML in Python | XLS/XLSX to HTML using Python"
description: "Use Python Excel to HTML converter API to convert MS Excel XLS/XLSX files to HTML using Python. High quality Excel to HTML conversion with worksheet tabs."
date: Fri, 21 Aug 2020 08:50:04 +0000
draft: false
url: /2020/08/21/convert-ms-excel-files-to-html-using-python/
author: Usman Aziz
summary: ''
tags: ['convert Excel to HTML using python', 'convert xls to html using python', 'convert xlsx to html using python']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Excel-to-HTML-Logo.jpg" alt="Excel to HTML Python">}}


MS Excel files are very much in business for storing, organizing, and analyzing a large amount of data. In certain cases, developers also prefer to use Excel files instead of a database to keep the records. However, in order to view the data in Excel files, you need to install MS Excel. Furthermore, you can not view the content of the Excel files from within your applications. **Excel to HTML** conversion is one of the possible solutions in such cases. This article aims to provide you the ways of **how to convert Excel spreadsheets to HTML files using Python**.

*   [Python Excel to HTML Converter][1]
*   [Convert Excel Files to HTML using Python][2]
*   [Convert Excel Files to HTML having Tooltips][3]

## Python Excel to HTML Converter API {#Python-Excel-to-HTML-Converter}

[Aspose.Cells for Python via Java][4] is a powerful spreadsheet API that lets you create and manipulate Excel files quite easily using Python. The API's builtin Excel to HTML converter provides high-quality conversion of Excel workbooks to HTML files. Furthermore, it renders tabs to navigate between sheets within the HTML file. You can run the following pip command in order to install and use the API in Python applications.

*   `pip install aspose-cells`

## Convert Excel Files to HTML using Python {#Convert-Excel-Files-to-HTML-using-Python}

Converting XLS/XLSX files to HTML using Aspose.Cells is as easy as pie and can be done in a couple of lines of code. The following are the steps to convert an XLSX file to HTML using Python.

*   Create an object of [Workbook][5] class to load the Excel file.
*   Save Excel file as HTML using [Workbook.save(fileName)][6] method.

The following code sample shows how to convert an XLSX file to HTML using Python.

{{< gist aspose-com-gists 2f9ef0f14351208cb913d9bf4ebec551 "excel-to-html.py" >}}

### Excel to HTML



{{< figure align=center src="images/Excel-to-HTML.jpg" alt="convert Excel to HTML in Python">}}


## Convert Excel File to HTML having Tooltips using Python {#Convert-Excel-File-to-HTML-with-Tooltip-using-Python}

You can also configure the API to add tooltip text in the converted HTML file. This feature is used when the text's length exceeds the width of the cell in the worksheet and a part of the text may become hidden. For this, the API exposes the [HtmlSaveOptions][7] class. The following are the steps to enable tooltips in Excel to HTML conversion.

*   Load the Excel file using [Workbook][8] class.
*   Create an object of the [HtmlSaveOptions][9] class.
*   Enable tooltip using [HtmlSaveOptions.setAddTooltipText(True)][10] method.
*   Convert Excel to HTML using [Workbook.save(fileName, HtmlSaveOptions)][11] method.

The following code sample shows how to convert XLSX file to HTML having tooltip using Python.

{{< gist aspose-com-gists 2f9ef0f14351208cb913d9bf4ebec551 "excel-to-html-tooltip.py" >}}

## Conclusion

In this article, you have seen how to convert Excel files to HTML using Python. Furthermore, you have learned how to enable tooltips in the converted HTML files programmatically. In order to learn more about Aspose's Python Excel API, please visit the [documentation][12].

## See Also

*   [Create Excel Files using Python][13]




[1]: #Python-Excel-to-HTML-Converter
[2]: #Convert-Excel-Files-to-HTML-using-Python
[3]: #Convert-Excel-File-to-HTML-with-Tooltip-using-Python
[4]: https://products.aspose.com/cells/python-java/
[5]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[6]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String)
[7]: https://apireference.aspose.com/cells/python/asposecells.api/HtmlSaveOptions
[8]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[9]: https://apireference.aspose.com/cells/python/asposecells.api/HtmlSaveOptions
[10]: https://apireference.aspose.com/cells/python/asposecells.api/htmlsaveoptions#AddTooltipText
[11]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String,%20com.aspose.cells.SaveOptions)
[12]: https://docs.aspose.com/cells/pythonjava/
[13]: https://blog.aspose.com/2020/08/19/create-excel-xls-xlsx-using-python-excel-api/





