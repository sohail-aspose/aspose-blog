---
title: 'Find and Replace Text in Excel Spreadsheets using Java'
seoTitle: "Find and Replace Text in Excel in Java | Replace Text in XLSX with Regex"
description: "Find and replace text in Excel spreadsheets using Java. Replace text with plain text or regular expression in Excel workbooks from within Java applications."
date: Tue, 08 Dec 2020 23:02:52 +0000
draft: false
url: /2020/12/08/find-and-replace-text-in-spreadsheets-using-java/
author: Usman Aziz
summary: "In this post, you will learn **how to find and replace text in MS Excel spreadsheets programmatically in Java**. In various scenarios, MS Excel spreadsheets consist of a huge amount of data that may spread in multiple sheets. For such cases, the find and replace option could help you minimize the efforts required to update all the occurrences of a particular piece of text. Let's check out how to automate this option when dealing with a large number of spreadsheets from within the Java applications."
tags: ['Java Excel API', 'find and replace text in excel in java', 'find and replace text in excel with regex']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Find-and-Replace-Text-in-Excel.png" alt="find and replace text in excel java">}}


In this post, you will learn **how to find and replace text in MS Excel spreadsheets programmatically in Java**. In various scenarios, MS Excel spreadsheets consist of a huge amount of data that may spread in multiple sheets. For such cases, the find and replace option could help you minimize the efforts required to update all the occurrences of a particular piece of text. Let's check out how to automate this option when dealing with a large number of spreadsheets from within the Java applications.

*   [Java API to Find and Replace Text in Excel Files][1]
*   [Find and Replace Text in Excel File][2]
*   [Find and Replace Text using Regular Expression][3]

## Java API to Find and Replace Text in Excel Files {#Java-API-to-Find-and-Replace-Text-in-Excel-Files}

[Aspose.Cells for Java][4] is a powerful spreadsheet manipulation API that lets you create new and process existing Excel documents. The Excel automation features provided by the API also include finding and replacing the text seamlessly. You can either [download][5] the API or install it within your Maven-based applications for free.

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
    <version>20.11</version>
</dependency>
```

## Find and Replace Text in Excel using Java {#Find-and-Replace-Text-in-Excel-File}

The following are the steps of how to find and replace text in Excel spreadsheets.

*   Load the Excel file using [Workbook][6] class.
*   Create an instance of [ReplaceOptions][7] class.
*   Enable case sensitive search using [ReplaceOptions.setCaseSensitive(boolean)][8] method.
*   Set option for text matching with entire cell's content using [ReplaceOptions.setMatchEntireCellContents(boolean)][9] method.
*   Find and replace text using [Workbook.replace(String, String, ReplaceOptions)][10] method.
*   Save the updated spreadsheet using [Workbook.save(String)][11] method.

The following code sample shows how to find and replace a text in an Excel spreadsheet.

{{< gist aspose-com-gists 931e04bc25e66a77c5487d4cdb65e49b "find-replace-text-in-Excel.java" >}}

## Find and Replace Text in Excel using Regular Expression {#Find-and-Replace-Text-using-Regular-Expression}

You can also use regular expressions in order to find and replace text in the spreadsheets. The only difference in code is, you will enable the regex search and provide regex instead of plain text in _Workbook.replace_ method. The following are the steps to perform find and replace operation using regex.

*   Load the Excel file using [Workbook][12] class.
*   Create an instance of [ReplaceOptions][13] class.
*   Enable regex search using [ReplaceOptions.setRegexKey(true)][14] method.
*   Find and replace text using [Workbook.replace(String, String, ReplaceOptions)][15] method.
*   Save the updated spreadsheet using [Workbook.save(String)][16] method.

The following code sample shows how to find and replace text in spreadsheets using regex.

{{< gist aspose-com-gists 931e04bc25e66a77c5487d4cdb65e49b "find-replace-text-in-Excel-regex.java" >}}

## Conclusion

Excel automation has become a widely adopted feature in various business domains. In accordance with that, in this post, you have learned one of the basic yet important features of spreadsheet manipulation. The step by step guide and code samples have shown you how to find and replace text in Excel files using Java. In case you want to learn about the advanced features of the API, you can explore the [documentation][17].

## See Also

*   [Create MS Excel Files using Java without MS Office][18]




[1]: #Java-API-to-Find-and-Replace-Text-in-Excel-Files
[2]: #Find-and-Replace-Text-in-Excel-File
[3]: #Find-and-Replace-Text-using-Regular-Expression
[4]: https://products.aspose.com/cells/java
[5]: https://downloads.aspose.com/cells/java
[6]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook
[7]: https://apireference.aspose.com/cells/java/com.aspose.cells/ReplaceOptions
[8]: https://apireference.aspose.com/cells/java/com.aspose.cells/replaceoptions#IsCaseSensitive
[9]: https://apireference.aspose.com/cells/java/com.aspose.cells/replaceoptions#MatchEntireCellContents
[10]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#replace(java.lang.String,%20java.lang.String,%20com.aspose.cells.ReplaceOptions)
[11]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String)
[12]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook
[13]: https://apireference.aspose.com/cells/java/com.aspose.cells/ReplaceOptions
[14]: https://apireference.aspose.com/cells/java/com.aspose.cells/replaceoptions#RegexKey
[15]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#replace(java.lang.String,%20java.lang.String,%20com.aspose.cells.ReplaceOptions)
[16]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String)
[17]: https://docs.aspose.com/cells/java/getting-started/
[18]: https://blog.aspose.com/2020/10/13/create-excel-xlsx-xls-using-java-without-ms-office/





