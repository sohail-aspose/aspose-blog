---
title: 'Create Excel Files using Java without MS Office'
seoTitle: "Create Excel Files in Java | Add Charts, Tables, Formulas in XLSX XLS"
description: "Create MS Excel XLSX or XLS files using Java without MS Office. Java code samples of how to add tables, charts, and built-in or add-in functions in Excel."
date: Tue, 13 Oct 2020 02:34:04 +0000
draft: false
url: /2020/10/13/create-excel-xlsx-xls-using-java-without-ms-office/
author: Usman Aziz
summary: 'MS Excel spreadsheets have made it easier to keep and share a large amount of tabular data. Not only this, you can perform various operations such as applying formulas, generating charts and graphs, sorting and filtering data, and so on. In this article, you will learn how to implement Excel automation features from within your Java applications. After reading this article, you will be able to create MS Excel XLSX or XLS files from scratch using Java. In addition, this article will cover how to update an existing Excel file, generate charts, and add tables in Excel worksheets.'
tags: ['add charts in excel using java', 'add pivot table in excel using java', 'create excel files in java', 'create xls in java', 'create xlsx in java']
categories: ['Aspose.Cells Product Family']
---

MS Excel spreadsheets have made it easier to keep and share a large amount of tabular data. Not only this, you can perform various operations such as applying formulas, generating charts and graphs, sorting and filtering data, and so on. In this article, you will learn how to implement Excel automation features from within your Java applications. After reading this article, you will be able to **create Excel XLSX or XLS files from scratch using Java**. In addition, this article will cover how to update an existing Excel file, generate charts, apply formulas, and add pivot tables in Excel worksheets.

*   [Java API to Create Excel Files][1]
*   [Create Excel XLSX or XLS Files using Java][2]
*   [Edit Existing Excel Files using Java][3]
*   [Create Charts in Excel Files using Java][4]
*   [Create a Pivot Table in an XLSX using Java][5]
*   [Add Formulas for Cells in XLSX using Java][6]

## Java API to Create Excel Files - Free Download {#Java-API-to-Create-Excel-Files}

[Aspose.Cells for Java][7] is a powerful spreadsheet manipulation API that lets you create or modify Excel files without MS Office. The API supports adding charts, graphs, formulas, and perform other spreadsheet manipulation operations programmatically. You can [download][8] the API for free or install it within your Maven-based applications.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-cells</artifactId>
    <version>20.9</version>
</dependency>
```

## Create Excel XLSX or XLS using Java {#Create-Excel-XLS-or-XLSX-Files-using-Java}

The MS Excel files are referred to as workbooks and each workbook is composed of one or more worksheets. The worksheets further contain the rows and columns to keep the data in the form of cells. So let's start by creating a simple workbook. The following are the steps to create an Excel XLSX file from scratch.

*   Create an instance of [Workbook][9] class.
*   Access the desired worksheet using [Workbook.getWorksheets.get()][10] method.
*   Put the value in the desired cell in the worksheet using the cell’s identifier, such as A1, B3, etc.
*   Save the workbook as an Excel file using the [Workbook.save()][11] method.

The following code sample shows how to create an Excel XLSX file using Java.

{{< gist aspose-com-gists c6e9577bbbc58d56e081b5e5a1b349de "create-excel-file.java" >}}



{{< figure align=center src="images/Create-Excel-Worksheet.jpg" alt="">}}


## Edit an Excel XLSX File using Java {#Edit-an-Excel-XLSX-File-using-Java}

Lets now have a look at how to modify or insert data into an existing MS Excel file. For this, you can simply load the file, access the desired worksheet and save the updated file. The following are the steps to modify an existing Excel file.

*   Open Excel file using [Workbook][12] class.
*   Access the worksheets and cells using the [Worksheet][13] and [Cell][14] classes respectively.
*   Save the updated workbook as an Excel _.xlsx_ file.

The following code sample shows how to edit an existing MS Excel file using Java.

{{< gist aspose-com-gists c6e9577bbbc58d56e081b5e5a1b349de "update-excel-file.java" >}}

## Create Charts or Graphs in Excel using Java {#Create-Charts-in-Excel-Files-using-Java}

Charts in spreadsheets are used to visually represent the data stored in the worksheets. They make it easier to analyze a large amount of data quite easily. Aspose.Cells for Java provides a [wide range of charts][15] that you can create within the Excel files programmatically. The following are the steps to create a chart in an Excel XLSX file.

*   Create a new Excel file or load an existing one using [Workbook][16] class.
*   Add data to the worksheet (optional).
*   Get the chart collection of the worksheet using the [Worksheet.getCharts()][17] method.
*   Add a new chart using _Worksheet.getCharts().add()_ method.
*   Get the newly created chart from the collection.
*   Specify the cells’ range to set NSeries for the chart.
*   Save the workbook as an Excel _.xlsx_ file.

The following code sample shows how to create chart in Excel XLSX using Java.

{{< gist aspose-com-gists c6e9577bbbc58d56e081b5e5a1b349de "insert-chart-in-excel.java" >}}



{{< figure align=center src="images/Create-Chart-in-Excel.jpg" alt="create chart in excel using java">}}


## Create a Pivot Table in Excel XLSX using Java {#Create-a-Pivot-Table-in-Excel-using-Java}

Pivot tables in Excel worksheets have various purposes such as adding filters to the data, computing totals, summarizing data, and etc. Pivot tables can be created using the range of the cells in the worksheet. The following are the steps to create a pivot table in an Excel worksheet.

*   Create a new [Workbook][18] or load an existing file.
*   Insert data into the worksheet (optional).
*   Access the pivot table collection using [Worksheet.getPivotTables()][19] method.
*   Add a new pivot table in the worksheet using _Worksheet.getPivotTables().add()_ method.
*   Provide data to the pivot table.
*   Save the workbook.

The following code sample shows how to create pivot table in Excel using Java.

{{< gist aspose-com-gists c6e9577bbbc58d56e081b5e5a1b349de "insert-pivottable-in-excel.java" >}}



{{< figure align=center src="images/Create-Pivot-Table-in-Excel.jpg" alt="create pivot table in excel using java">}}


## Add Formulas for Cells in Excel File using Java {#Add-Formulas-for-Cells-in-XLSX-using-Java}

Aspose.Cells for Java also allows you to work with formulas in the Excel worksheets. You can apply the built-in as well as add-in functions to the cells.

### Apply Built-in Functions in Excel

For using the built-in functions, you can simply access the desired cell in the worksheet and add formula using the [Cell.setFormula(String)][20] method. The following code sample shows how to set a built-in formula using Java.

{{< gist aspose-com-gists c6e9577bbbc58d56e081b5e5a1b349de "add-builtin-formula.java" >}}

### Add Add-in Functions in Excel

There might be a case when you have to use a user-defined function. For this, you will have to register the add-in function using a .xlam (Excel macro-enabled add-in) file and then use it for the desired cells. For registering the add-in functions, Aspose.Cells for Java provides [registerAddInFunction(int, String)][21] and [registerAddInFunction(String, String, boolean)][22] methods. The following code sample shows how to register and use an add-in function using Java.

{{< gist aspose-com-gists c6e9577bbbc58d56e081b5e5a1b349de "add-addin-formula.java" >}}

## Conclusion

In this article, you have seen how to create MS Excel files from scratch using Java without MS Office. You have also learned how to update workbooks, create charts, add tables, and apply formulas to cell values within MS Excel worksheets. You can learn more about Aspose's Java Excel API using [documentation][23].

## See Also

*   [Convert Excel Files to PDF using Java][24]




[1]: #Java-API-to-Create-Excel-Files
[2]: #Create-Excel-XLS-or-XLSX-Files-using-Java
[3]: #Edit-an-Excel-XLSX-File-using-Java
[4]: #Create-Charts-in-Excel-Files-using-Java
[5]: #Create-a-Pivot-Table-in-Excel-using-Java
[6]: #Add-Formulas-for-Cells-in-XLSX-using-Java
[7]: https://products.aspose.com/cells/java
[8]: https://downloads.aspose.com/cells/java
[9]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[10]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#Worksheets
[11]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String)
[12]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook
[13]: https://apireference.aspose.com/cells/java/com.aspose.cells/Worksheet
[14]: https://apireference.aspose.com/cells/java/com.aspose.cells/Cell
[15]: https://docs.aspose.com/cells/java/creating-and-customizing-charts/#creating-a-simple-chart
[16]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook
[17]: https://apireference.aspose.com/cells/java/com.aspose.cells/worksheet#Charts
[18]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook
[19]: https://apireference.aspose.com/cells/java/com.aspose.cells/worksheet#PivotTables
[20]: https://apireference.aspose.com/cells/java/com.aspose.cells/cell#Formula
[21]: https://apireference.aspose.com/cells/java/com.aspose.cells/worksheetcollection#registerAddInFunction(int,%20java.lang.String)
[22]: https://apireference.aspose.com/cells/java/com.aspose.cells/worksheetcollection#registerAddInFunction(java.lang.String,%20java.lang.String,%20boolean)
[23]: https://docs.aspose.com/cells/java/getting-started/
[24]: https://blog.aspose.com/2020/08/12/convert-excel-to-pdf-using-java/





