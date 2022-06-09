---
title: 'Convert JSON to PDF using Java'
seoTitle: "JSON to PDF in Java | Convert JSON Data to PDF in Java"
description: "Use Java Excel API to convert JSON data to PDF using Java. Import JSON data and convert it to PDF from within Spring or other Java applications."
date: Sat, 22 May 2021 03:43:00 +0000
draft: false
url: /2021/05/22/convert-json-to-pdf-using-java/
author: Usman Aziz
summary: '[JSON][1] to [PDF][2] conversion is required in various cases for sharing, printing, or other purposes. To perform this conversion programmatically, this article covers **how to convert JSON to PDF using Java**.'
tags: ['JSON to PDF Java', 'Java API for JSON to PDF Conversion', 'Java JSON to PDF Converter']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/JSON-to-PDF.jpg" alt="JSON to PDF Java">}}


[JSON][3] to [PDF][4] conversion is required in various cases for sharing, printing, or other purposes. To perform this conversion programmatically, this article covers **how to convert JSON to PDF using Java**.

*   [API for JSON to PDF Conversion][5]
*   [Convert JSON Data to PDF][6]

## Java API for JSON to PDF Conversion {#API-for-JSON-to-PDF-Conversion}

In order to convert JSON files to PDF format, we will use [Aspose.Cells for Java][7]. It is a feature-rich spreadsheet manipulation API that allows you to generate and process Excel files using Java. You can either [download][8] the API or install it using the following [Maven][9] configurations.

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

## Convert JSON Data to PDF {#Convert-JSON-to-PDF-in-Csharp}

The following are the steps to convert a JSON file to PDF using Java.

1.  First, create an instance of [Workbook][10] class.
2.  Select the default [Worksheet][11] from the [WorksheetsCollection][12].
3.  Read JSON data into a string object.
4.  Create an instance of [JsonLayoutOptions][13] and set options.
5.  Import data from JSON to worksheet using [JsonUtility.importData][14] method with reference to [Worksheet][15] object and JSON data.
6.  Finally, convert JSON to PDF by saving the workbook as PDF using [Workbook.save(string, SaveFormat.Auto)][16] method.

The following code sample shows how to convert a JSON file to PDF.

{{< gist aspose-com-gists a92f28aeaffae678d3433561ec7d4193 "json-to-pdf.java" >}}

## Get a Free License {#Get-a-Free-License}

You can use Aspose.Cells for Java without evaluation limitations using a [temporary license][17].

## Conclusion

In this article, you have learned how to convert JSON data to PDF using Java. You can easily install the API and use the provided code sample in your Java applications. Furthermore, to learn more about Aspose.Cells for Java, you can explore the [documentation][18]. Also, you can post your questions or queries on our [forum][19].

## See Also

*   [Import Data from JSON to Excel in Java][20]




[1]: https://docs.fileformat.com/web/json/
[2]: https://docs.fileformat.com/pdf/
[3]: https://docs.fileformat.com/web/json/
[4]: https://docs.fileformat.com/pdf/
[5]: #API-for-JSON-to-PDF-Conversion
[6]: #Convert-JSON-to-PDF-in-Csharp
[7]: https://products.aspose.com/cells/java
[8]: https://downloads.aspose.com/cells/java
[9]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-cells
[10]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[11]: https://apireference.aspose.com/cells/java/com.aspose.cells/Worksheet
[12]: https://apireference.aspose.com/cells/java/com.aspose.cells/WorksheetCollection
[13]: https://apireference.aspose.com/cells/java/com.aspose.cells/JsonLayoutOptions
[14]: https://apireference.aspose.com/cells/java/com.aspose.cells/jsonutility#importData(java.lang.String,%20com.aspose.cells.Cells,%20int,%20int,%20com.aspose.cells.JsonLayoutOptions)
[15]: https://apireference.aspose.com/cells/java/com.aspose.cells/Worksheet
[16]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String,%20int)
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/cells/java
[19]: https://forum.aspose.com/
[20]: https://blog.aspose.com/2019/04/20/import-data-from-json-using-aspose.cells-for-java-19.3/





