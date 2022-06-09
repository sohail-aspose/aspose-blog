---
title: 'Convert JSON Data to CSV using Python'
seoTitle: "Covert JSON to CSV in Python | Python Source Code"
description: "Use Python Spreadsheet API to convert JSON data or files to CSV format using Python. Automate JSON to CSV conversion in your Python applications."
date: Sat, 04 Sep 2021 09:18:00 +0000
draft: false
url: /2021/09/04/convert-json-data-to-csv-using-python/
author: Usman Aziz
summary: '[JSON][1] is a well-known and widely used format to keep and share structured data. Often, it is used to transmit data between different types of applications. [CSV][2], on the other hand, is also used to store the data in a comma separated format. In certain cases, you may need to import data from JSON files to CSV. Therefore, in this article, you will learn **how to convert JSON data to CSV programmatically using Python**.'
tags: ['Convert JSON Data or File to CSV Python', 'JSON to CSV Python', 'Python JSON to CSV Conversion']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Convert-JSON-to-CSV.jpg" alt="JSON to CSV in Python">}}


[JSON][3] is a well-known and widely used format to keep and share structured data. Often, it is used to transmit data between different types of applications. [CSV][4], on the other hand, is also used to store the data in a comma separated format. In certain cases, you may need to import data from JSON files to CSV. Therefore, in this article, you will learn **how to convert JSON data to CSV programmatically using Python**.

*   [API for JSON to CSV Conversion][5]
*   [Convert JSON Data or File to CSV][6]

## Python API for JSON to CSV Conversion {#API-for-JSON-to-CSV-Conversion}

In order to convert JSON data to CSV format, we will use [Aspose.Cells for Python via Java][7]. It is a powerful API for creating, modifying, and converting spreadsheet files using Python. You can either [download][8] the API or install it using the following pip command.

*   `pip install aspose-cells`

## Convert a JSON Data or File to CSV {#Convert-JSON-Data-or-File-to-CSV}

The following are the steps to convert JSON data to CSV format using Python.

*   Create a new [Workbook][9] object.
*   Get reference of the first worksheet using [Workbook.getWorksheets().get(0)][10] method.
*   Create an object of _JsonLayoutOptions_ class to set additional options.
*   Import data from JSON to CSV using _JsonUtility.importData()_ method.
*   Save the CSV file using [Workbook.save(string, SaveFormat.CSV)][11] method.

The following code sample shows how to convert JSON data to CSV format.

{{< gist aspose-com-gists 05b412179a9a1745da590dc3b9fcba91 "json-to-csv.py" >}}

### JSON Data

The following is the JSON data that we used in the above code sample.

```
[{"nodeId":1,"reputation":1134},{"nodeId":2,"reputation":547},{"nodeId":3,"reputation":1703},{"nodeId":4,"reputation":-199},{"nodeId":5,"reputation":-306},{"nodeId":6,"reputation":-49},{"nodeId":7,"reputation":1527},{"nodeId":8,"reputation":1223}]'
```

### Converted CSV

The following is the converted CSV file.



{{< figure align=center src="images/JSON-to-CSV.jpg" alt="JSON to CSV">}}


## Get a Free License {#Get-a-Free-License}

Get a [temporary license][12] and use Aspose.Cells for Python via Java without evaluation limitations.

## Conclusion

JSON and CSV files are widely used to store and transmit the data. In accordance with that, this article covered how to convert JSON data or files to CSV using Python. Furthermore, you can also explore Aspose.Cells for Python via Java using the [documentation][13]. Also, you can ask your questions via our [forum][14].

## See Also

*   [Encrypt and Decrypt Excel Files in Python][15]
*   [Create MS Excel Files using Python – Python Excel API][16]




[1]: https://docs.fileformat.com/web/json/
[2]: https://docs.fileformat.com/spreadsheet/csv/
[3]: https://docs.fileformat.com/web/json/
[4]: https://docs.fileformat.com/spreadsheet/csv/
[5]: #API-for-JSON-to-CSV-Conversion
[6]: #Convert-JSON-Data-or-File-to-CSV
[7]: https://products.aspose.com/cells/python-java/
[8]: https://downloads.aspose.com/cells/python
[9]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[10]: https://apireference.aspose.com/cells/python/asposecells.api/worksheetcollection#Item%20(int)
[11]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String,%20int)
[12]: https://purchase.aspose.com/temporary-license
[13]: https://docs.aspose.com/cells/pythonjava
[14]: https://forum.aspose.com/
[15]: https://blog.aspose.com/2021/06/01/encrypt-and-decrypt-excel-files-in-python/
[16]: https://blog.aspose.com/2020/08/19/create-excel-xls-xlsx-using-python-excel-api/




