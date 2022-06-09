---
title: 'Create Excel Files from Scratch using PHP'
seoTitle: "Create Excel XLSX XLS Files in PHP | Create Charts and Tables in Excel"
description: "Create Excel XLSX files using PHP programmatically without MS Office or MS Excel. Create an Excel file with charts, graphs, and tables in PHP web apps."
date: Fri, 11 Jun 2021 16:26:32 +0000
draft: false
url: /2021/06/11/create-excel-files-from-scratch-using-php/
author: Usman Aziz
summary: '**Spreadsheets** have become an essential part of keeping, organizing, and analyzing the data. Since **automated solutions** are more in business these days, the trend of creating and manipulating Excel documents (XLS/XLSX) has emerged and growing at a huge pace. In accordance with the above-mentioned scenario, this article covers **how to create Excel XLSX or XLS files in PHP based web applications**.'
tags: ['Create Charts or Graphs in an Excel File using PHP', 'Create Excel XLS or XLSX Files using PHP', 'Create a Table in an Excel File using PHP', 'PHP Excel Automation API', 'Write Data to Existing Excel File using PHP']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/C-Excel-Automation-Library.png" alt="Create Excel files in PHP">}}


**Spreadsheets** have become an essential part of keeping, organizing, and analyzing the data. Since **automated solutions** are more in business these days, the trend of creating and manipulating Excel documents (XLS/XLSX) has emerged and growing at a huge pace. In accordance with the above-mentioned scenario, this article covers **how to create Excel XLSX or XLS files in PHP based web applications**.

*   [PHP Excel Automation API][1]
*   [Create Excel XLS or XLSX Files using PHP][2]
*   [Write Data to Existing Excel File using PHP][3]
*   [Create Charts or Graphs in an Excel File using PHP][4]
*   [Create a Table in an Excel File using PHP][5]

## PHP API to Create Excel Files {#PHP-Excel-Automation-API}

In order to create and manipulate Excel files in PHP based web applications, we will use [Aspose.Cells for PHP via Java][6]. It is a powerful API that provides a wide range of features for Excel automation. You can download the API package from [here][7].

### Usage

The following are the prerequisites that you need to fulfill in order to use _Aspose.Cells for PHP via Java_.

*   [Java SE Development Kit 1.7 or higher][8]
*   [PHP 7.0 or higher][9]
*   [Java Bridge][10]
*   [Java Inc][11]

Once you have completed the prerequisites, follow the below steps to execute the _example.php_ file for testing.

1.  Place _Java.inc_ file in the root folder of the API’s package that you have downloaded.
2.  Run _JavaBridge.jar_ using the below commands in the command prompt:
    *   \> cd aspose.cells
    *   \> %JAVA\_HOME%\\bin\\java -Djava.ext.dirs=lib -jar JavaBridge.jar SERVLET\_LOCAL:8080
3.  Run _example.php_ from the API’s root folder using the below command:
    *   \> php example.php

## Create Excel XLS or XLSX Files using PHP {#Create-Excel-XLS-or-XLSX-Files-using-PHP}

The following are the steps to create an Excel XLSX/XLS file using PHP.

*   Create an object of [Workbook][12] class.
*   Access the [WorksheetCollection][13] using [$workbook->getWorksheets()][14] method.
*   Access [Cells][15] collection of the desired worksheet using [$worksheets->get(index)->getCells()][16] method.
*   Insert value into the desired cell using [$cells->get("A1")->putValue("Hello world!")][17] method.
*   Save the Excel workbook using [$workbook->save("output.xlsx", cells\\SaveFormat::XLSX)][18] method.

The following code sample shows how to create an Excel XLSX file using PHP.

{{< gist aspose-com-gists decc4c44d870ffe2223a550c26f9e98e "create-excel-file.php" >}}

## Write Data to Existing Excel File using PHP {#Write-Data-to-Existing-Excel-File-using-PHP}

In the previous section, we created an Excel file from scratch. Now, let's edit an existing Excel file and insert data into it. The following are the steps to write data to an XLSX file using Aspose.Cells for PHP via Java.

*   Create an object of [Workbook][19] class and initialize it with the path to the Excel file.
*   Access the [WorksheetCollection][20] of the Excel file using [$workbook->getWorksheets()][21] method.
*   Access [Cells][22] collection of the desired worksheet using [$worksheets->get(index)->getCells()][23] method.
*   Insert value into the desired cell using [$cells->get("A1")->putValue("Hello world!")][24] method.
*   Save the Excel workbook using [$workbook->save("output.xlsx", cells\\SaveFormat::XLSX)][25] method.

The following code sample shows how to modify an Excel file and write data into it using PHP.

{{< gist aspose-com-gists decc4c44d870ffe2223a550c26f9e98e "modify-excel-file.php" >}}

## Create Charts in an Excel File using PHP {#Create-Charts-in-an-Excel-File-using-PHP}

The following are the steps to create charts in an Excel file using PHP.

*   Create a new Excel file or load an existing one using the [Workbook][26] class.
*   Add data to the worksheet if a new workbook is created.
*   Get the chart collection of the worksheet using the [$worksheet->getCharts()][27] method.
*   Add a new chart using [$worksheet->getCharts()->add()][28] method.
*   Get the newly created [Chart][29] from the collection.
*   Specify the cells’ range to set NSeries for the chart.
*   Save the workbook as an Excel _.xlsx_ file using [$workbook->save("output.xlsx", cells\\SaveFormat::XLSX)][30] method.

The following code sample shows how to create charts in Excel files in PHP.

{{< gist aspose-com-gists decc4c44d870ffe2223a550c26f9e98e "create-chart-in-excel.php" >}}

## Create a Pivot Table in an Excel File using PHP {#Create-a-Table-in-an-Excel-File-using-PHP}

Pivot tables in Excel worksheets are used for adding filters to the data, computing totals, summarizing data, etc. Pivot tables can be created using the range of the cells in the worksheet. The following are the steps to create a pivot table in an Excel worksheet using PHP.

*   Create a new Excel file or load an existing one using the [Workbook][31] class.
*   Insert data into the worksheet.
*   Access the pivot table collection using [$worksheet->getPivotTables()][32] method.
*   Add a new pivot table in the worksheet using [$worksheet->getPivotTables()->add()][33] method.
*   Provide data to the pivot table.
*   Save the workbook using [$workbook->save("output.xlsx", cells\\SaveFormat::XLSX)][34] method.

The following code sample shows how to create a pivot table in Excel using PHP.

{{< gist aspose-com-gists decc4c44d870ffe2223a550c26f9e98e "create-excel-pivot-table.php" >}}

## Get a Free API License {#Get-Free-License}

You can use the API for free without evaluation limitations using a [temporary license][35].

## Conclusion

In this article, you have learned how to create Excel files from scratch using PHP. Furthermore, you have seen how to write data to an existing Excel file and generate charts or tables. You can explore more about the PHP Excel API using the [documentation][36]. In case you would have any questions, feel free to let us know via our [forum][37].

## See Also

*   [Convert Excel Files to HTML in PHP][38]
*   [Convert Excel Files to PDF in PHP][39]




[1]: #PHP-Excel-Automation-API
[2]: #Create-Excel-XLS-or-XLSX-Files-using-PHP
[3]: #Write-Data-to-Existing-Excel-File-using-PHP
[4]: #Create-Charts-in-an-Excel-File-using-PHP
[5]: #Create-a-Table-in-an-Excel-File-using-PHP
[6]: https://products.aspose.com/cells/php-java
[7]: https://downloads.aspose.com/cells/php
[8]: https://www.oracle.com/technetwork/java/javase/downloads/java-archive-downloads-javase7-521261.html
[9]: https://www.php.net/downloads.php
[10]: https://sourceforge.net/projects/php-java-bridge/files/Binary%20package/php-java-bridge_7.2.1/exploded/JavaBridge.jar/download
[11]: http://php-java-bridge.sourceforge.net/pjb/download.php
[12]: https://apireference.aspose.com/cells/php/aspose.cells/Workbook
[13]: https://apireference.aspose.com/cells/php/aspose.cells/WorksheetCollection
[14]: https://apireference.aspose.com/cells/php/aspose.cells/workbook#Worksheets
[15]: https://apireference.aspose.com/cells/php/aspose.cells/Cells
[16]: https://apireference.aspose.com/cells/php/aspose.cells/worksheet#Cells
[17]: https://apireference.aspose.com/cells/php/aspose.cells/cell#putValue(java.lang.String)
[18]: https://apireference.aspose.com/cells/php/aspose.cells/workbook#save(java.lang.String,%20int)
[19]: https://apireference.aspose.com/cells/php/aspose.cells/Workbook
[20]: https://apireference.aspose.com/cells/php/aspose.cells/WorksheetCollection
[21]: https://apireference.aspose.com/cells/php/aspose.cells/workbook#Worksheets
[22]: https://apireference.aspose.com/cells/php/aspose.cells/Cells
[23]: https://apireference.aspose.com/cells/php/aspose.cells/worksheet#Cells
[24]: https://apireference.aspose.com/cells/php/aspose.cells/cell#putValue(java.lang.String)
[25]: https://apireference.aspose.com/cells/php/aspose.cells/workbook#save(java.lang.String,%20int)
[26]: https://apireference.aspose.com/cells/php/aspose.cells/Workbook
[27]: https://apireference.aspose.com/cells/php/aspose.cells/worksheet#Charts
[28]: https://apireference.aspose.com/cells/php/aspose.cells/chartcollection#add(int,%20int,%20int,%20int,%20int)
[29]: https://apireference.aspose.com/cells/php/aspose.cells/Chart
[30]: https://apireference.aspose.com/cells/php/aspose.cells/workbook#save(java.lang.String,%20int)
[31]: https://apireference.aspose.com/cells/php/aspose.cells/Workbook
[32]: https://apireference.aspose.com/cells/php/aspose.cells/worksheet#PivotTables
[33]: https://apireference.aspose.com/cells/php/aspose.cells/pivottablecollection#add(com.aspose.cells.PivotTable,%20java.lang.String,%20java.lang.String)
[34]: https://apireference.aspose.com/cells/php/aspose.cells/workbook#save(java.lang.String,%20int)
[35]: https://purchase.aspose.com/temporary-license
[36]: https://docs.aspose.com/cells/phpjava/
[37]: https://forum.aspose.com/
[38]: https://blog.aspose.com/2021/05/25/convert-excel-to-html-in-php/
[39]: https://blog.aspose.com/2021/05/11/convert-excel-files-to-pdf-in-php/





