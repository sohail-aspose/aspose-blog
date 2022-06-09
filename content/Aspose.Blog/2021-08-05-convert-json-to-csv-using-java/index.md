---
title: 'Convert JSON to CSV Programmatically using Java'
seoTitle: "Covert JSON to CSV in Java | Java API | Source Code"
description: "Use Java Spreadsheet API to convert JSON data or files to CSV format using Java. Automate JSON to CSV conversion in your Java applications."
date: Thu, 05 Aug 2021 13:39:00 +0000
draft: false
url: /2021/08/05/convert-json-to-csv-using-java/
author: Usman Aziz
summary: '[JSON][1] files are widely used to store and transmit structured data between applications. On the other hand, [CSV][2] is also used to store the data, such as datasets, as comma-separated values. In this article, you will learn how to export data from JSON files to CSV programmatically. More specifically, the article will cover **how to convert JSON data to CSV using Java**.'
tags: ['convert json data to csv in java', 'json to csv converter java', 'json to csv java']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Convert-JSON-to-CSV.jpg" alt="JSON to CSV in Java">}}


[JSON][3] files are widely used to store and transmit structured data between applications. On the other hand, [CSV][4] is also utilized to store the data, such as datasets, as comma-separated values. In this article, you will learn how to export data from JSON files to CSV programmatically. More specifically, the article will cover **how to convert JSON data to CSV using Java**.

*   [API for JSON to CSV Conversion][5]
*   [Convert JSON Data or File to CSV][6]

## Java API for JSON to CSV Conversion {#API-for-JSON-to-CSV-Conversion}

[Aspose.Cells for Java][7] is a powerful API to create and manipulate spreadsheet documents from within the Java applications. We will use this API to convert the JSON data to CSV format. You can either [download][8] Aspose.Cells for Java or install it using the following Maven configurations.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-cells</artifactId>
    <version>21.9</version>
</dependency>
```

## Convert a JSON Data or File to CSV {#Convert-JSON-Data-or-File-to-CSV}

The following are the steps to convert JSON data to CSV format using Java.

*   Create a new [Workbook][9] object.
*   Get reference of the first worksheet using [Workbook.getWorksheets().get(0)][10] method.
*   Create an object of [JsonLayoutOptions][11] class to set additional options.
*   Import data from JSON to CSV using [JsonUtility.importData()][12] method.
*   Save the CSV file using [Workbook.save(string, SaveFormat.CSV)][13] method.

The following code sample shows how to convert JSON data to CSV format.

{{< gist aspose-com-gists 33eb534a63398b3a4f04cfc52fd6c8c3 "json-to-csv.java" >}}

### JSON Data

The following is the JSON data that we used in the above code sample.

```
[{"nodeId":1,"reputation":1134},{"nodeId":2,"reputation":547},{"nodeId":3,"reputation":1703},{"nodeId":4,"reputation":-199},{"nodeId":5,"reputation":-306},{"nodeId":6,"reputation":-49},{"nodeId":7,"reputation":1527},{"nodeId":8,"reputation":1223}]'
```

### Converted CSV

The following is the screenshot of the data converted to CSV format.



{{< figure align=center src="images/JSON-to-CSV.jpg" alt="JSON to CSV">}}


## Get a Free License {#Get-a-Free-License}

You can get a [temporary license][14] and use Aspose.Cells for Java without evaluation limitations.

## Conclusion

JSON and CSV files are immensely used to keep and exchange data. Often, you need to export data from JSON files to CSV programmatically. For such cases, this article covered how to convert JSON data or files to CSV using Java. Alongside, you can also explore Aspose.Cells for Java using the [documentation][15]. In addition, you can ask your questions via our [forum][16].

## See Also

*   [Create Excel Files using Java without MS Office][17]




[1]: https://docs.fileformat.com/web/json/
[2]: https://docs.fileformat.com/spreadsheet/csv/
[3]: https://docs.fileformat.com/web/json/
[4]: https://docs.fileformat.com/spreadsheet/csv/
[5]: #API-for-JSON-to-CSV-Conversion
[6]: #Convert-JSON-Data-or-File-to-CSV
[7]: https://products.aspose.com/cells/java
[8]: https://downloads.aspose.com/cells/java
[9]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[10]: https://apireference.aspose.com/cells/java/com.aspose.cells/worksheetcollection#Item%20(int)
[11]: https://apireference.aspose.com/cells/java/com.aspose.cells/JsonLayoutOptions
[12]: https://apireference.aspose.com/cells/java/com.aspose.cells/jsonutility#importData(java.lang.String,%20com.aspose.cells.Cells,%20int,%20int,%20com.aspose.cells.JsonLayoutOptions)
[13]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String,%20int)
[14]: https://purchase.aspose.com/temporary-license
[15]: https://docs.aspose.com/cells/java
[16]: https://forum.aspose.com/
[17]: https://blog.aspose.com/2020/10/13/create-excel-xlsx-xls-using-java-without-ms-office/





