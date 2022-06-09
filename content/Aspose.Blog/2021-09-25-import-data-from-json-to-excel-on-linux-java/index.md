---
title: 'Import Data from JSON to Excel on Linux'
seoTitle: "JSON to Excel on Linux | XLSX to JSON, XLS to JSON on Linux"
description: "Use Java Spreadsheet API to import data from JSON to Excel on the Linux platform. Import data from JSON to XLSX or XLS programmatically on Linux."
date: Sat, 25 Sep 2021 15:52:00 +0000
draft: false
url: /2021/09/25/import-data-from-json-to-excel-on-linux-java/
author: Usman Aziz
summary: '[JSON][1] files are immensely used to store and transmit structured data. However, in certain cases, you may need to import data from JSON files to Excel spreadsheets. To achieve this programmatically, this article covers **how to convert JSON files to Excel [XLSX][2] or [XLS][3] format on the Linux platform**.'
tags: ['Import JSON to Excel Linux', 'JSON to Excel Linux', 'JSON to XLS Linux', 'JSON to XLSX Linux']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Convert-JSON-to-Excel-C.png" alt="Convert JSON to Excel Linux">}}


[JSON][4] files are immensely used to store and transmit structured data. However, in certain cases, you may need to import data from JSON files to Excel spreadsheets. To achieve this programmatically, this article covers **how to convert JSON files to Excel [XLSX][5] or [XLS][6] format on the Linux platform**.

*   [API to Import Data from JSON to Excel][7]
*   [Import JSON Data to Excel][8]

## API to Import Data from JSON to Excel on Linux {#API-to-Import-Data-from-JSON-to-Excel}

[Aspose.Cells for Java][9] is a powerful and feature-rich API that lets you create and process spreadsheet documents. In addition, it lets you convert the spreadsheet files with high fidelity. You can download the API’s [JAR][10] or install it using the following Maven configurations.

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
    <version>21.9</version>
</dependency>
```

## Import JSON Data to Excel on Linux {#Import-JSON-Data-to-Excel}

The following are the steps to import data from a JSON file to an Excel spreadsheet.

*   First, read the JSON data into a string object.
*   Then, create an instance of [Workbook][11] class.
*   Get the reference of first worksheet into a [Worksheet][12] object.
*   Create an instance of [JsonLayoutOptions][13] class.
*   Set option using [JsonLayoutOptions.setArrayAsTable()][14].
*   Import data from JSON to Excel using [JsonUtility.importData()][15] method.
*   Finally, save the workbook using [Workbook.save(string, SaveFormat)][16] method.

The following code sample shows how to import data from JSON to Excel worksheet.

{{< gist aspose-com-gists 472e8ea861c2359f0ea55d4a4ce9d0c7 "json-to-excel.java" >}}

## Get a Free License {#Get-a-Free-License}

You can use Aspose.Cells for Java without evaluation limitations using a [temporary license][17].

## Conclusion

In this article, you have learned how to import data from JSON files to Excel XLSX/XLS on Linux. You can explore more about Aspose.Cells for Java using the [documentation][18]. In case you would have any queries, you can ask us via our [forum][19].

## See Also

*   [Convert Excel Files to PDF using Java][20]
*   [Convert Excel Files to PDF on Linux using .NET][21]
*   [Import Data from JSON to Excel on Linux using .NET][22]
*   [Create or Edit Excel Files on Linux using Java][23]




[1]: https://docs.fileformat.com/web/json/
[2]: https://docs.fileformat.com/spreadsheet/xlsx/
[3]: https://docs.fileformat.com/spreadsheet/xls/
[4]: https://docs.fileformat.com/web/json/
[5]: https://docs.fileformat.com/spreadsheet/xlsx/
[6]: https://docs.fileformat.com/spreadsheet/xls/
[7]: #API-to-Import-Data-from-JSON-to-Excel
[8]: #Import-JSON-Data-to-Excel
[9]: https://products.aspose.com/cells/java
[10]: https://downloads.aspose.com/cells/java
[11]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[12]: https://apireference.aspose.com/cells/java/com.aspose.cells/Worksheet
[13]: https://apireference.aspose.com/cells/java/com.aspose.cells/JsonLayoutOptions
[14]: https://apireference.aspose.com/cells/java/com.aspose.cells/jsonlayoutoptions#ArrayAsTable
[15]: https://apireference.aspose.com/cells/java/com.aspose.cells/jsonutility#importData(java.lang.String,%20com.aspose.cells.Cells,%20int,%20int,%20com.aspose.cells.JsonLayoutOptions)
[16]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String,%20int)
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/cells/java
[19]: https://forum.aspose.com/
[20]: https://blog.aspose.com/2020/08/12/convert-excel-to-pdf-using-java/
[21]: https://blog.aspose.com/2021/10/12/convert-excel-files-to-pdf-on-linux/
[22]: https://blog.aspose.com/2021/09/16/import-data-from-json-to-excel-on-linux/
[23]: https://blog.aspose.com/2021/10/08/create-excel-files-on-linux/




