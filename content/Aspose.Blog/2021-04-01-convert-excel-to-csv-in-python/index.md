---
title: 'Convert Excel to CSV in Python'
seoTitle: "Convert Excel to CSV in Python | XLSX to CSV Python Code Sample"
description: "Use Python spreadsheet API to convert Excel files to CSV in Python. Convert XLS or CSV or XLSX to CSV in Python without Pandas."
date: Thu, 01 Apr 2021 07:23:00 +0000
draft: false
url: /2021/04/01/convert-excel-to-csv-in-python/
author: Usman Aziz
summary: "Excel spreadsheets are widely used to keep, import, or export data from one application to another. In addition, you can perform various operations on data, such as sorting, applying mathematical formulas, generating charts, etc. However, in various cases, Excel's [XLSX][1] or [XLS][2] workbooks are required to be converted to [CSV][3] (Comma Separated Values) format. For such scenarios, this article covers **how to convert Excel files to CSV in Python**."
tags: ['Convert Excel File to CSV Python', 'Python Excel to CSV Converter API']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/convert-csv-excel-xls-xlsx-csharp.png" alt="Excel to CSV Python">}}


Excel spreadsheets are widely used to keep, import, or export data from one application to another. In addition, you can perform various operations on data, such as sorting, applying mathematical formulas, generating charts, etc. However, in various cases, Excel's [XLSX][4] or [XLS][5] workbooks are required to be converted to [CSV][6] (Comma Separated Values) format. For such scenarios, this article covers **how to convert Excel files to CSV in Python**.

*   [Excel to CSV Converter API][7]
*   [Convert Excel File to CSV][8]

## Python Excel to CSV Converter API {#Python-Excel-to-CSV-Converter-API}

In order to convert Excel's XLSX or XLS formats to CSV, we will use [Aspose.Cells for Python via Java][9]. It is a powerful spreadsheet manipulation API that allows you to create, modify or convert Excel files. You can install the API using the following command.

*   `pip install aspose-cells`

## Convert Excel File to CSV {#Convert-Excel-File-to-CSV}

The following are the steps to convert an Excel XLSX or XLS file to CSV in Python.

*   Load Excel file using [Workbook][10] class.
*   Convert Excel to CSV using [Workbook.save(String, SaveFormat.CSV)][11] method.

The following code sample shows how to convert an XLSX file to CSV in Python.

{{< gist aspose-com-gists 01d71bf3cafec445f7ea46625a5dbaa3 "excel-to-csv.py" >}}

### Excel File



{{< figure align=center src="images/image.png" alt="Excel to CSV Python">}}


### Converted CSV```
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

## Get a Free API License

You can use the API without evaluation limitations by requesting a [free temporary license][12].

## Conclusion

In this article, you have learned how to convert Excel files to CSV in Python. You can explore more about the Python spreadsheet API using the [documentation][13]. In case you would have any questions or queries, feel free to let us know via our [forum][14].

## See Also

*   [Create MS Excel Files using Python][15]
*   [Convert Excel to PDF in Python][16]




[1]: https://docs.fileformat.com/spreadsheet/xlsx/
[2]: https://docs.fileformat.com/spreadsheet/xls/
[3]: https://docs.fileformat.com/spreadsheet/csv/
[4]: https://docs.fileformat.com/spreadsheet/xlsx/
[5]: https://docs.fileformat.com/spreadsheet/xls/
[6]: https://docs.fileformat.com/spreadsheet/csv/
[7]: #Python-Excel-to-CSV-Converter-API
[8]: #Convert-Excel-File-to-CSV
[9]: https://products.aspose.com/cells/python-java
[10]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[11]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String,%20int)
[12]: https://purchase.aspose.com/temporary-license
[13]: https://docs.aspose.com/cells/pythonjava/
[14]: https://forum.aspose.com/
[15]: https://blog.aspose.com/2020/08/19/create-excel-xls-xlsx-using-python-excel-api/
[16]: https://blog.aspose.com/2021/04/02/convert-excel-files-to-pdf-in-python/





