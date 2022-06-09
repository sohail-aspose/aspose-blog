---
title: 'Split Text to Columns in Excel using Java'
seoTitle: "Java: Split Text to Column in Excel | Split Text into Multiple Columns"
description: "Use Java Excel API to split text to column in Excel using Java. Split text in one column into multiple columns programmatically in Java."
date: Tue, 25 May 2021 09:50:00 +0000
draft: false
url: /2021/05/25/split-text-to-columns-in-excel-using-java/
author: Usman Aziz
summary: "MS Excel provides the Text to Columns feature to split the text into multiple columns. The splitting can be based on a blank space, a comma, a special character, etc. In order to automate the feature, this article covers **how to perform Excel's Text to Columns from within your Java applications**. The step-by-step guide and code sample will show you how to split text in a column in an Excel worksheet."
tags: ['Excel Text to Column Java', 'Java API to Split Text to Column in Excel', 'Split Text to Column in Excel using Java']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Text-to-Column-Java.jpg" alt="Excel Text to Column Java">}}


MS Excel provides the Text to Columns feature to split the text into multiple columns. The splitting can be based on a blank space, a comma, a special character, etc. In order to automate the feature, this article covers **how to perform Excel's Text to Columns from within your Java applications**. The step-by-step guide and code sample will show you how to split text in a column in an Excel worksheet.

*   [API to Split Text to Columns in Excel][1]
*   [Split Text to Columns in Excel][2]

## Java API to Split Text to Columns in Excel {#Java-API-to-Split-Text-to-Column-in-Excel}

In order to split the text into columns in Excel worksheets, we'll use [Aspose.Cells for Java][3]. It is a powerful API that lets you create, process, and convert Excel files from within your Java applications. You can either [download][4] the API or install it using the following Maven configurations.

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
    <version>21.6</version>
</dependency>
```

## Split Text to Columns in Excel using Java {#Split-Text-to-Column-in-Excel-using-Java}

The following are the steps to split text to columns in Excel using Java.

*   Load the Excel file using the [Workbook][5] class.
*   Get the reference to the worksheet where you want to split the text.
*   Add values to the cells (optional).
*   Create an instance of [TxtLoadOptions][6] class and specify the splitting character using [TxtLoadOptions.setSeparator(value)][7] method.
*   Split text to columns using [Worksheet.getCells().textToColumns(int row, int column, int totalRows, TxtLoadOptions options)][8] method.
*   Save the Excel file using [Workbook.save(fileName, SaveFormat.XLSX)][9] method.

The following code sample shows how to split text to columns in an Excel worksheet.

{{< gist aspose-com-gists 05b1407519b4ee653792fc456bb06506 "text-to-column.java" >}}

### Output



{{< figure align=center src="images/Text-to-Column-in-Excel.jpg" alt="Excel Text to Column Python">}}


## Get a Free API License {#Get-a-Free-API-License}

You can [get a temporary license][10] in order to use the API without evaluation limitations.

## Conclusion

In this article, you have learned how to implement Excel's text to columns feature using Java. The code sample has shown you how to split the text in a column into multiple columns within a few steps. You can explore more about Aspose.Cells for Java using the [documentation][11]. In case you would have any queries, contact us via our [forum][12].

## See Also

*   [Create Excel Files using Java without MS Office][13]




[1]: #Java-API-to-Split-Text-to-Column-in-Excel
[2]: #Split-Text-to-Column-in-Excel-using-Java
[3]: https://products.aspose.com/cells/java
[4]: https://downloads.aspose.com/cells/java
[5]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[6]: https://apireference.aspose.com/cells/java/com.aspose.cells/TxtLoadOptions
[7]: https://apireference.aspose.com/cells/java/com.aspose.cells/txtloadoptions#Separator
[8]: https://apireference.aspose.com/cells/java/com.aspose.cells/cells#textToColumns(int,%20int,%20int,%20com.aspose.cells.TxtLoadOptions)
[9]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String,%20int)
[10]: https://purchase.aspose.com/temporary-license
[11]: https://docs.aspose.com/cells/java
[12]: https://forum.aspose.com/
[13]: https://blog.aspose.com/2020/10/13/create-excel-xlsx-xls-using-java-without-ms-office/





