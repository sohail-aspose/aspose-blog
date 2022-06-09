---
title: 'Add or Modify VBA Macros in Excel Files using Java'
seoTitle: "Add or Modify Excel VBA Macro in Java | Java Excel API | Aspose"
description: "Use Java spreadsheet manipulation API to add or modiy VBA macro in Excel using Java. Access and manipulate the VBA modules attached to the worksheets."
date: Tue, 08 Jun 2021 07:53:02 +0000
draft: false
url: /2021/06/08/add-modify-vba-macros-in-excel-using-java/
author: Usman Aziz
summary: '[VBA][1] is a programming language used to automate various operations in MS Excel files. Particularly, VBA macros are user-defined codes that let you speed up the spreadsheet manipulation tasks. In this article, you will learn how to work with VBA macros in Excel files programmatically. Ultimately, you will be able to **add and modify VBA macros in Excel using Java**.'
tags: ['Add VBA Macros to an Excel Workbook', 'Modify VBA Macro in an Excel Workbook', 'Work with VBA Macros using Java API']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Work-with-VBA-Macros.jpg" alt="VBA Macro in Excel Java">}}


[VBA][2] is a programming language used to automate various operations in MS Excel files. Particularly, VBA macros are user-defined codes that let you speed up the spreadsheet manipulation tasks. In this article, you will learn how to work with VBA macros in Excel files programmatically. Ultimately, you will be able to **add and modify VBA macros in Excel using Java**.

*   [Work with VBA Macros using Java API][3]
*   [Add VBA Macros to an Excel Workbook][4]
*   [Modify VBA Macro in an Excel Workbook][5]

**TIP**

You may want to try Aspose [online VBA macro removal tool][6].

## Work with Excel VBA Macros using Java API {#Work-with-VBA-Macros-using-Java-API}

In order to work with VBA macros in Excel files, we will use [Aspose.Cells for Java][7]. It is a powerful spreadsheet automation API that lets you create, modify and convert Excel files. Furthermore, it simplifies the manipulation of VBA macros. You can either [download][8] the API or install it using the following Maven configurations.

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
    <version>21.5</version>
</dependency>
```

## Add VBA Macros to an Excel Workbook in Java {#Add-VBA-Macros-to-an-Excel-Workbook}

The following are the steps to add VBA macro in Excel files in Java.

*   First, load an existing workbook or create a new using [Workbook][9] class.
*   Fetch the worksheet into a [Worksheet][10] object using [Workbook.getWorksheets().get(index)][11] method.
*   Add a new VBA module using [Workbook.getVbaProject().getModules().add(Worksheet)][12] method.
*   Get the reference of the newly added module into [VbaModule][13] object.
*   Set name and code of the module using [VbaModule.setName()][14] and [VbaModule.setCodes()][15] methods, respectively.
*   Finally, save the workbook using [Workbook.save(string, SaveFormat.XLSM)][16] method.

The following code sample shows how to add a VBA macro in an Excel file using Java.

{{< gist aspose-com-gists 1d8519df9064d918a223e1278e9f0ff7 "add-vba-macro.java" >}}

## Modify VBA Macro in an Excel Workbook in Java {#Modify-VBA-Macro-in-an-Excel-Workbook}

The following are the steps to modify VBA macro in Excel files using Java.

*   First, load an existing workbook using the [Workbook][17] class.
*   Retrieve VBA module collection in a [VbaModuleCollection][18] object using [Workbook.getVbaProject().getModules()][19] method.
*   Fetch each VBA module from the collection into a [VbaModule][20] object iteratively.
*   Update name and code of the desired module using [VbaModule.setName()][21] and [VbaModule.setCodes()][22] methods respectively.
*   Finally, save the workbook using [Workbook.save(string, SaveFormat.XLSM)][23] method.

The following code sample shows how to modify the VBA macro in an Excel file using Java.

{{< gist aspose-com-gists 1d8519df9064d918a223e1278e9f0ff7 "modify-vba-macro.java" >}}

## Get a Free License {#Get-a-Free-License}

You can use Aspose.Cells for Java without evaluation limitations using a temporary license. [Get yours now][24].

## Conclusion

VBA macros are used to automate various types of tasks in spreadsheets. In order to work with VBA macros programmatically, this article covered how to add and modify code in VBA modules using Java. To learn more, you can explore [documentation][25] of Java spreadsheet manipulation API. Also, you can post your questions or queries on our [forum][26].

## See Also

*   [Create Excel Files using Java without MS Office][27]
*   [Convert Excel Files to PDF using Java][28]




[1]: https://en.wikipedia.org/wiki/Visual_Basic_for_Applications
[2]: https://en.wikipedia.org/wiki/Visual_Basic_for_Applications
[3]: #Work-with-VBA-Macros-using-Java-API
[4]: #Add-VBA-Macros-to-an-Excel-Workbook
[5]: #Modify-VBA-Macro-in-an-Excel-Workbook
[6]: https://products.aspose.app/slides/remove-macros
[7]: https://products.aspose.com/cells/java
[8]: https://downloads.aspose.com/cells/java
[9]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[10]: https://apireference.aspose.com/cells/java/com.aspose.cells/Worksheet
[11]: https://apireference.aspose.com/cells/java/com.aspose.cells/worksheetcollection#Item%20(int)
[12]: https://apireference.aspose.com/cells/java/com.aspose.cells/vbamodulecollection#add(com.aspose.cells.Worksheet)
[13]: https://apireference.aspose.com/cells/java/com.aspose.cells/VbaModule
[14]: https://apireference.aspose.com/cells/java/com.aspose.cells/vbamodule#Name
[15]: https://apireference.aspose.com/cells/java/com.aspose.cells/vbamodule#Codes
[16]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String,%20int)
[17]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[18]: https://apireference.aspose.com/cells/java/com.aspose.cells/VbaModuleCollection
[19]: https://apireference.aspose.com/cells/java/com.aspose.cells/vbaproject#Modules
[20]: https://apireference.aspose.com/cells/java/com.aspose.cells/VbaModule
[21]: https://apireference.aspose.com/cells/java/com.aspose.cells/vbamodule#Name
[22]: https://apireference.aspose.com/cells/java/com.aspose.cells/vbamodule#Codes
[23]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String,%20int)
[24]: https://purchase.aspose.com/temporary-license
[25]: https://docs.aspose.com/cells/java/developer-guide/
[26]: https://forum.aspose.com/
[27]: https://blog.aspose.com/2020/10/13/create-excel-xlsx-xls-using-java-without-ms-office/
[28]: https://blog.aspose.com/2020/08/12/convert-excel-to-pdf-using-java/





