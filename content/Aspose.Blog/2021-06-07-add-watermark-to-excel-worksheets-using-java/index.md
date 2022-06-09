---
title: 'Add Watermark to Excel Worksheets using Java'
seoTitle: "Add Watermark to Excel Worksheet in Java | Java Excel API by Aspose"
description: "Use Java Excel API to add watermark to Excel worksheets using Java. Source code to customize the locking properties of the watermark."
date: Mon, 07 Jun 2021 16:54:00 +0000
draft: false
url: /2021/06/07/add-watermark-to-excel-worksheets-using-java/
author: Usman Aziz
summary: 'Watermarks are used to define the ownership of the copyrighted content and protect the Excel files from theft or being used illegally. In this article, you will learn how to add watermarks to Excel sheets programmatically. More precisely, the article will cover **how to add watermark to Excel worksheets using Java**.'
tags: ['Add a Watermark to Excel Worksheet', 'Java API to Add Watermarks to Excel Files']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Add-Watermark-to-Excel-Sheets.jpg" alt="Add Watermark to Excel Sheet Java">}}


Watermarks are used to define the ownership of the copyrighted content and protect the Excel files from theft or being used illegally. In this article, you will learn how to add watermarks to Excel sheets programmatically. More precisely, the article will cover **how to add watermark to Excel worksheets using Java**.

*   [Java API to Add Watermarks to Excel Worksheets][1]
*   [Add Watermark to an Excel Worksheet][2]

## Java API to Add Watermarks to Excel Worksheets {#API-to-Add-Watermarks-to-Excel-Files}

In order to add watermark to Excel files, we will use [Aspose.Cells for Java][3]. The API allows you to create, modify or convert Excel files from within the Java applications. You can either [download][4] the API's JAR or install it using the following Maven configurations.

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

## Add Watermark to an Excel Worksheet in Java {#Add-a-Watermark-to-Excel-Worksheet}

The following are the steps to add a watermark in an Excel worksheet using Java.

*   First, load the Excel file using [Workbook][5] class by providing its path.
*   Get reference of the [Worksheet][6] to which you want to add the watermark.
*   Create a watermark by adding a new [Shape][7] to the worksheet and set the its text and properties.
*   Set [Shape.setLocked(boolean)][8] property to true to lock the watermark.
*   Set other lock types using [Shape.setLockedProperty(ShapeLockType, boolean)][9] method.
*   Finally, save the updated Excel file using [Workbook.save(String)][10] method.

The following code sample shows how to add a watermark to an Excel worksheet.

{{< gist aspose-com-gists 7ba1fc8dc4c8cf93eadb60dfba54ce0b "add-watermark-to-Excel.java" >}}

### Output

The following is the screenshot of the Excel worksheet after adding the watermark.



{{< figure align=center src="images/Add-Watermark-to-Excel-Worksheet.jpg" alt="Adding Watermark in Excel Worksheet">}}


## Get a Free License {#Get-a-Free-License}

You can use Aspose.Cells for Java without evaluation limitations using a [temporary license][11].

## Conclusion

In this article, you have learned how to add watermark to Excel worksheets using Java. The provided code sample can easily be integrated into the Java applications. You can also explore other features of Aspose.Cells for Java using the [documentation][12]. In case you would have any queries, you can post on our [forum][13].

## See Also

*   [Create Excel Files using Java without MS Office][14]
*   [Protect Excel Files in Java][15]




[1]: #API-to-Add-Watermarks-to-Excel-Files
[2]: #Add-a-Watermark-to-Excel-Worksheet
[3]: https://products.aspose.com/cells/java
[4]: https://downloads.aspose.com/cells/java
[5]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[6]: https://apireference.aspose.com/cells/java/com.aspose.cells/Worksheet
[7]: https://apireference.aspose.com/cells/java/com.aspose.cells/Shape
[8]: https://apireference.aspose.com/cells/java/com.aspose.cells/shape#IsLocked
[9]: https://apireference.aspose.com/cells/java/com.aspose.cells/shape#setLockedProperty(int,%20boolean)
[10]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String)
[11]: https://purchase.aspose.com/temporary-license
[12]: https://docs.aspose.com/cells/java
[13]: https://forum.aspose.com/
[14]: https://blog.aspose.com/2020/10/13/create-excel-xlsx-xls-using-java-without-ms-office/
[15]: https://blog.aspose.com/2021/01/11/Protect-Unprotect-Excel-Files-in-Java/





