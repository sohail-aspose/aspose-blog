---
title: 'Copy Rows and Columns in Excel using Java'
seoTitle: "Copy Rows and Columns in Excel in Java | Aspose.Cells for Java"
description: "Use Java Excel API to copy rows and columns in Excel worksheets using Java. Copy rows or columns within different Excel workbooks programmatically."
date: Tue, 15 Jun 2021 16:51:00 +0000
draft: false
url: /2021/06/15/copy-rows-and-columns-in-excel-using-java/
author: Usman Aziz
summary: 'In certain cases, you need to copy rows and columns in an Excel file without copying the entire worksheet. To perform this operation programmatically, this article covers **how to copy rows or columns in an Excel worksheet using Java**.'
tags: ['Copy Columns in Excel Worksheet using Java', 'Copy Rows in Excel Worksheet using Java', 'Java API to Copy Rows and Columns in Excel']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Excel-File.jpg" alt="Copy Rows and Columns in Excel using C#">}}


In certain cases, you need to copy rows and columns in an Excel file without copying the entire worksheet. To perform this operation programmatically, this article covers **how to copy rows or columns in an Excel worksheet using Java**.

*   [Java API to Copy Rows and Columns in Excel][1]
*   [Copy Rows in Excel Worksheet using Java][2]
*   [Copy Columns in Excel Worksheet using Java][3]

## Java API to Copy Rows and Columns in Excel {#API-to-Copy-Rows-and-Columns-in-Excel}

[Aspose.Cells for Java][4] lets you implement Excel automation features from within your Java applications. In addition, the API provides simple ways to copy rows and columns within or between the Excel workbooks. You can either [download][5] the API or install it using the following Maven configurations.

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
    <version>21.7</version>
</dependency>
```

## Copy Rows in Excel Worksheet using Java {#Copy-Rows-in-Excel-Worksheet}

The following are the steps to copy a row in an Excel worksheet using Java.

*   First, load the Excel file using [Workbook][6] class.
*   Get the desired [Worksheet][7] from [Workbook.getWorksheets()][8] collection.
*   Copy desired row by specifying the source and target row index in [Worksheet.getCells().copyRow(Workheet.getCells(), sourceRowIndex, targetRowIndex)][9] method.
*   Finally, save the updated Excel file using [Workbook.save(string)][10] method.

The following code sample shows how to copy a row in an Excel worksheet using Java.

{{< gist aspose-com-gists b6f33bfc3832977297cceccb0264743e "copy-rows.java" >}}

## Copy Columns in Excel Worksheet using Java {#Copy-Columns-in-Excel-Worksheet}

The following are the steps to copy a column in an Excel worksheet using Java.

*   First, load the Excel file using [Workbook][11] class.
*   Get the desired [Worksheet][12] from [Workbook.getWorksheets()][13] collection.
*   Copy desired column by specifying the source and target column index in [Worksheet.getCells().copyColumn(Cells, sourceColumnIndex, targetColumnIndex)][14] method.
*   Finally, save the updated Excel file using [Workbook.save(string)][15] method.

The following code sample shows how to copy a column in an Excel worksheet using Java.

{{< gist aspose-com-gists b6f33bfc3832977297cceccb0264743e "copy-columns.java" >}}

## Get a Free License {#Get-a-Free-License}

You can use Aspose.Cells for Java without evaluation limitations using a [temporary license][16].

## Conclusion

In this article, you have learned how to copy rows and columns in Excel worksheets using Java. Moreover, you can use the provided code samples to copy rows or columns within different Excel workbooks as well. In addition, you can explore the [documentation][17] of Aspose.Cells for Java. In case you would have any queries, feel free to post to our [forum][18].

## See Also

*   [Create MS Excel Files in Java without MS Office][19]




[1]: #API-to-Copy-Rows-and-Columns-in-Excel
[2]: #Copy-Rows-in-Excel-Worksheet
[3]: #Copy-Columns-in-Excel-Worksheet
[4]: https://products.aspose.com/cells/Java
[5]: https://downloads.aspose.com/cells/java
[6]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[7]: https://apireference.aspose.com/cells/java/com.aspose.cells/Worksheet
[8]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#Worksheets
[9]: https://apireference.aspose.com/cells/java/com.aspose.cells/cells#copyRow(com.aspose.cells.Cells,%20int,%20int)
[10]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String)
[11]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[12]: https://apireference.aspose.com/cells/java/com.aspose.cells/Worksheet
[13]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#Worksheets
[14]: https://apireference.aspose.com/cells/java/com.aspose.cells/cells#copyColumn(com.aspose.cells.Cells,%20int,%20int)
[15]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String)
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/cells/java
[18]: https://forum.aspose.com/
[19]: https://blog.aspose.com/2020/10/13/create-excel-xlsx-xls-using-java-without-ms-office/





