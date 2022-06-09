---
title: 'Convert CSV to Excel in Python'
seoTitle: "Convert CSV to Excel in Python | CSV to XLSX without Pandas | Code"
description: "Use Python spreadsheet API to convert CSV files to Excel in Python. Convert CSV to XLS or CSV to XLSX in Python without Pandas."
date: Mon, 17 May 2021 04:05:00 +0000
draft: false
url: /2021/05/17/convert-csv-to-excel-in-python/
author: Usman Aziz
summary: "[CSV][1] (Comma Separated Values) is a commonly used file format to keep, import, and export data from one application to another. Furthermore, most of the datasets in the field of data science are stored in CSV files. However, in certain cases, you have to convert comma separated values in CSV to tabular form in Excel's XLSX or XLS workbooks. For such scenarios, this article covers **how to convert CSV files to Excel in Python**."
tags: ['Convert CSV to Excel XLSX or XLS', 'Python CSV to Excel Converter API']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/convert-csv-excel-xls-xlsx-csharp.png" alt="CSV to Excel Python">}}


[CSV][2] (Comma Separated Values) is a commonly used file format to keep, import, and export data from one application to another. Furthermore, most of the datasets in the field of data science are stored in CSV files. However, in certain cases, you have to convert comma separated values in CSV to tabular form in Excel's XLSX or XLS workbooks. For such scenarios, this article covers **how to convert CSV files to Excel in Python**.

*   [Python CSV to Excel Converter API][3]
*   [Convert CSV to Excel XLSX or XLS][4]

## Python CSV to Excel Converter API {#Python-CSV-to-Excel-Converter-API}

In order to convert CSV to Excel's XLSX or XLS formats, we will use [Aspose.Cells for Python via Java][5]. It is a powerful spreadsheet manipulation API that allows you to create, modify or convert Excel files. You can install the API using the following command.

*   `pip install aspose-cells`

## Convert CSV to Excel in Python {#Convert-CSV-to-Excel-XLSX-or-XLS}

The following are the steps to convert a CSV file to Excel XLSX or XLS format.

*   Create an object of [LoadOptions][6] class and initialize it with [FileFormatType.CSV][7].
*   Create an object of the [Workbook][8] class and initialize it with the CSV file's path and _LoadOptions_ object.
*   Convert CSV to Excel using [Workbook.save(String, SaveFormat.XLSX)][9] method.

The following code sample shows how to convert CSV file to Excel in Python.

{{< gist aspose-com-gists 01d71bf3cafec445f7ea46625a5dbaa3 "csv-to-excel.py" >}}

### CSV File```
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

### Converted Excel File



{{< figure align=center src="images/image.png" alt="CSV to Excel in Python">}}


## Get a Free API License

You can use the API without evaluation limitations by requesting a [free temporary license][10].

## Conclusion

In this article, you have learned how to convert CSV files to Excel in Python. You can explore more about the Python spreadsheet API using the [documentation][11]. In case you would have any questions or queries, feel free to let us know via our [forum][12].

## See Also

*   [Create MS Excel Files using Python][13]
*   [Convert Excel to PDF in Python][14]




[1]: https://docs.fileformat.com/spreadsheet/csv/
[2]: https://docs.fileformat.com/spreadsheet/csv/
[3]: #Python-CSV-to-Excel-Converter-API
[4]: #Convert-CSV-to-Excel-XLSX-or-XLS
[5]: https://products.aspose.com/cells/python-java
[6]: https://apireference.aspose.com/cells/python/asposecells.api/LoadOptions
[7]: https://apireference.aspose.com/cells/python/asposecells.api/FileFormatType
[8]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[9]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String,%20int)
[10]: https://purchase.aspose.com/temporary-license
[11]: https://docs.aspose.com/cells/pythonjava/
[12]: https://forum.aspose.com/
[13]: https://blog.aspose.com/2020/08/19/create-excel-xls-xlsx-using-python-excel-api/
[14]: https://blog.aspose.com/2021/04/02/convert-excel-files-to-pdf-in-python/





