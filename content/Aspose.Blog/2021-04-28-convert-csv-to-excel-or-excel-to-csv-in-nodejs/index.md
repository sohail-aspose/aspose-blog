---
title: 'Convert CSV to Excel or Excel to CSV in Node.js'
seoTitle: "CSV to Excel, Excel to CSV in Node.js | XSLX to CSV | CSV to XLSX"
description: "Use Node.js Excel API to convert Excel files to CSV in Node.js applications. Convert XLSX XLS to CSV or CSV to XLSX XLS programmatically."
date: Wed, 28 Apr 2021 16:03:00 +0000
draft: false
url: /2021/04/28/convert-csv-to-excel-or-excel-to-csv-in-nodejs/
author: Usman Aziz
summary: '[CSV][1] format is widely used to import or export large datasets from one application to another. However, in some cases, you may need to convert CSV files to Excel [XLSX][2] or [XLS][3]. Likewise, vice versa can also be required in certain scenarios. In accordance with that, this article covers **how to convert CSV to Excel and Excel to CSV format programmatically in Node.js**.'
tags: ['csv to excel nodejs', 'csv to xlsx nodejs', 'excel to csv nodejs', 'xlsx to csv nodejs']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/convert-csv-excel-xls-xlsx-csharp.png" alt="convert csv to excel node.js">}}


[CSV][4] format is widely used to import or export large datasets from one application to another. However, in some cases, you may need to convert CSV files to Excel [XLSX][5] or [XLS][6]. Likewise, vice versa can also be required in certain scenarios. In accordance with that, this article covers **how to convert CSV to Excel and Excel to CSV format programmatically in Node.js**.

*   [Node.js CSV to Excel or Excel to CSV Converter][7]
*   [Convert CSV to XLSX or XLS in Node.js][8]
*   [Convert XLSX or XLS to CSV in Node.js][9]
*   [Get a Free API Licence][10]

## Node.js CSV to Excel or Excel to CSV Converter {#Node.js-CSV-to-Excel-or-Excel-to-CSV-Converter}

For back and forth conversion of CSV and Excel formats, we'll use [Aspose.Cells for Node.js via Java][11]. It is a powerful and feature-rich API for the manipulation of spreadsheet formats from within the Node.js applications. You can either [download][12] the API’s package or install it using the following [NPM][13] command.

```
 > npm install aspose.cells
```

## Convert CSV to XLSX or XLS in Node.js {#Convert-CSV-to-XLSX-or-XLSX-in-Node.js}

The following are the steps to convert a CSV file to Excel XLSX or XLS.

*   Create an object of [LoadOptions][14] class and initialize it with [FileFormatType.CSV][15].
*   Create an object of the [Workbook][16] class to load the CSV file.
*   Convert CSV to XLSX using [Workbook.save(String , SaveFormat.XLSX)][17] method.

The following code sample shows how to convert CSV to Excel XLSX in Node.js.

{{< gist aspose-com-gists abd903fb9bdac23bae74e548f4458445 "csv-to-excel.js" >}}

### Sample CSV```
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

### CSV to Excel



{{< figure align=center src="images/image.png" alt="csv to excel or excel to csv node.js">}}


## Convert XLSX or XLS to CSV in Node.js {#Convert-XLS-or-XLSX-to-CSV-in-Node.js}

The following are the steps to convert XLSX or XLS file to CSV in Node.js.

*   Create an object of the [Workbook][18] class to load the XLSX file.
*   Convert XLSX file to CSV using [Workbook.save(String , SaveFormat.CSV)][19] method.

The following code sample shows how to convert Excel XLSX or XLS to CSV.

{{< gist aspose-com-gists abd903fb9bdac23bae74e548f4458445 "excel-to-csv.js" >}}

## Get a Free API License {#Get-a-Free-API-License}

In order to use the API without evaluation limitations, you can [request a free temporary license][20].

## Conclusion

In this article, you have learned how easy it is to convert CSV to Excel or Excel to CSV in Node.js applications. You can explore more about the Node.js Excel API using the [documentation][21]. In case you would have any queries, feel free to let us know via our [forum][22].

## See Also

*   [Convert Excel Files to PDF in Node.js][23]
*   [Create Excel XLSX/XLS Files in Node.js Applications][24]




[1]: https://docs.fileformat.com/spreadsheet/csv/
[2]: https://docs.fileformat.com/spreadsheet/xlsx/
[3]: https://docs.fileformat.com/spreadsheet/xls/
[4]: https://docs.fileformat.com/spreadsheet/csv/
[5]: https://docs.fileformat.com/spreadsheet/xlsx/
[6]: https://docs.fileformat.com/spreadsheet/xls/
[7]: #Node.js-CSV-to-Excel-or-Excel-to-CSV-Converter
[8]: #Convert-CSV-to-XLSX-or-XLSX-in-Node.js
[9]: #Convert-XLS-or-XLSX-to-CSV-in-Node.js
[10]: #Get-a-Free-API-License
[11]: https://products.aspose.com/cells/nodejs-java
[12]: https://downloads.aspose.com/cells/nodejs
[13]: https://www.npmjs.com/package/aspose.cells
[14]: https://apireference.aspose.com/cells/nodejs/LoadOptions
[15]: https://apireference.aspose.com/cells/nodejs/global#FileFormatType#.CSV
[16]: https://apireference.aspose.com/cells/nodejs/Workbook
[17]: https://apireference.aspose.com/cells/nodejs/Workbook#save
[18]: https://apireference.aspose.com/cells/nodejs/Workbook
[19]: https://apireference.aspose.com/cells/nodejs/Workbook#save
[20]: https://purchase.aspose.com/temporary-license
[21]: https://docs.aspose.com/cells/nodejsjava/
[22]: https://forum.aspose.com/
[23]: https://blog.aspose.com/2021/03/05/convert-excel-xlsx-xls-to-pdf-in-node-js/
[24]: https://blog.aspose.com/2020/08/05/create-excel-files-in-node.js/





