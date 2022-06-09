---
title: 'How to Read Excel Files in Java'
seoTitle: "How to Read an Excel File in Java | Read Data from Excel Worksheets"
description: "Use Java Excel library to read Excel files in XLSX/XLS/CVS and other formats using Java. Read data from a single or all worksheets in an Excel file."
date: Wed, 10 Nov 2021 09:39:00 +0000
draft: false
url: /2021/11/10/how-to-read-excel-files-in-java/
author: Usman Aziz
summary: 'MS Excel files are largely used to keep tabular data in the form of worksheets. Often, the huge datasets are also maintained in Excel files. Therefore, you may come across the scenario where you need to read and fetch data from the worksheets in an Excel file. To achieve that, this article shows **how to read an Excel file in Java**. We will demonstrate how to read the whole Excel file or only a single worksheet programmatically.'
tags: ['read csv files in java', 'read excel files in java', 'read xls files in java', 'read xlsx files in java']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Excel-File.jpg" alt="Read data in Excel files using Java">}}


MS Excel files are largely used to keep tabular data in the form of worksheets. Often, the huge datasets are also maintained in Excel files. Therefore, you may come across the scenario where you need to read and fetch data from the worksheets in an Excel file. To achieve that, this article shows **how to read an Excel file in Java**. We will demonstrate how to read the whole Excel file or only a single worksheet programmatically.

*   [Java Library to Read Excel Files][1]
*   [Read Data from an Excel File][2]
*   [Read a Worksheet in an Excel Workbook][3]

## Java Library to Read Excel Files {#Library-to-Read-Excel-Files}

To read data from the worksheets, we will use [Aspose.Cells for Java][4]. It is a spreadsheet manipulation API to create Excel files from scratch. Moreover, it allows you to read and manipulate existing Excel files quite easily. The API can be downloaded from the [downloads section][5] or installed by adding the following Maven configurations in pom.xml.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-cells</artifactId>
    <version>21.11</version>
</dependency>
```

## Read an Excel File in Java {#Read-Data-from-an-Excel-File}

In Excel files, the data is stored in **cells** where each cell is identified by its name (A1, B3, etc.) or the row and column index. These cells collectively form a worksheet and an Excel file is comprised of single or multiple worksheets. All the worksheets are contained in a **workbook**. So this was a brief overview of the structure of an Excel file. Let's now proceed to read data from an Excel file.

The following are the steps to read an Excel file and print its data using Java.

*   Load the Excel file using [Workbook][6] class.
*   Create an object of [WorksheetCollection][7] class and get reference of the worksheets using [Workbook.getWorksheets()][8] method.
*   Start a loop to go though all the worksheets in the collection and in each iteration, perform the following steps:
    *   Get reference of the worksheet in a [Worksheet][9] object.
    *   Get count of data rows and columns in the worksheet.
    *   Start a loop for rows.
    *   Start a nested loop for columns.
    *   Read data from each cell using [Worksheet.getCells().get(rowIndex, columnIndex).getValue()][10] method.

The following code sample shows how to read an Excel file in Java.

{{< gist aspose-com-gists 7a30bbcd1b5018f7b44c9463e44f0d8b "read-excel-file.java" >}}

The following is the output that we get in the console after running the code sample above.



{{< figure align=center src="images/Read-Excel-Files.jpg" alt="Reading data in the worksheets of Excel file in Java" caption="Reading an Excel File in Java">}}


## Read a Particular Worksheet in Excel in Java {#Read-a-Worksheet-in-an-Excel-Workbook}

You can also read only a particular worksheet in the Excel file by following the steps below.

*   Load the Excel file using [Workbook][11] class.
*   Get reference of desired worksheet in a [Worksheet][12] object using [Workbook.getWorksheets().get(index)][13] method.
*   Get count of data rows and columns in the worksheet.
*   Start a loop for rows.
*   Start a nested loop for columns.
*   Read data from each cell using [Worksheet.getCells().get(rowIndex, columnIndex).getValue()][14] method.

The following code sample shows how to read data from a particular worksheet in Java.

{{< gist aspose-com-gists 7a30bbcd1b5018f7b44c9463e44f0d8b "read-worksheet.java" >}}

## Get a Free API License

You can use Aspose.Cells for Java without evaluation limitations by getting a [free temporary license][15].

## Conclusion

In this article, you have learned how to read Excel files dynamically in Java. With the help of code samples, you have seen how to read data from a particular worksheet or all the worksheets in an Excel workbook. In addition, you can explore other features of Aspose.Cells for Java using the [documentation][16]. In case you would have any queries, feel free to let us know via our [forum][17].

## See Also

*   [Create Excel Files using Java without MS Office][18]




[1]: #Library-to-Read-Excel-Files
[2]: #Read-Data-from-an-Excel-File
[3]: #Read-a-Worksheet-in-an-Excel-Workbook
[4]: https://products.aspose.com/cells/java/
[5]: https://downloads.aspose.com/cells/java/
[6]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[7]: https://apireference.aspose.com/cells/java/com.aspose.cells/WorksheetCollection
[8]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#Worksheets
[9]: https://apireference.aspose.com/cells/java/com.aspose.cells/Worksheet
[10]: https://apireference.aspose.com/cells/java/com.aspose.cells/cell#Value
[11]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[12]: https://apireference.aspose.com/cells/java/com.aspose.cells/Worksheet
[13]: https://apireference.aspose.com/cells/java/com.aspose.cells/worksheetcollection#Item%20(int)
[14]: https://apireference.aspose.com/cells/java/com.aspose.cells/cell#Value
[15]: https://purchase.aspose.com/temporary-license
[16]: https://docs.aspose.com/cells/java/
[17]: https://forum.aspose.com/
[18]: https://blog.aspose.com/2020/10/13/create-excel-xlsx-xls-using-java-without-ms-office/




