---
title: 'Protect and Unprotect Excel Files in Java'
seoTitle: "Protect or Unprotect Excel Files in Java | Protect Unprotect Worksheets"
description: "Protect and unprotect Excel files using Java. Apply different protection types on whole Excel workbook or a particular worksheet using Java Excel API."
date: Mon, 11 Jan 2021 17:34:22 +0000
draft: false
url: /2021/01/11/Protect-Unprotect-Excel-Files-in-Java/
author: Usman Aziz
summary: 'Excel files are used to store small as well as large-sized data in the form of rows and columns. Along with data storage, you can perform other operations such as computations and data analysis using graphs and charts. Since data is worth being protected, MS Excel allows you to protect the Excel files. This article covers how to automate the protection of MS Excel files programmatically. Particularly, you will learn **how to protect and unprotect Excel files using Java**.'
tags: ['Java-API-to-Protect-Excel-Files', 'Protect-Excel-Files-using-Java', 'Protect-Worksheets-using-Java', 'Unprotect-Excel-Files-using-Java', 'Unprotect-Worksheets-using-Java']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Protect-Excel-Files-C.jpg" alt="Protect Excel Files in Java">}}


Excel files are used to store small as well as large-sized data in the form of rows and columns. Along with data storage, you can perform other operations such as computations and data analysis using graphs and charts. Since data is worth being protected, MS Excel allows you to protect the Excel files. This article covers how to automate the protection of MS Excel files programmatically. Particularly, you will learn **how to protect and unprotect Excel files using Java**.

*   [Java API to Protect Excel Files][1]
*   [Protect Excel Files using Java][2]
*   [Unprotect Excel Files using Java][3]
*   [Protect Worksheets using Java][4]
*   [Unprotect Worksheets using Java][5]
*   [Get Free License][6]

## Java API to Protect Excel Files {#Java-API-to-Protect-Excel-Files}

[Aspose.Cells for Java][7] is a well-known spreadsheet manipulation API that is designed to create, edit, and convert Excel files from within the Java applications. Along with other basic as well as advanced Excel automation features, Aspose.Cells supports the protection of the Excel files. You can either [download][8] API's JAR or install it using the following Maven configuration.

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
    <version>20.12</version>
</dependency>
```

## Protect Excel Files using Java {#Protect-Excel-Files-using-Java}

Aspose.Cells for Java provides the following protection types in order to protect the Excel workbooks.

*   [**ALL**][9] - User cannot modify anything
*   [**CONTENTS**][10] - User cannot enter data
*   [**OBJECTS**][11] - User cannot modify drawing objects
*   [**SCENARIOS**][12] - User cannot modify saved scenarios
*   [**STRUCTURE**][13] - User cannot modify saved structure
*   [**WINDOWS**][14] - User cannot modify saved windows
*   [**NONE**][15] - No protection

The following are the steps to protect an Excel file using Aspose.Cells for Java.

*   Load Excel file using [Workbook][16] class.
*   Use [Workbook.protect(ProtectionType, String)][17] method to protect the Excel file.
*   Save the protected file using [Workbook.save(String)][18] method.

The following code sample shows how to protect an Excel file in Java.

{{< gist aspose-com-gists 647605e64f8abf8046f2c257f8d9ec4a "protect-workbook.java" >}}

## Unprotect Excel Files using Java {#Unprotect-Excel-Files-using-Java}

The following are the steps to unprotect a password-protected Excel file using Aspose.Cells for Java.

*   Load Excel file using [Workbook][19] class.
*   Use [Workbook.unprotect(String)][20] method to unprotect the Excel file.
*   Save the unprotected Excel file using [Workbook.save(String)][21] method.

The following code sample shows how to unprotect an Excel file in Java.

{{< gist aspose-com-gists 647605e64f8abf8046f2c257f8d9ec4a "unprotect-workbook.java" >}}

## Protect Excel Worksheets using Java {#Protect-Worksheets-using-Java}

You can also apply protection at worksheet level. The following are the steps to protect an Excel worksheet using Aspose.Cells for Java.

*   Load Excel file using [Workbook][22] class.
*   Get the specific worksheet in a [Worksheet][23] object using [Workbook.getWorksheets().get(int)][24] method.
*   Get the worksheet protection settings into the [Protection][25] object using [Worksheet.getProtection()][26] method.
*   Set password using [Protection.setPassword(String)][27] method.
*   Save the Excel file using [Workbook.save(String)][28] method.

The following code sample shows how to protect an Excel worksheet using Java.

{{< gist aspose-com-gists 647605e64f8abf8046f2c257f8d9ec4a "protect-worksheet.java" >}}

## Unprotect Worksheets using Java {#Unprotect-Worksheets-using-Java}

The procedure of unprotecting a worksheet is same as protecting one. The only difference is, you will use the [Worksheet.unprotect(String)][29] method. The following code sample shows how to unprotect an Excel worksheet using Java.

{{< gist aspose-com-gists 647605e64f8abf8046f2c257f8d9ec4a "unprotect-worksheet.java" >}}

## Get a Free License {#Get-Free-License}

You can [get a free temporary license][30] in order to try the APIs without evaluation limitations.

## Conclusion

In this article, you have learned how to protect and unprotect Excel files using Java. Furthermore, you have seen how to protect and unprotect a particular worksheet in an Excel workbook. You can explore more about the Java Excel automation API using [documentation][31].

## See Also

*   [Create MS Excel Files using Java without MS Office][32]




[1]: #Java-API-to-Protect-Excel-Files
[2]: #Protect-Excel-Files-using-Java
[3]: #Unprotect-Excel-Files-using-Java
[4]: #Protect-Worksheets-using-Java
[5]: #Unprotect-Worksheets-using-Java
[6]: #Get-Free-License
[7]: http://products.aspose.com/cells/java
[8]: http://downloads.aspose.com/cells/java
[9]: https://apireference.aspose.com/cells/java/com.aspose.cells/protectiontype#ALL
[10]: https://apireference.aspose.com/cells/java/com.aspose.cells/protectiontype#CONTENTS
[11]: https://apireference.aspose.com/cells/java/com.aspose.cells/protectiontype#OBJECTS
[12]: https://apireference.aspose.com/cells/java/com.aspose.cells/protectiontype#SCENARIOS
[13]: https://apireference.aspose.com/cells/java/com.aspose.cells/protectiontype#STRUCTURE
[14]: https://apireference.aspose.com/cells/java/com.aspose.cells/protectiontype#WINDOWS
[15]: https://apireference.aspose.com/cells/java/com.aspose.cells/protectiontype#NONE
[16]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[17]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#protect(int,%20java.lang.String)
[18]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String)
[19]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[20]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#unprotect(java.lang.String)
[21]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String)
[22]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[23]: https://apireference.aspose.com/cells/java/com.aspose.cells/worksheet
[24]: https://apireference.aspose.com/cells/java/com.aspose.cells/worksheetcollection#Item%20(int)
[25]: https://apireference.aspose.com/cells/java/com.aspose.cells/protection
[26]: https://apireference.aspose.com/cells/java/com.aspose.cells/worksheet#Protection
[27]: https://apireference.aspose.com/cells/java/com.aspose.cells/protection#Password
[28]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String)
[29]: https://apireference.aspose.com/cells/java/com.aspose.cells/worksheet#unprotect(java.lang.String)
[30]: https://purchase.aspose.com/temporary-license
[31]: https://docs.aspose.com/cells/java/developer-guide/
[32]: https://blog.aspose.com/2020/10/13/create-excel-xlsx-xls-using-java-without-ms-office/





