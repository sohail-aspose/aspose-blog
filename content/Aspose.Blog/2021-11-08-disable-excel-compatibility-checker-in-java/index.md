---
title: 'Disable Compatibility Checker in Excel Files using Java'
seoTitle: "Disable Compatibility Checker in Excel in Java | Java Excel Library"
description: "Use Java Excel library to enable or disable compatibility checker in XLSX/XLS in Java. Turn the MS Excel compatibility mode on/off dynamically."
date: Mon, 08 Nov 2021 13:29:00 +0000
draft: false
url: /2021/11/08/disable-excel-compatibility-checker-in-java/
author: Usman Aziz
summary: 'Various versions of MS Excel are available and being used around the world. This makes it possible that the newer versions provide features that may not be available in the older ones. Therefore, MS Excel uses compatibility checker to degrade the features which are not supported by an older format when saving the files. While manipulating Excel files, you may need to disable the compatibility checker dynamically. To achieve it, this article shows **how to disable the compatibility checker for MS Excel workbooks in Java**.'
tags: ['Java Library for Excel Compatibility Checker', 'disable compatibility checker in Excel in Java', 'disable compatibility checker in xls in Java', 'disable compatibility checker in xlsx in Java']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Excel-File.jpg" alt="Enable or Disable Excel Compatibility Checker in Java">}}


Various versions of MS Excel are available and being used around the world. This makes it possible that the newer versions provide features that may not be available in the older ones. Therefore, MS Excel uses compatibility checker to degrade the features which are not supported by an older format when saving the files. While manipulating Excel files, you may need to disable the compatibility checker dynamically. To achieve it, this article shows **how to disable the compatibility checker for MS Excel workbooks in Java**.

*   [Java Library for Excel Compatibility Checker][1]
*   [Disable Compatibility Checker in Excel Files][2]

## Java Library to Disable Compatibility Checker in Excel {#Library-for-Excel-Compatibility-Checker}

[Aspose.Cells for Java][3] provides a wide range of features for spreadsheet manipulation. Using the API, you can create new spreadsheet documents from scratch and manipulate the existing ones. We will use this API to disable the compatibility checker for Excel files. You can download the API’s [JAR][4] or install it using the following Maven configurations.

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

## Disable Compatibility Checker in Excel Files {#Enable-or-Disable-Excel-Compatibility-Checker}

In order to disable the compatibility checker for an Excel workbook, you need to update the workbook's settings. The following are the steps to perform this operation.

*   First, load the Excel file using [Workbook][5] class.
*   Then, disable compatibility checker using [Workbook.getSettings().setCheckCompatibility(boolean)][6] method (set true and false to enable and disable checker, respectively).
*   Finally, save the updated workbook using [Workbook.save(string)][7] method.

The following code sample shows how to disable the compatibility checker using Java.

{{< gist aspose-com-gists 94d43731515ef2098a378472f60777d9 "disable-excel-compatibility-checker.java" >}}

## Get a Free License {#Get-a-Free-License}

You can use Aspose.Cells for Java without evaluation limitations using a [temporary license][8].

## Conclusion

MS Excel compatibility checker allows the users to create documents that can be viewed by everyone without compatibility issues. While working with Excel files programmatically, you may need to disable compatibility checker. Therefore, in this article, you have learned how to enable or disable compatibility checker for Excel files using Java. Besides, you can also explore other features of Aspose.Cells for Java using the [documentation][9]. In case you would have any queries, you can post on our [forum][10].

## See Also

*   [Create Excel Files using Java without MS Office][11]




[1]: #Library-for-Excel-Compatibility-Checker
[2]: #Enable-or-Disable-Excel-Compatibility-Checker
[3]: https://products.aspose.com/cells/java/
[4]: https://downloads.aspose.com/cells/java
[5]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[6]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbooksettings#CheckCompatibility
[7]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String)
[8]: https://purchase.aspose.com/temporary-license
[9]: https://docs.aspose.com/cells/java/
[10]: https://forum.aspose.com/
[11]: https://blog.aspose.com/2020/10/13/create-excel-xlsx-xls-using-java-without-ms-office/




