---
title: 'Create MS Excel Files using Python - Python Excel API'
seoTitle: ""
description: ""
date: Wed, 19 Aug 2020 17:05:25 +0000
draft: false
url: /2020/08/19/create-excel-xls-xlsx-using-python-excel-api/
author: Usman Aziz
summary: ''
tags: ['create chart in excel in python', 'create excel file in python', 'create pivot table in excel in python', 'create xlsx in python', 'update excel file in python']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Create-Excel-Files-in-Python.jpg" alt="Create Excel Files in Python">}}


[Python][1] has become one of the ruling programming languages in the past few years. The usefulness and popularity of Python have immensely grown the community of Python enthusiasts. On the other hand, spreadsheet automation has made it easier to keep, organize, and play with a large amount of data from within the web or desktop applications. This article aims to put together Python and spreadsheet automation to show you **how to create Excel XSLX or XLS files using Python**. Furthermore, you will learn how to insert data, images, charts, and tables in an Excel worksheet programmatically using Python.

*   [Python API to Create Excel Files][2]
*   [Create Excel XLS/XLSX Files using Python][3]
*   [Insert Data into Existing Excel File using Python][4]
*   [Create Excel File having Images using Python][5]
*   [Generate Charts within Excel Worksheet using Python][6]
*   [Create Pivot Tables in Excel Worksheet using Python][7]
*   [Use Aspose.Cells for Free][8]

**Info**: Aspose provides other Python APIs (for example, [Aspose.Slides for Python via .NET][9] for working with PowerPoint and presentations in other formats) and free online tools for viewing, editing, merging, and converting documents (for example, the [PPT to JPG converter][10].

## Python API to Create Excel XLSX/XLS Files - Free Download {#Python-Excel-API}

[Aspose.Cells for Python via Java][11] is a powerful yet easy to use spreadsheet manipulation API that lets you implement spreadsheet automation within your applications using Python. You can create new Excel files as well as update and convert existing spreadsheet documents in a few lines of code. In order to integrate and use Aspose.Cells for Python via Java, execute the following pip command.

*   `pip install aspose-cells`

You can also download the API's package from the [downloads][12] section.

## Create Excel XLSX/XLS Files using Python {#Create-Excel-XLS-XLSX-Files-using-Python}

Let's start by creating a simple Excel XLSX file using Aspose.Cells for Python via Java. The following are the steps to do this:

*   Create a new object of [Workbook][13] class.
*   Access the desired [Worksheet][14] in the workbook using [Workbook.getWorksheets().get(index)][15] method.
*   Put value in the desired cell using [Worksheet.getCells().get("A1").putValue()][16] method.
*   Save the workbook as _.xlsx_ file using [Workbook.save()][17] method.

The following code sample shows how to create an Excel XLSX file using Python.

{{< gist aspose-com-gists f16dc7586917c051564eaebbb159c63f "create-excel-file.py" >}}

### Output



{{< figure align=center src="images/Create-Excel-Worksheet.jpg" alt="create excel file using python">}}


## Python Code to Insert Data into an Excel File {#Insert-Data-into-Existing-Excel-File-using-Python}

In the previous example, you have created a new Excel XLSX file from scratch. However, there might be the case when you need to update the content of an existing Excel file. In this case, you can load the Excel file by providing its path to the [Workbook][18] constructor. The rest of the methods for accessing the worksheets and cells will remain the same.

The following code sample shows how to update an Excel file using Python.

{{< gist aspose-com-gists f16dc7586917c051564eaebbb159c63f "update-excel-file.py" >}}

### Output



{{< figure align=center src="images/update-excel-file-in-python.jpg" alt="update excel file in python">}}


## Create Excel File having Images using Python {#Create-Excel-File-having-Images-using-Python}

In both of the previous examples, you have seen how to insert or update text in the cells of Excel worksheets. Let's now check out how to insert an image into the worksheet using Python.

*   Create a new Excel workbook or load an existing one using [Workbook][19] class.
*   Access the worksheet in which you want to insert the image using [Worksheet][20] class.
*   Insert image using [Worksheet.getPictures().add(upperLeftRow, upperLeftColumn, fileName)][21] method.
*   Save the workbook as _.xlsx_ file using [Workbook.save(fileName)][22] method.

The following code sample shows how to create an Excel file and insert an image using Python.

{{< gist aspose-com-gists f16dc7586917c051564eaebbb159c63f "create-excel-file-with-image.py" >}}

### Output



{{< figure align=center src="images/insert-image-in-excel-using-python.jpg" alt="insert image in excel using python">}}


## Generate Charts within Excel Worksheet using Python {#Generate-Charts-within-Excel-Worksheet-using-Python}

Charts in Excel worksheets are used to visually represent the data in the form of histograms, pyramids, bars, doughnuts and etc. Aspose.Cells for Python via Java supports a multitude of chart types that are listed [here][23]. The following are the steps to generate a chart within an Excel worksheet.

*   Create a new Excel workbook or load an existing one using [Workbook][24] class.
*   Access the desired worksheet and add values in the cells (optional if the worksheet already contains data).
*   Get charts collection using [Worksheet.getCharts()][25] method.
*   Add a new chart in the charts collection using [Worksheet.getCharts().add(type, upperLeftRow, upperLeftColumn, lowerRightRow, lowerRightColumn)][26] method.
*   Define the range of the cells to set NSeries for the chart.
*   Create the Excel _.xlsx_ file using [Workbook.save(fileName)][27] method.

The following code sample shows how to generate charts in an Excel worksheet using Python.

{{< gist aspose-com-gists f16dc7586917c051564eaebbb159c63f "create-excel-file-with-chart.py" >}}

### Output



{{< figure align=center src="images/Create-Chart-in-Excel.jpg" alt="create chart in excel using python">}}


## Create Pivot Tables in Excel Worksheet using Python {#Create-Pivot-Tables-in-Excel-Worksheet-using-Python}

Pivot tables in Excel are created to summarize a large amount of data within the worksheets. You can specify the range of the cells to be used in the pivot table. The following are the steps to create a pivot table using Aspose.Cells for Python via Java.

*   Load the Excel file or create a new one using [Workbook][28] class.
*   Insert data into the worksheet (optional).
*   Access pivot tables using [Worksheet.getPivotTables()][29] method.
*   Add a new pivot table using [Worksheet.getPivotTables().add(sourceData, destCellName, tableName)][30] method.
*   Configure row, column, and the data areas of the pivot table.
*   Save the workbook as _.xlsx_ using [Workbook.save(fileName)][31] method.

The following code sample shows how to create a pivot table in Excel using Python.

{{< gist aspose-com-gists f16dc7586917c051564eaebbb159c63f "create-excel-file-with-pivot-table.py" >}}



{{< figure align=center src="images/Create-Pivot-Table-in-Excel.jpg" alt="create pivot table in excel using python">}}


## Get a Free API License {#Free-API-License}

You can use Aspose.Cells for Python Java without evaluation limitations by getting a free [temporary license][32].

## Conclusion

In this article, you have seen **how to create Excel files from scratch using Python**. Furthermore, you have learned how to insert data, images, charts, and pivot tables within Excel worksheets programmatically. You can learn more about Aspose's Python Excel API using the [documentation][33].

## See Also

*   [Convert Excel Files to PDF using Python][34]
*   [Read Excel Files in Python][35]
*   [Export Excel Data to Google Sheets in Python][36]
*   [Add Watermark to Excel Files in Python][37]
*   [Add Comments in Excel Worksheets in Python][38]
*   [Create PowerPoint Files in Python][39]
*   [Convert PowerPoint PPT to HTML in Python][40]




[1]: https://en.wikipedia.org/wiki/Python_(programming_language)
[2]: #Python-Excel-API
[3]: #Create-Excel-XLS-XLSX-Files-using-Python
[4]: #Insert-Data-into-Existing-Excel-File-using-Python
[5]: #Create-Excel-File-having-Images-using-Python
[6]: #Generate-Charts-within-Excel-Worksheet-using-Python
[7]: #Create-Pivot-Tables-in-Excel-Worksheet-using-Python
[8]: #Free-API-License
[9]: https://products.aspose.com/slides/python-net/
[10]: https://products.aspose.app/slides/conversion/ppt-to-jpg)
[11]: https://products.aspose.com/cells/python-java
[12]: https://downloads.aspose.com/cells/python-java
[13]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[14]: https://apireference.aspose.com/cells/python/asposecells.api/Worksheet
[15]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#Worksheets
[16]: https://apireference.aspose.com/cells/python/asposecells.api/worksheet#Cells
[17]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String)
[18]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[19]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[20]: https://apireference.aspose.com/cells/python/asposecells.api/Worksheet
[21]: https://apireference.aspose.com/cells/python/asposecells.api/picturecollection#add(int,%20int,%20java.lang.String)
[22]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String)
[23]: https://apireference.aspose.com/cells/python/asposecells.api/ChartType
[24]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[25]: https://apireference.aspose.com/cells/python/asposecells.api/worksheet#Charts
[26]: https://apireference.aspose.com/cells/python/asposecells.api/chartcollection#add(int,%20int,%20int,%20int,%20int)
[27]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String)
[28]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[29]: https://apireference.aspose.com/cells/python/asposecells.api/worksheet#PivotTables
[30]: https://apireference.aspose.com/cells/python/asposecells.api/pivottablecollection#add(java.lang.String,%20java.lang.String,%20java.lang.String)
[31]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String)
[32]: https://purchase.aspose.com/temporary-license
[33]: https://docs.aspose.com/cells/pythonjava/
[34]: https://blog.aspose.com/2021/04/02/convert-excel-files-to-pdf-in-python/
[35]: https://blog.aspose.com/2021/12/09/read-excel-files-using-python/
[36]: https://blog.aspose.com/2022/02/14/export-excel-data-to-google-sheets-in-python/
[37]: https://blog.aspose.com/2021/05/07/add-watermark-to-excel-worksheets-in-python/
[38]: https://blog.aspose.com/2021/06/15/add-comments-in-excel-worksheets-using-python/
[39]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[40]: https://blog.aspose.com/2021/12/16/convert-ppt-to-html-in-python/





