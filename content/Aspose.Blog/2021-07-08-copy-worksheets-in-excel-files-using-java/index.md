---
title: 'Copy or Move Worksheets in Excel Files using Java'
seoTitle: "Java Copy and Move Excel Worksheets | Aspose.Cells for Java"
description: "Use Java Excel API to copy or move worksheets in Excel workbooks using Java. Copy worksheet within a workbook or from another workbook."
date: Thu, 08 Jul 2021 14:12:38 +0000
draft: false
url: /2021/07/08/copy-worksheets-in-excel-files-using-java/
author: Usman Aziz
summary: 'You may often need to copy worksheets within an Excel workbook or from one workbook to another. Also, changing the position of the worksheets is also required in certain cases. In order to perform the above-mentioned tasks programmatically, this article shows **how to copy worksheets within Excel workbooks using Java**. Furthermore, it also covers **how to move a worksheet in an Excel workbook**.'
tags: ['Copy Worksheets from One Workbook to Another Java', 'Copy Worksheets within an Excel Workbook Java', 'Java API to Copy Excel Worksheets', 'Move Worksheets from One Position to Another Java']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Copy-Worksheets.jpg" alt="Copy Worksheets in Excel Files using Java">}}


You may often need to copy worksheets within an Excel workbook or from one workbook to another. Also, changing the position of the worksheets is also required in certain cases. In order to perform the above-mentioned tasks programmatically, this article shows **how to copy worksheets within Excel workbooks using Java**. Furthermore, it also covers **how to move a worksheet in an Excel workbook**.

*   [Java API to Copy Excel Worksheets][1]
*   [Copy Worksheets within an Excel Workbook][2]
*   [Copy Worksheets from One Workbook to Another][3]
*   [Move Worksheets from One Position to Another][4]

## Java API to Copy or Move Excel Worksheets {#Java-API-to-Copy-Excel-Worksheets}

In order to copy or move the worksheets in Excel files, we'll use [Aspose.Cells for Java][5]. It is a feature-rich API that lets you create or modify spreadsheet documents quite easily. You can either [download][6] the API or install it using the following Maven configurations.

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

## Copy Worksheets within an Excel Workbook in Java {#Copy-Worksheets-within-an-Excel-Workbook}

The following are the steps to copy a worksheet in an Excel workbook using Java.

1.  Load Excel file using [Workbook][7] class.
2.  Retrieve worksheets in a [WorksheetCollection][8] object using [Workbook.getWorksheets()][9] method.
3.  Use [WorksheetCollection.addCopy(String)][10] method to copy the worksheet by providing its name.
4.  Save the updated workbook using [Workbook.save(String)][11] method.

The following code sample shows how to copy or clone a worksheet in an Excel workbook.

{{< gist aspose-com-gists 719efcb90f9408835ed72a0d8625d033 "copy-worksheet.java" >}}

## Copy Worksheets from One Workbook to Another {#Copy-Worksheets-from-One-Workbook-to-Another}

You can also copy a worksheet from one Excel workbook to another. The following are the steps to make a clone of a worksheet in one workbook and add it to another.

1.  Create an object of the [Workbook][12] class and load the source Excel file.
2.  Create another object of the [Workbook][13] class and load the destination Excel file.
3.  Copy worksheet from source to destination workbook using [Workbook.getWorksheets().get(int).copy(sourceWorkbook.getWorksheets().get(int))][14] method.
4.  Save the destination workbook using [Workbook.save(String)][15] method.

The following code sample shows how to clone a worksheet from one Excel workbook to another in Java.

{{< gist aspose-com-gists 719efcb90f9408835ed72a0d8625d033 "copy-worksheets-in-workbooks.java" >}}

## Move Worksheets from One Position to Another in Java {#Move-Worksheets-from-One-Position-to-Another-in-Java}

The following are the steps to move a worksheet from one position to another in Java.

1.  Load Excel file using [Workbook][16] class.
2.  Retrieve worksheets in a [WorksheetCollection][17] object using [Workbook.getWorksheets()][18] method.
3.  Access the desired worksheet from worksheet collection into a [Worksheet][19] object.
4.  Use [Worksheet.moveTo(int)][20] method to move the worksheet to the specified index.
5.  Save the updated workbook using [Workbook.save(string)][21] method.

The following code sample shows how to move a worksheet from one position to another in Java.

{{< gist aspose-com-gists 719efcb90f9408835ed72a0d8625d033 "move-worksheet.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try and evaluate Aspose.Cells for Java for free by requesting a [temporary license][22].

## Conclusion

In this article, you have learned how to copy worksheets in Excel workbooks using Java. Furthermore, you have seen how to move a worksheet from one position to another within an Excel workbook. You can explore other features of Aspose.Cells for Java using the [documentation][23]. In case you would have any queries, feel free to post to our [forum][24].

## See Also

*   [Create Excel Files using Java without MS Office][25]




[1]: #Java-API-to-Copy-Excel-Worksheets
[2]: #Copy-Worksheets-within-an-Excel-Workbook
[3]: #Copy-Worksheets-from-One-Workbook-to-Another
[4]: #Move-Worksheets-from-One-Position-to-Another-in-Java
[5]: https://products.aspose.com/cells/java
[6]: https://downloads.aspose.com/cells/java
[7]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[8]: https://apireference.aspose.com/cells/java/com.aspose.cells/WorksheetCollection
[9]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#Worksheets
[10]: https://apireference.aspose.com/cells/java/com.aspose.cells/worksheetcollection#addCopy(int)
[11]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String)
[12]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[13]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[14]: https://apireference.aspose.com/cells/java/com.aspose.cells/worksheet#copy(com.aspose.cells.Worksheet)
[15]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String)
[16]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[17]: https://apireference.aspose.com/cells/java/com.aspose.cells/WorksheetCollection
[18]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#Worksheets
[19]: https://apireference.aspose.com/cells/java/com.aspose.cells/Worksheet
[20]: https://apireference.aspose.com/cells/java/com.aspose.cells/worksheet#moveTo(int)
[21]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String)
[22]: https://purchase.aspose.com/temporary-license
[23]: https://docs.aspose.com/cells/java
[24]: https://forum.aspose.com/
[25]: https://blog.aspose.com/2020/10/13/create-excel-xlsx-xls-using-java-without-ms-office/





