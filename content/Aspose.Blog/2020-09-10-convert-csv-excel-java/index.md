---
title: 'Convert CSV to Excel or Excel to CSV File using Java'
seoTitle: "Java Convert CSV to Excel XLSX XLS or Excel to CSV Programmatically"
description: "Convert Excel XLSX XLS to CSV or CSV to Excel programmatically using Java code. Import or Export CSV, XLSX, XLS file easily with high fidelity."
date: Thu, 10 Sep 2020 22:20:53 +0000
draft: false
url: /2020/09/10/convert-csv-excel-java/
author: Farhan Raza
summary: 'CSV file format is used to save comma-separated values. CSV to Excel conversion is helpful when there are numbers involved in the input data and you need to perform some calculations. Likewise, Excel to CSV conversion is helpful in some scenarios, like serialization of data in some cases. Let us explore the inter-conversion between CSV and Excel file format.'
tags: ['CSV to Excel', 'CSV to XLS', 'CSV to XLSX', 'Convert CSV to Excel', 'Excel to CSV', 'XLS to CSV', 'XLSX to CSV', 'csv to excel java', 'csv to xlsx java', 'java convert csv to xlsx', 'java csv to xlsx']
categories: ['Aspose.Cells Product Family']
---

[CSV][1] file format is used to save comma-separated values. CSV to Excel conversion is helpful when there are numbers involved in the input data and you need to perform some calculations. Likewise, Excel to CSV conversion is helpful in some scenarios, like serialization of data in some cases. Let us explore the inter-conversion between CSV and Excel file format ([XLS][2]/[XLSX][3] in detail using [Aspose.Cells for Java][4] API:

*   [CSV to Excel and Excel to CSV Converter API – Installation][5]
*   [Convert CSV to Excel (XLSX/XLS) using Java][6]
*   [Convert Excel (XLSX/XLS) to CSV using Java][7]

## CSV to Excel and Excel to CSV Converter API – Installation {#section1}

In order to convert these file formats, firstly you need to configure Aspose.Cells for Java API in your Java environment. This will let you achieve the requirements with only a couple of lines of code. The API will take care of the rest of the tasks and activities. You can set it up either by downloading the JAR file or by adding the following Maven Repository specifications:

### Repository```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```

### Dependency```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-cells</artifactId>
    <version>20.8</version>
</dependency>
```

After installing and configuring the API successfully, let us proceed to learn the conversion CSV and Excel (XLSX/XLS) file formats.

## Convert CSV to Excel (XLSX/XLS) using Java {#section2}

One of the popular use cases for **CSV to Excel conversion** is when you need to populate some values into a Table in the Excel worksheet. Likewise, the are many possibilities and use cases where you might need to perform this conversion. To keep this simple and easy, let us consider a basic CSV file as an example:

```
My Data,,,,,,,

Items A,Items B,Items C,Items D,Items E,Items F,Items G,Items H
12,23,33,66,11,87,99,33
23,22,33,77,31,22,45,56
34,11,12,23,22,34,11,12
45,43,54,88,36,45,45,37
65,65,65,65,13,65,9,35
34,22,27,22,32,23,23,32
213,186,224,341,145,276,232,205
```

Let us follow the steps below to convert a CSV to Excel file:

1.  Initialize [LoadOptions][8] class object
2.  Specify [FileFormatType][9] as [CSV][10]
3.  Instantiate an object of [Workbook][11] class
4.  Save the output Excel file

The code snippet below shows how to convert CSV to Excel (XLSX/XLS) using Java:

\[gist id="8fe0aa068ce23dadc02f3bd0e1802a28" file="CSVtoExcel.java"\]

The screenshot below shows the output Excel file generated with the above code snippet:



{{< figure align=center src="images/Convert-Excel-CSV.png" alt="Convert Excel CSV">}}


## Convert Excel (XLSX/XLS) to CSV using Java {#section3}

**Excel (XLSX/XLS) to CSV** conversion is also an important use case. As we have created an Excel file already, let us consider it as an input file to proceed with the conversion. This can explain the high fidelity between the conversion of CSV and Excel files that we have converted already. Let us follow the steps below for converting Excel (XLSX/XLS) to CSV using Java.

1.  Load the input Excel file with [Workbook][12] constructor
2.  Save output CSV file by specifying the CSV [SaveFormat][13]

Following code snippet shows how to convert Excel (XLSX/XLS) to CSV in Java:

\[gist id="8fe0aa068ce23dadc02f3bd0e1802a28" file="ExceltoCSV.java"\]

After converting the input Excel file, you may compare the output CSV file with the file which was used above in the first example. You will notice the output files are identical to each other. This high fidelity speaks volumes about the efficiency of these file format conversions.

## Conclusion

In a nutshell, we have learned how easily we can convert an Excel file to CSV and CSV to Excel with Java. However, if you notice any problem with configuration or conversion then please feel free to reach out to us at [Free Support Forum][14]. We would love to help you out!

## See Also

[Convert CSV to Excel Files or Excel to CSV using C# VB.NET][15]



[1]: https://docs.fileformat.com/spreadsheet/csv/
[2]: https://docs.fileformat.com/spreadsheet/xls/
[3]: https://docs.fileformat.com/spreadsheet/xlsx/)
[4]: https://products.aspose.com/cells/java
[5]: #section1
[6]: #section2
[7]: #section3
[8]: https://apireference.aspose.com/cells/java/com.aspose.cells/LoadOptions
[9]: https://apireference.aspose.com/cells/java/com.aspose.cells/FileFormatType
[10]: https://apireference.aspose.com/cells/java/com.aspose.cells/fileformattype#CSV
[11]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[12]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[13]: https://apireference.aspose.com/cells/java/com.aspose.cells/SaveFormat
[14]: https://forum.aspose.com/c/cells
[15]: https://blog.aspose.com/2020/11/17/csv-excel-csharp-vb-net/





