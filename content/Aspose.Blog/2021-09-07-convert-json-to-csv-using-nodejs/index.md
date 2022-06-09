---
title: 'Convert JSON Data to CSV using Node.js'
seoTitle: "Covert JSON to CSV in Node.js | Node.js Source Code"
description: "Use Node.js Spreadsheet API to convert JSON data or files to CSV format in Node.js. Automate JSON to CSV conversion in your Node.js applications."
date: Tue, 07 Sep 2021 13:18:00 +0000
draft: false
url: /2021/09/07/convert-json-to-csv-using-nodejs/
author: Usman Aziz
summary: '[JSON][1] files are widely used to transmit data between different applications. [CSV][2], on the other hand, is also a commonly used format to store the data in a comma separated format. In certain cases, you may need to import data from JSON files to CSV. For such cases, this article covers **how to convert JSON data to CSV programmatically using Node.js**.'
tags: ['convert json to csv nodejs', 'export json data to csv', 'import json data to csv nodejs', 'json to csv nodejs']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Convert-JSON-to-CSV.jpg" alt="JSON to CSV in Node.js">}}


[JSON][3] files are widely used to transmit data between different applications. [CSV][4], on the other hand, is also a commonly used format to store the data in a comma separated format. In certain cases, you may need to import data from JSON files to CSV. For such cases, this article covers **how to convert JSON data to CSV programmatically using Node.js**.

*   [API for JSON to CSV Conversion][5]
*   [Convert JSON Data or File to CSV][6]

## Node.js API for JSON to CSV Conversion {#API-for-JSON-to-CSV-Conversion}

For JSON to CSV conversion, we will use [Aspose.Cells for Node.js via Java][7]. It is a feature-rich API for creating, modifying, and converting spreadsheet files in Node.js applications. You can either [download][8] the API or install it using the following npm command.

`npm install aspose.cells`

## Convert JSON Data or File to CSV {#Convert-JSON-Data-or-File-to-CSV}

The following are the steps to convert JSON data to CSV format using Node.js.

*   Create a new [Workbook][9] object.
*   Get reference of the first worksheet using [Workbook.getWorksheets().get(0)][10] method.
*   Create an object of _JsonLayoutOptions_ class to set additional options.
*   Import data from JSON to CSV using _JsonUtility.importData()_ method.
*   Save the CSV file using [Workbook.save(string, SaveFormat.CSV)][11] method.

The following code sample shows how to convert JSON data to CSV format.

{{< gist aspose-com-gists 11bbd8922307a2430747c29074e5fd73 "json-to-csv.js" >}}

### JSON Data

The following is the JSON data that we used in the above code sample.

```
[{"nodeId":1,"reputation":1134},{"nodeId":2,"reputation":547},{"nodeId":3,"reputation":1703},{"nodeId":4,"reputation":-199},{"nodeId":5,"reputation":-306},{"nodeId":6,"reputation":-49},{"nodeId":7,"reputation":1527},{"nodeId":8,"reputation":1223}]'
```

### Converted CSV

The following is the converted CSV file.



{{< figure align=center src="images/JSON-to-CSV.jpg" alt="JSON to CSV">}}


## Get a Free License {#Get-a-Free-License}

Get a [temporary license][12] and use Aspose.Cells for Node.js via Java without evaluation limitations.

## Conclusion

JSON and CSV files are widely used to store and transmit the data. In accordance with that, this article covered how to convert JSON data or files to CSV in Node.js applications. Furthermore, you can explore Aspose.Cells for Node.js via Java using the [documentation][13]. Also, you can ask your questions via our [forum][14].

## See Also

*   [Convert Excel Files to PDF in Node.js][15]
*   [Create Excel XLSX/XLS Files in Node.js Applications][16]




[1]: https://docs.fileformat.com/web/json/
[2]: https://docs.fileformat.com/spreadsheet/csv/
[3]: https://docs.fileformat.com/web/json/
[4]: https://docs.fileformat.com/spreadsheet/csv/
[5]: #API-for-JSON-to-CSV-Conversion
[6]: #Convert-JSON-Data-or-File-to-CSV
[7]: https://products.aspose.com/cells/nodejs-java/
[8]: https://downloads.aspose.com/cells/nodejs
[9]: https://apireference.aspose.com/cells/nodejs/Workbook
[10]: https://apireference.aspose.com/cells/nodejs/WorksheetCollection#get
[11]: https://apireference.aspose.com/cells/nodejs/Workbook#save
[12]: https://purchase.aspose.com/temporary-license
[13]: https://docs.aspose.com/cells/nodejsjava
[14]: https://forum.aspose.com/
[15]: https://blog.aspose.com/2021/03/05/convert-excel-xlsx-xls-to-pdf-in-node-js/
[16]: https://blog.aspose.com/2020/08/05/create-excel-files-in-node.js/




