---
title: 'Create Excel XLSX/XLS File in Node.js Applications - A Complete Guide'
seoTitle: ""
description: ""
date: Wed, 05 Aug 2020 17:10:33 +0000
draft: false
url: /2020/08/05/create-excel-files-in-node.js/
author: Usman Aziz
summary: ''
tags: ['Create Excel Files in Node.js', 'create spreadsheets in node.js', 'create xlsx files in node.js']
categories: ['Aspose.Cells Product Family']
---

In this article, I'll show you how to implement Excel automation and **create Excel XLSX/XLS file in Node.js** applications programmatically.



{{< figure align=center src="images/Create-Excel-Files-in-Nodejs-Logo.jpg" alt="create excel file in nodejs - logo">}}


[Spreadsheets][1] have made it possible to store a huge amount of data in the form of rows, columns, and sheets. In addition, you can perform a variety of operations on the data such as sorting, applying mathematical formulas, generating charts and graphs, and much more. In the current era of the digital world, automation has taken the place of manual work. As a result, Excel automation has also emerged as a tool to generate spreadsheet documents without any third-party software. Keeping that in mind, I'll let you know how to create Excel file and insert various objects in worksheets in Node.js.

*   [Excel API for Node.js][2]
*   [Create Excel File in Node.js][3]
*   [Insert Data into an Excel File in Node.js][4]
*   [Create an Excel File having Image in Node.js][5]
*   [Insert Charts or Graphs in Excel in Node.js][6]
*   [Create a Pivot Table in Excel in Node.js][7]

## Create Excel File with Node.js API {#Excel-API-for-Node.js}

[Aspose.Cells for Node.js via Java][8] is a powerful spreadsheet manipulation API that lets you create, edit, or convert Excel file within Node.js applications. The API's easy to use methods enable you to perform Excel automation features seamlessly in a few lines of code. You can [download][9] the API's package and integrate it into your Node.js application. For more details, you can visit the [Installation and Usage][10] guide.

## Create Excel XLSX File in Node.js {#Create-Excel-Files-in-Node.js}

The following are steps to create a simple Excel file using Aspose.Cells for Node.js via Java:

*   Create an instance of [Workbook][11] class.
*   Access the desired worksheet from the workbook using [Workbook.getWorksheets.get()][12] method.
*   Put the value in the desired cell in the worksheet using the cell's identifier, such as A1, B3, etc.
*   Save the workbook as an Excel file using [Workbook.save()][13] method.

The following code sample shows how to create an Excel file in Node.js.

{{< gist aspose-com-gists 1008531e0e9ae8c99b24a405b502f4c8 "create-excel-file.js" >}}



{{< figure align=center src="images/Create-Excel-Worksheet.jpg" alt="create excel file in node.js">}}


## Insert Data into an Excel XLSX in Node.js {#Insert-Data-into-an-Excel-File-in-Node.js}

You can also load an existing Excel file to update its content. The only thing you'll have to do is provide the Excel file's path in the Workbook constructor. The following code sample shows how to update the content of an existing Excel file in Node.js.

{{< gist aspose-com-gists 1008531e0e9ae8c99b24a405b502f4c8 "insert-data-in-existing-excel.js" >}}

## Create an Excel File having Image in Node.js {#Create-an-Excel-File-having-Image-in-Node.js}

The following are the steps to insert an image in an Excel worksheet in Node.js.

*   Create an instance of [Workbook][14] class.
*   Access the desired worksheet as well as cell in the worksheet.
*   Set the height and width of the cell using _setRowHeight()_ and _setColumnWidth()_ methods of [Cell][15] class.
*   Insert image using [Worksheet.getPictures().add(upperLeftRow, upperLeftColumn, fileName)][16] method.
*   Save the workbook as an Excel file.

The following code sample shows how to insert an image in the Excel worksheet in Node.js.

{{< gist aspose-com-gists 1008531e0e9ae8c99b24a405b502f4c8 "insert-image-in-excel.js" >}}



{{< figure align=center src="images/Insert-Image-in-Excel.jpg" alt="Insert image in Excel in node.js">}}


## Insert Charts or Graphs in Excel in Node.js {#Insert-Charts-or-Graphs-in-an-Excel-in-Node.js}

Chart and graphs are important components of Excel files that are used to visually represent the data. Aspose.Cells for Node.js via Java lets you draw and manipulate a [variety of charts][17] including sunburst, treemap, histogram, pyramid, and etc. The following are the simple steps to draw a chart in the Excel worksheet.

*   Create a new Excel file or load an existing one using [Workbook][18] class.
*   Add data to the worksheet as a data source for charts.
*   Access the chart collection of the worksheet using [Worksheet.getCharts()][19] method.
*   Add a new chart using _Worksheet.getCharts().add()_ method.
*   Access the newly created chart from the collection in a new variable.
*   Specify the cells’ range to set NSeries for the chart.
*   Save the workbook as an Excel _.xlsx_ file.

The following code sample shows how to draw charts in Excel in Node.js.

{{< gist aspose-com-gists 1008531e0e9ae8c99b24a405b502f4c8 "insert-chart-in-excel.js" >}}



{{< figure align=center src="images/Create-Chart-in-Excel.jpg" alt="insert chart in excel in node.js">}}


## Create a Pivot Table in Excel in Node.js {#Create-a-Table-in-an-Excel-File-in-Node.js}

Excel files also allow you to create pivot tables based on a range of cells to summarize a large amount of data. The following are the steps to create a pivot table within an Excel worksheet.

*   Create a new [Workbook][20] or load an existing excel file.
*   Insert data into the worksheet (optional).
*   Access the pivot table collection using [Worksheet.getPivotTables()][21] method.
*   Add a new pivot table in the worksheet using _Worksheet.getPivotTables().add()_ method.
*   Provide data to the pivot table.
*   Save the workbook as Excel file.

The following code sample shows how to create a pivot table in Excel in Node.js.

{{< gist aspose-com-gists 1008531e0e9ae8c99b24a405b502f4c8 "insert-pivottable-in-excel.js" >}}



{{< figure align=center src="images/Create-Pivot-Table-in-Excel.jpg" alt="create pivot table in excel in node.js">}}


## Conclusion

In this article, you have learned how to create an Excel XLSX or XLS file from scratch in Node.js applications. We have also seen how to insert data, images, charts, and pivot tables in Excel worksheets. You can learn more about the advanced features of Aspose.Cells for Node.js via Java using the [documentation][22].

## See Also

*   [Convert Excel Files to PDF in Node.js][23]
*   [Convert Excel Files to HTML in Node.js][24]
*   [Convert CSV to Excel or Excel to CSV in Node.js][25]
*   [Create Excel File Programmatically using C#][26]




[1]: https://en.wikipedia.org/wiki/Spreadsheet
[2]: #Excel-API-for-Node.js
[3]: #Create-Excel-Files-in-Node.js
[4]: #Insert-Data-into-an-Excel-File-in-Node.js
[5]: #Create-an-Excel-File-having-Image-in-Node.js
[6]: #Insert-Charts-or-Graphs-in-an-Excel-in-Node.js
[7]: #Create-a-Table-in-an-Excel-File-in-Node.js
[8]: https://products.aspose.com/cells/nodejs-java
[9]: https://downloads.aspose.com/cells/nodejs
[10]: https://docs.aspose.com/display/cellsjava/Setup+Environment+and+Installation+Guidelines
[11]: https://apireference.aspose.com/cells/nodejs/Workbook
[12]: https://apireference.aspose.com/cells/nodejs/Workbook#getWorksheets
[13]: https://apireference.aspose.com/cells/nodejs/Workbook#save
[14]: https://apireference.aspose.com/cells/nodejs/Workbook
[15]: https://apireference.aspose.com/cells/nodejs/Cell
[16]: https://apireference.aspose.com/cells/nodejs/PictureCollection#add
[17]: https://apireference.aspose.com/cells/nodejs/Chart
[18]: https://apireference.aspose.com/cells/nodejs/Workbook
[19]: https://apireference.aspose.com/cells/nodejs/Worksheet#getCharts
[20]: https://apireference.aspose.com/cells/nodejs/Workbook
[21]: https://apireference.aspose.com/cells/nodejs/Worksheet#getPivotTables
[22]: https://docs.aspose.com/display/cellsjava/Create+Pivot+Table
[23]: https://blog.aspose.com/2021/03/05/convert-excel-xlsx-xls-to-pdf-in-node-js/
[24]: https://blog.aspose.com/2021/02/11/convert-excel-files-to-html-in-node-js/
[25]: https://blog.aspose.com/2021/04/28/convert-csv-to-excel-or-excel-to-csv-in-nodejs/
[26]: https://blog.aspose.com/2020/01/21/create-excel-xls-xlsx-programmatically-in-csharp-net/





