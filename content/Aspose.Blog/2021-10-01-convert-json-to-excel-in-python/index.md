---
title: 'Convert JSON to Excel Worksheet in Python'
seoTitle: "Convert JSON to Excel in Python | Import JSON Data to XLSX or XLS"
description: "Use Python Excel API to convert JSON data to Excel worksheet using Python. Import data from JSON to Excel and apply styles using Python."
date: Fri, 01 Oct 2021 17:24:52 +0000
draft: false
url: /2021/10/01/convert-json-to-excel-in-python/
author: Usman Aziz
summary: 'MS Excel is a feature-rich program that lets you keep and organize data in tabular form. Moreover, it allows you to store the data in multiple worksheets. In addition to the data organization, you can perform sorting, graph plotting, mathematical computations and etc. [JSON][1], on the other hand, is a widely used format to store and transmit the data in the form of key-value pairs. In certain cases, you may need to import data from JSON files to Excel worksheets programmatically. In accordance with that, this article covers **how to convert JSON data to Excel XLSX/XLS using Python**.'
tags: ['JSON to Excel Python', 'JSON to XLS Python', 'JSON to XLSX Python']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Convert-JSON-to-Excel-C.png" alt="Convert JSON to Excel Python">}}


MS Excel is a feature-rich program that lets you keep and organize data in tabular form. Moreover, it allows you to store the data in multiple worksheets. In addition to the data organization, you can perform sorting, graph plotting, mathematical computations and etc. [JSON][2], on the other hand, is a widely used format to store and transmit the data in the form of key-value pairs. In certain cases, you may need to import data from JSON files to Excel worksheets programmatically. In accordance with that, this article covers **how to convert JSON data to Excel XLSX/XLS using Python**.

*   [Python API for JSON to Excel Conversion][3]
*   [Import Data from JSON to Excel Worksheet][4]
*   [Apply Cell Formatting in JSON to Excel Conversion][5]

## Python API for JSON to Excel Conversion {#API-for-JSON-to-Excel-Conversion}

In order to perform JSON to Excel conversion, we'll use [Aspose.Cells for Python via Java][6]. It is a spreadsheet manipulation API that lets you create, modify or convert Excel files using Python. You can either [download][7] the API or install it using the following pip command.

*   `pip install aspose-cells`

## Import Data from JSON to Excel in Python {#Import-Data-from-JSON-to-Excel-Worksheet}

The following are the steps to import data from JSON to Excel in Python:

*   Create a new [Workbook][8] object.
*   Get reference of the desired worksheet using [Workbook.getWorksheets().get(index)][9] method.
*   Create an object of _JsonLayoutOptions_ class to set additional options.
*   Import data from JSON to Excel using _JsonUtility.importData()_ method.
*   Save the Excel file using [Workbook.save(string, SaveFormat)][10] method.

The following code sample shows how to import data from JSON to Excel.

{{< gist aspose-com-gists 02b2579f7a9876d6142bf25b411ede1a "JSON-to-Excel.py" >}}

### Input JSON Data```
[{"nodeId":1,"reputation":1134},{"nodeId":2,"reputation":547},{"nodeId":3,"reputation":1703},{"nodeId":4,"reputation":-199},{"nodeId":5,"reputation":-306},{"nodeId":6,"reputation":-49},{"nodeId":7,"reputation":1527},{"nodeId":8,"reputation":1223}]'
```

### Output Excel Worksheet



{{< figure align=center src="images/JSON-to-Excel.jpg" alt="JSON to Excel Python">}}


## Import JSON to Excel with Formatting Styles {#Import-JSON-to-Excel-with-Formatting-Styles}

Aspose.Cells also allows you to apply styles in JSON to Excel conversion. For example, you can set font, color, alignment, border styles, etc. The following are the steps to apply styles while importing data from JSON to Excel.

*   Create a new [Workbook][11] object.
*   Get reference of the desired worksheet using [Workbook.getWorksheets().get(index)][12] method.
*   Create an object of [CellsFactory][13] class and retreive reference of [Style][14] using [CellsFactory.createStyle()][15] method.
*   Set desired styling options.
*   Create an object of _JsonLayoutOptions_ class to set additional options.
*   Import data from JSON to Excel using _JsonUtility.importData()_ method.
*   Save the Excel file using [Workbook.save(string, SaveFormat)][16] method.

The following code sample applies different styles when importing data from JSON to Excel in Python.

{{< gist aspose-com-gists 02b2579f7a9876d6142bf25b411ede1a "JSON-to-Excel-Styles.py" >}}

### Output Excel Worksheet



{{< figure align=center src="images/JSON-to-Excel-Formatting.jpg" alt="JSON to XLSX Python">}}


## Get a Free License {#Get-a-Free-License}

You can use Aspose.Cells for Python via Java without evaluation limitations using a [temporary license][17].

## Conclusion

JSON and Excel files are extensively used to store and share the data. Accordingly, in this article, you have learned how to import data from JSON to Excel XLSX/XLS using Python. In addition, you have seen how to apply formatting in JSON to Excel conversion. You can also explore other features of Aspose.Cells for Python via Java using the [documentation][18]. In case you would have any queries, you can post on our [forum][19].

## See Also

*   [Encrypt and Decrypt Excel Files in Python][20]
*   [Create MS Excel Files using Python – Python Excel API][21]




[1]: https://en.wikipedia.org/wiki/JSON
[2]: https://en.wikipedia.org/wiki/JSON
[3]: #API-for-JSON-to-Excel-Conversion
[4]: #Import-Data-from-JSON-to-Excel-Worksheet
[5]: #Import-JSON-to-Excel-with-Formatting-Styles
[6]: https://products.aspose.com/cells/python-java/
[7]: https://downloads.aspose.com/cells/python
[8]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[9]: https://apireference.aspose.com/cells/python/asposecells.api/worksheetcollection#Item%20(int)
[10]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String,%20int)
[11]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[12]: https://apireference.aspose.com/cells/python/asposecells.api/worksheetcollection#Item%20(int)
[13]: https://apireference.aspose.com/cells/python/asposecells.api/CellsFactory
[14]: https://apireference.aspose.com/cells/python/asposecells.api/Style
[15]: https://apireference.aspose.com/cells/python/asposecells.api/cellsfactory#createStyle()
[16]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String,%20int)
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/cells/pythonjava
[19]: https://forum.aspose.com/
[20]: https://blog.aspose.com/2021/06/01/encrypt-and-decrypt-excel-files-in-python/
[21]: https://blog.aspose.com/2020/08/19/create-excel-xls-xlsx-using-python-excel-api/




