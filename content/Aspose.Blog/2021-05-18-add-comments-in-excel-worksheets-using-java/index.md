---
title: 'Add Comments in Excel Worksheets using Java'
seoTitle: "Add Comments in Excel using Java | Format Comments in Cells"
description: "Use Java Excel API to add comments to the Excel worksheets using Java. Format the cell comments in Excel worksheets programmatically using Java."
date: Tue, 18 May 2021 15:17:00 +0000
draft: false
url: /2021/05/18/add-comments-in-excel-worksheets-using-java/
author: Usman Aziz
summary: 'Comments are used to add additional information or to explain a formula in the Excel worksheet. MS Excel also allows you to set the font size, height, width, etc. of the comments. In this article, you will learn **how to add comments to the Excel worksheets programmatically using Java**. Furthermore, the article will also cover how to format the comments.'
tags: ['Add Comments in Excel Worksheets Java', 'Format Comment in Excel Java', 'Java Excel API']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Add-Comments-in-Excel.jpg" alt="Add Comments in Excel Worksheet Java">}}


Comments are used to add additional information or to explain a formula in the Excel worksheet. MS Excel also allows you to set the font size, height, width, etc. of the comments. In this article, you will learn **how to add comments to the Excel worksheets programmatically using Java**. Furthermore, the article will also cover how to format the comments.

*   [API to Add Comments in Excel][1]
*   [Add Comments in an Excel Worksheet][2]
*   [Apply Formatting to Comments in Excel][3]

## Java API to Add Comments in Excel {#API-to-Add-or-Format-Comments-in-Excel}

In order to add comments to the cells in Excel worksheets, we will use [Aspose.Cells for Java][4]. The API lets you create, modify, and convert Excel files from within your Java applications. You can either [download][5] the API or install it using the following Maven configurations.

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

## Add Comments to an Excel Worksheet in Java {#Add-Comments-in-an-Excel-Worksheet}

The following are the steps to add a comment to a cell in an Excel worksheet using Java.

*   Load the Excel file using [Workbook][6] class.
*   Get reference of the desired [Worksheet][7] using [Workbook.getWorksheets().get(index)][8] method.
*   Add comment to the cell using [Worksheet.getComments().add(string cellName)][9] method and get the reference of the comment in a [Comment][10] object.
*   Set comment's note using [Comment.setNote()][11] method.
*   Save the updated Excel file using [Workbook.save(string)][12] method.

The following code sample shows how to add a comment in an Excel worksheet using Java.

{{< gist aspose-com-gists 292bd31bdac961d2ced4eb8547c73b3b "add-comment-in-worksheet.java" >}}

## Apply Formatting to Comments in Excel {#Apply-Formatting-to-Comments-in-Excel}

The following are the steps to apply formatting to the comments in Excel using Java.

*   Load the Excel file using [Workbook][13] class.
*   Get reference of the desired [Worksheet][14] using [Workbook.getWorksheets().get(index)][15] method.
*   Add comment to the cell using [Worksheet.getComments().add(string cellName)][16] method and get the reference of the comment in a [Comment][17] object.
*   Set comment's note using [Comment.setNote()][18] method.
*   Set the desired formatting of the comment using Comment object.
*   Save the updated Excel file using [Workbook.save(string)][19] method.

The following code sample shows how to set formatting of the comments in Excel.

{{< gist aspose-com-gists 292bd31bdac961d2ced4eb8547c73b3b "format-comment-in-worksheet.java" >}}

## Get a Free License {#Get-a-Free-License}

You can use Aspose.Cells for Java without evaluation limitations using a [temporary license][20].

## Conclusion

In this article, you have learned how to add comments to the cells in Excel worksheets using Java. Furthermore, you have seen how to apply formatting to the comments programmatically. You can visit the [documentation][21] to explore other features of Aspose.Cells for Java. In case you would have any queries, feel free to post to our [forum][22].

## See Also

*   [Generate Excel Files without MS Office using Java][23]




[1]: #API-to-Add-or-Format-Comments-in-Excel
[2]: #Add-Comments-in-an-Excel-Worksheet
[3]: #Apply-Formatting-to-Comments-in-Excel
[4]: https://products.aspose.com/cells/java
[5]: https://downloads.aspose.com/cells/java
[6]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[7]: https://apireference.aspose.com/cells/java/com.aspose.cells/Worksheet
[8]: https://apireference.aspose.com/cells/java/com.aspose.cells/worksheetcollection#Item%20(int)
[9]: https://apireference.aspose.com/cells/java/com.aspose.cells/commentcollection#add(java.lang.String)
[10]: https://apireference.aspose.com/cells/java/com.aspose.cells/Comment
[11]: https://apireference.aspose.com/cells/java/com.aspose.cells/comment#Note
[12]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String)
[13]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[14]: https://apireference.aspose.com/cells/java/com.aspose.cells/Worksheet
[15]: https://apireference.aspose.com/cells/java/com.aspose.cells/worksheetcollection#Item%20(int)
[16]: https://apireference.aspose.com/cells/java/com.aspose.cells/commentcollection#add(java.lang.String)
[17]: https://apireference.aspose.com/cells/java/com.aspose.cells/Comment
[18]: https://apireference.aspose.com/cells/java/com.aspose.cells/comment#Note
[19]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String)
[20]: https://purchase.aspose.com/temporary-license
[21]: https://docs.aspose.com/cells/java
[22]: https://forum.aspose.com/
[23]: https://blog.aspose.com/2020/10/13/create-excel-xlsx-xls-using-java-without-ms-office/





