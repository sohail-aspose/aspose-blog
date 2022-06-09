---
title: 'Create Excel File in Android Programmatically'
seoTitle: "Create Excel File in Android Programmatically | Android Excel API"
description: "Use Android Excel API to create Excel file in Android apps programmatically. Create, edit, convert and write data to the Excel files within your apps."
date: Fri, 18 Jun 2021 17:46:00 +0000
draft: false
url: /2021/06/18/create-excel-file-in-android-programmatically/
author: Usman Aziz
summary: 'In this article, you will learn how to implement Excel automation features from within your Android applications. After reading this article, you will be able to **create Excel XLSX or XLS file from scratch in your Android app programmatically**. In addition, this article will cover how to update an existing Excel file, generate charts, apply formulas, and add pivot tables in Excel worksheets.'
tags: ['Android API to Create Excel File', 'Android Excel API', 'Create Charts in Excel Files in Android', 'Create Excel XLSX or XLS Files Android', 'Edit Existing Excel Files in Android']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/C-Excel-Automation-Library.png" alt="create Excel files in Android">}}


In this article, you will learn how to implement Excel automation features from within your Android applications. After reading this article, you will be able to **create Excel XLSX or XLS file from scratch in your Android app programmatically**. In addition, this article will cover how to update an existing Excel file, generate charts, apply formulas, and add pivot tables in Excel worksheets.

*   [Android API to Create Excel File][1]
*   [Create Excel XLSX or XLS Files][2]
*   [Edit Existing Excel Files][3]
*   [Create Charts in Excel Files][4]
*   [Create a Pivot Table in an XLSX][5]
*   [Add Formulas for Cells in XLSX][6]

## Android API to Create Excel File - Free Download {#Java-API-to-Create-Excel-Files}

[Aspose.Cells for Android via Java][7] is a powerful spreadsheet manipulation API that lets you create or modify Excel files without MS Office. The API supports adding charts, graphs, formulas, and perform other spreadsheet manipulation operations programmatically. You can either [download][8] the API or install it using the following configurations in build.gradle.

```
maven {
    url "https://repository.aspose.com/repo/" }
```
```
compile (
        group: 'com.aspose',
        name: 'aspose-cells',
        version: '21.3',
        classifier: 'android.via.java')
```

## Create Excel XLSX or XLS in Android {#Create-Excel-XLS-or-XLSX-Files-using-Java}

Each Excel workbook is composed of one or more worksheets that further contain the rows and columns to keep the data in the form of cells. The following are the steps to create an Excel XLSX file from scratch.

*   Create an instance of [Workbook][9] class.
*   Access the desired worksheet using [Workbook.getWorksheets.get()][10] method.
*   Put the value in the desired cell in the worksheet using the cell’s identifier, such as A1, B3, etc.
*   Save the workbook as an Excel file using the [Workbook.save()][11] method.

The following code sample shows how to create an Excel XLSX file in Android.

{{< gist aspose-com-gists c6e9577bbbc58d56e081b5e5a1b349de "create-excel-file.java" >}}



{{< figure align=center src="images/Create-Excel-Worksheet.jpg" alt="create Excel XLSX XLS in Android">}}


## Edit an Excel XLSX File in Android {#Edit-an-Excel-XLSX-File-using-Java}

Lets now have a look at how to modify or insert data into an existing MS Excel file. For this, you can simply load the file, access the desired worksheet and save the updated file. The following are the steps to modify an existing Excel file.

*   Open Excel file using [Workbook][12] class.
*   Access the worksheets and cells using the [Worksheet][13] and [Cell][14] classes respectively.
*   Save the updated workbook as an Excel _.xlsx_ file.

The following code sample shows how to edit an existing MS Excel file in Android.

{{< gist aspose-com-gists c6e9577bbbc58d56e081b5e5a1b349de "update-excel-file.java" >}}

## Create Charts or Graphs in Excel in Android {#Create-Charts-in-Excel-Files-using-Java}

Charts in spreadsheets are used to visually represent the data stored in the worksheets. They make it easier to analyze a large amount of data quite easily. Aspose.Cells for Android via Java provides a [wide range of charts][15] that you can create within the Excel files programmatically. The following are the steps to create a chart in an Excel XLSX file.

*   Create a new Excel file or load an existing one using [Workbook][16] class.
*   Add data to the worksheet (optional).
*   Get the chart collection of the worksheet using the [Worksheet.getCharts()][17] method.
*   Add a new chart using _Worksheet.getCharts().add()_ method.
*   Get the newly created chart from the collection.
*   Specify the cells’ range to set NSeries for the chart.
*   Save the workbook as an Excel _.xlsx_ file.

The following code sample shows how to create a chart in Excel XLSX in Android.

{{< gist aspose-com-gists c6e9577bbbc58d56e081b5e5a1b349de "insert-chart-in-excel.java" >}}



{{< figure align=center src="images/Create-Chart-in-Excel.jpg" alt="create chart in excel Android">}}


## Create a Pivot Table in Excel XLSX in Android {#Create-a-Pivot-Table-in-Excel-using-Java}

Pivot tables in Excel worksheets have various purposes such as adding filters to the data, computing totals, summarizing data, and etc. Pivot tables can be created using the range of the cells in the worksheet. The following are the steps to create a pivot table in an Excel worksheet.

*   Create a new [Workbook][18] or load an existing file.
*   Insert data into the worksheet (optional).
*   Access the pivot table collection using [Worksheet.getPivotTables()][19] method.
*   Add a new pivot table in the worksheet using _Worksheet.getPivotTables().add()_ method.
*   Provide data to the pivot table.
*   Save the workbook.

The following code sample shows how to create a pivot table in Excel.

{{< gist aspose-com-gists c6e9577bbbc58d56e081b5e5a1b349de "insert-pivottable-in-excel.java" >}}



{{< figure align=center src="images/Create-Pivot-Table-in-Excel.jpg" alt="create pivot table in excel ">}}


## Add Formulas for Cells in Excel File {#Add-Formulas-for-Cells-in-XLSX-using-Java}

Aspose.Cells for Android via Java also allows you to work with formulas in the Excel worksheets. You can apply the built-in as well as add-in functions to the cells.

### Apply Built-in Functions in Excel

For using the built-in functions, you can simply access the desired cell in the worksheet and add formula using the [Cell.setFormula(String)][20] method. The following code sample shows how to set a built-in formula.

{{< gist aspose-com-gists c6e9577bbbc58d56e081b5e5a1b349de "add-builtin-formula.java" >}}

### Add Add-in Functions in Excel

There might be a case when you have to use a user-defined function. For this, you will have to register the add-in function using a .xlam (Excel macro-enabled add-in) file and then use it for the desired cells. For registering the add-in functions, Aspose.Cells for Android via Java provides [registerAddInFunction(int, String)][21] and [registerAddInFunction(String, String, boolean)][22] methods. The following code sample shows how to register and use an add-in function.

{{< gist aspose-com-gists c6e9577bbbc58d56e081b5e5a1b349de "add-addin-formula.java" >}}

## Conclusion

In this article, you have seen how to create MS Excel files from scratch in Android without MS Office. You have also learned how to update workbooks, create charts, add tables, and apply formulas to cell values within MS Excel worksheets. You can learn more about Android Excel API using [documentation][23]. In case you would have any queries, feel free to let us know via our [forum][24].

## See Also

*   [Convert Excel Files to PDF in Android][25]




[1]: #Java-API-to-Create-Excel-Files
[2]: #Create-Excel-XLS-or-XLSX-Files-using-Java
[3]: #Edit-an-Excel-XLSX-File-using-Java
[4]: #Create-Charts-in-Excel-Files-using-Java
[5]: #Create-a-Pivot-Table-in-Excel-using-Java
[6]: #Add-Formulas-for-Cells-in-XLSX-using-Java
[7]: https://products.aspose.com/cells/android-java/
[8]: https://downloads.aspose.com/cells/androidjava
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
[24]: https://forum.aspose.com/
[25]: https://blog.aspose.com/2021/04/21/convert-excel-files-to-pdf-in-android/





