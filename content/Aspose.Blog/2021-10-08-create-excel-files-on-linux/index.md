---
title: 'Create or Edit Excel Files on Linux using Java'
seoTitle: "Create Excel Files on Linux | Java Spreadsheet API for Linux"
description: "Create MS Excel XLSX or XLS files using Java on Linux. Java code samples of how to add tables, charts, and built-in or add-in functions in Excel."
date: Fri, 08 Oct 2021 13:59:00 +0000
draft: false
url: /2021/10/08/create-excel-files-on-linux/
author: Usman Aziz
summary: 'These days, spreadsheets are widely used to keep and share a large amount of tabular data. Also, you can perform various operations such as applying formulas, generating charts and graphs, sorting and filtering data, and so on. The spreadsheets automation has brough a revolution in various industries. The dynamic creation and manipulation of the spreadsheets have made the data handling quite easier. In order to perform spreadsheet manipulation programmatically, this article covers how to **create Excel XLSX or XLS files from scratch on Linux using Java**.'
tags: ['create excel files on linux', 'create xls files on linux', 'create xlsx files on linux']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Excel-File.jpg" alt="Create Excel Files on Linux">}}


These days, spreadsheets are widely used to keep and share a large amount of tabular data. Also, you can perform various operations such as applying formulas, generating charts and graphs, sorting and filtering data, and so on. The spreadsheets automation has brough a revolution in various industries. The dynamic creation and manipulation of the spreadsheets have made the data handling quite easier. In order to perform spreadsheet manipulation programmatically, this article covers how to **create Excel XLSX or XLS files from scratch on Linux using Java**.

*   [Java API to Create Excel Files on Linux][1]
*   [Create Excel XLSX or XLS Files on Linux][2]
*   [Edit Existing Excel Files][3]
*   [Create Charts in Excel Files][4]
*   [Create a Pivot Table in an XLSX][5]
*   [Add Formulas for Cells in XLSX][6]

## API to Create Excel Files on Linux - Free Download {#Java-API-to-Create-Excel-Files}

For creating and manipulating the Excel files, we will use [Aspose.Cells for Java][7]. It is a powerful spreadsheet manipulation API to create, update or convert Excel files. You can either [download][8] the API's JAR or install it within your Maven-based applications using the following configurations.

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
    <version>21.9</version>
</dependency>
```

## Create an Excel File on Linux {#Create-Excel-XLS-or-XLSX-Files-using-Java}

MS Excel files keep data in the worksheets that are composed of multiple cells. Whereas, these worksheets are contained by a workbook. The following are the steps to create an Excel XLSX file from scratch on Linux.

*   Create an instance of [Workbook][9] class.
*   Get reference of the desired worksheet using [Workbook.getWorksheets.get()][10] method.
*   Insert value in the desired cell of the worksheet using the cell’s identifier, such as A1, B3, etc.
*   Save the workbook using the [Workbook.save()][11] method.

The following code sample shows how to create an Excel XLSX file on Linux using Java.

{{< gist aspose-com-gists c6e9577bbbc58d56e081b5e5a1b349de "create-excel-file.java" >}}

The following is the output of the above code sample.



{{< figure align=center src="images/Create-Excel-Worksheet.jpg" alt="Create Excel file on Linux">}}


## Edit an Excel XLSX File on Linux {#Edit-an-Excel-XLSX-File-using-Java}

You can also modify the existing Excel files seamlessly. For this, you can simply load the file, access the desired worksheet, and update its content. The following are the steps to edit an Excel XLSX file.

*   Load the Excel file using [Workbook][12] class.
*   Get reference of the worksheets and cells using the [Worksheet][13] and [Cell][14] classes, respectively.
*   Update the content of the cells.
*   Save the updated workbook using [Workbook.save()][15] method.

The following code sample shows how to edit an Excel file on Linux.

{{< gist aspose-com-gists c6e9577bbbc58d56e081b5e5a1b349de "update-excel-file.java" >}}

## Create Charts in Excel Files on Linux {#Create-Charts-in-Excel-Files-using-Java}

Charts in spreadsheets are used to visually represent the data stored in the worksheets. Aspose.Cells for Java provides a [wide range of charts][16] that you can generate within the Excel files. The following are the steps to create a chart in an Excel XLSX file on Linux platform.

*   Create a new Excel file or load an existing one using [Workbook][17] class.
*   Add data to the worksheet (optional).
*   Get the chart collection of the worksheet using the [Worksheet.getCharts()][18] method.
*   Add a new chart to the collection using _Worksheet.getCharts().add()_ method.
*   Get reference of the newly created [Chart][19] from the collection.
*   Specify the cells’ range to set NSeries for the chart.
*   Finally, save the Excel file.

The following code sample shows how to create a chart in an Excel XLSX file.

{{< gist aspose-com-gists c6e9577bbbc58d56e081b5e5a1b349de "insert-chart-in-excel.java" >}}

The following screenshot shows the output of the above code sample.



{{< figure align=center src="images/Create-Chart-in-Excel.jpg" alt="create chart in excel linux">}}


## Create a Pivot Table in Excel File on Linux {#Create-a-Pivot-Table-in-Excel-using-Java}

Pivot tables in Excel worksheets have various purposes such as adding filters to the data, computing totals, summarizing data, and etc. Pivot tables can be created using the range of the cells in the worksheet. You can create a pivot table in an Excel file following the steps below.

*   Create a new Excel file or load an existing one using [Workbook][20] class.
*   Insert data into the worksheet (optional).
*   Access the pivot table collection using [Worksheet.getPivotTables()][21] method.
*   Add a new pivot table in the worksheet using _Worksheet.getPivotTables().add()_ method.
*   Provide data to the pivot table.
*   Save the workbook using [Workbook.save()][22] method.

The following code sample shows how to create a pivot table in Excel.

{{< gist aspose-com-gists c6e9577bbbc58d56e081b5e5a1b349de "insert-pivottable-in-excel.java" >}}

The following is the screenshot of the pivot table generated by the above code sample.



{{< figure align=center src="images/Create-Pivot-Table-in-Excel.jpg" alt="create pivot table in excel on linux">}}


## Add Formulas for Cells in Excel Files {#Add-Formulas-for-Cells-in-XLSX-using-Java}

Aspose.Cells for Java also supports working with formulas in Excel worksheets. The following sections describe how to work with built-in and add-in functions.

### Apply Built-in Functions in Excel

For built-in functions, you can simply get reference of the desired cell in the worksheet and add a formula using the [Cell.setFormula(String)][23] method. The following code sample shows how to set a built-in formula in Excel.

{{< gist aspose-com-gists c6e9577bbbc58d56e081b5e5a1b349de "add-builtin-formula.java" >}}

### Add Add-in Functions in Excel

Aspose.Cells for Java also supports user-defined function for the Excel worksheets. For this, you will have to register the add-in function using an [xlam][24] (Excel macro-enabled add-in) file. To register the add-in functions, the API provides [registerAddInFunction(int, String)][25] and [registerAddInFunction(String, String, boolean)][26] methods. The following code sample shows how to register and use an add-in function in Excel.

{{< gist aspose-com-gists c6e9577bbbc58d56e081b5e5a1b349de "add-addin-formula.java" >}}

## Get a Free License {#Get-a-Free-License}

You can use Aspose.Cells for Java without evaluation limitations using a [temporary license][27].

## Conclusion

In this article, you have learned how to create MS Excel files from scratch on Linux. Also, you have seen how to update the Excel files, generate charts, create pivot tables, and add formulas in the worksheets. You can learn more about Aspose.Cells for Java using [documentation][28]. In case you would have any questions, you can ask via our [forum][29].

## See Also

*   [Convert Excel Files to PDF using Java][30]
*   [Convert Excel Files to PDF on Linux using .NET][31]
*   [Import Data from JSON to Excel on Linux using .NET][32]




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
[15]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String)
[16]: https://docs.aspose.com/cells/java/creating-and-customizing-charts/#creating-a-simple-chart
[17]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook
[18]: https://apireference.aspose.com/cells/java/com.aspose.cells/worksheet#Charts
[19]: https://apireference.aspose.com/cells/java/com.aspose.cells/Chart
[20]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook
[21]: https://apireference.aspose.com/cells/java/com.aspose.cells/worksheet#PivotTables
[22]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String)
[23]: https://apireference.aspose.com/cells/java/com.aspose.cells/cell#Formula
[24]: https://docs.fileformat.com/spreadsheet/xlam/
[25]: https://apireference.aspose.com/cells/java/com.aspose.cells/worksheetcollection#registerAddInFunction(int,%20java.lang.String)
[26]: https://apireference.aspose.com/cells/java/com.aspose.cells/worksheetcollection#registerAddInFunction(java.lang.String,%20java.lang.String,%20boolean)
[27]: https://purchase.aspose.com/temporary-license
[28]: https://docs.aspose.com/cells/java/getting-started/
[29]: https://forum.aspose.com/
[30]: https://blog.aspose.com/2020/08/12/convert-excel-to-pdf-using-java/
[31]: https://blog.aspose.com/2021/10/12/convert-excel-files-to-pdf-on-linux/
[32]: https://blog.aspose.com/2021/09/16/import-data-from-json-to-excel-on-linux/




