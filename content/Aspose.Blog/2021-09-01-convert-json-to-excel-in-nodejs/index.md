---
title: 'Convert JSON to Excel Worksheet in Node.js'
seoTitle: "Convert JSON to Excel in Node.js | Import JSON Data to XLSX or XLS"
description: "Use Node.js Excel API to convert JSON data to Excel worksheet in Node.js. Export data from JSON to Excel and apply styles using Node.js."
date: Wed, 01 Sep 2021 14:48:00 +0000
draft: false
url: /2021/09/01/convert-json-to-excel-in-nodejs/
author: Usman Aziz
summary: 'MS Excel provides a wide range of features to keep and organize data in the form of worksheets contained by workbooks. In addition to the data organization, it lets you perform sorting, data visualization, mathematical computations and etc. In certain cases, you receive the data in JSON format and need to import it to Excel worksheets programmatically. For such cases, this article covers **how to convert JSON data to Excel XLSX/XLS in Node.js**.'
tags: ['json to excel nodejs', 'json to xls nodejs', 'json to xlsx nodejs']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Convert-JSON-to-Excel-C.png" alt="Convert JSON to Excel Node.js">}}


MS Excel provides a wide range of features to keep and organize data in the form of worksheets contained by workbooks. In addition to the data organization, it lets you perform sorting, data visualization, mathematical computations and etc. In certain cases, you receive data in [JSON][1] format and you need to export it to Excel worksheets programmatically. For such cases, this article covers **how to convert JSON data to Excel XLSX/XLS in Node.js**.

*   [Node.js API for JSON to Excel Conversion][2]
*   [Convert JSON to Excel Worksheet][3]
*   [Apply Cell Formatting in JSON to Excel Conversion][4]

## Node.js API for JSON to Excel Conversion {#API-for-JSON-to-Excel-Conversion}

[Aspose.Cells for Node.js via Java][5] is a powerful API that lets you create, modify or convert Excel files in Node.js applications. We will use this API to import data from JSON to Excel worksheets. You can either [download][6] the API’s package or install it using the following [NPM][7] command.

```
> npm install aspose.cells
```

## Convert JSON to Excel in Node.js {#Import-Data-from-JSON-to-Excel-Worksheet}

The following are the steps to convert JSON to Excel in Node.js:

*   Create a new [Workbook][8] object.
*   Get reference of the first worksheet using [Workbook.getWorksheets().get(0)][9] method.
*   Create an object of _JsonLayoutOptions_ class to set additional options.
*   Import data from JSON to Excel using _JsonUtility.importData()_ method.
*   Save the Excel file using [Workbook.save(string, SaveFormat)][10] method.

The following code sample shows how to import data from JSON to Excel.

{{< gist aspose-com-gists 2c4dcc027318410c00c7c2fd0c5c702b "json-to-excel.js" >}}

### Input JSON Data```
[{"nodeId":1,"reputation":1134},{"nodeId":2,"reputation":547},{"nodeId":3,"reputation":1703},{"nodeId":4,"reputation":-199},{"nodeId":5,"reputation":-306},{"nodeId":6,"reputation":-49},{"nodeId":7,"reputation":1527},{"nodeId":8,"reputation":1223}]'
```

### Output Excel Worksheet



{{< figure align=center src="images/JSON-to-Excel.jpg" alt="JSON to Excel Node.js">}}


## Convert JSON to Excel with Styles {#Import-JSON-to-Excel-with-Formatting-Styles}

You can also apply styles in JSON to Excel conversion using Aspose.Cells for Node.js via Java. For example, you can set font, color, alignment, border styles, etc. The following are the steps to apply styles while importing data from JSON to Excel.

*   Create a new [Workbook][11] object.
*   Get reference of the first worksheet using [Workbook.getWorksheets().get(0)][12] method.
*   Create an object of [CellsFactory][13] class and retreive reference of [Style][14] using [CellsFactory.createStyle()][15] method.
*   Set desired styling options.
*   Create an object of _JsonLayoutOptions_ class to set additional options.
*   Import data from JSON to Excel using _JsonUtility.importData()_ method.
*   Save the Excel file using [Workbook.save(string, SaveFormat)][16] method.

The following code sample applies styles when importing data from JSON to Excel in Node.js.

{{< gist aspose-com-gists 2c4dcc027318410c00c7c2fd0c5c702b "json-to-excel-styles.js" >}}

### Output Excel Worksheet



{{< figure align=center src="images/JSON-to-Excel-Formatting.jpg" alt="JSON to XLSX Node.js">}}


## Get a Free License {#Get-a-Free-License}

You can get a [temporary license][17] to use Aspose.Cells for Node.js via Java without evaluation limitations.

## Conclusion

JSON files are immensely used to store and share the data among different applications. Often, you need to export data from JSON files to Excel worksheets. Accordingly, in this article, you have learned how to convert JSON to Excel XLSX/XLS using Node.js. Also, you have seen how to apply formatting in JSON to Excel conversion. In order to explore more about Aspose.Cells for Node.js via Java, visit the [documentation][18]. Furthermore, you can ask your questions via our [forum][19].

## See Also

*   [Convert Excel Files to PDF in Node.js][20]
*   [Create Excel XLSX/XLS Files in Node.js Applications][21]




[1]: https://docs.fileformat.com/web/json/
[2]: #API-for-JSON-to-Excel-Conversion
[3]: #Import-Data-from-JSON-to-Excel-Worksheet
[4]: #Import-JSON-to-Excel-with-Formatting-Styles
[5]: https://products.aspose.com/cells/nodejs-java/
[6]: https://downloads.aspose.com/cells/nodejs
[7]: https://www.npmjs.com/package/aspose.cells
[8]: https://apireference.aspose.com/cells/nodejs/Workbook
[9]: https://apireference.aspose.com/cells/nodejs/WorksheetCollection#get
[10]: https://apireference.aspose.com/cells/nodejs/Workbook#save
[11]: https://apireference.aspose.com/cells/nodejs/Workbook
[12]: https://apireference.aspose.com/cells/nodejs/WorksheetCollection#get
[13]: https://apireference.aspose.com/cells/nodejs/CellsFactory
[14]: https://apireference.aspose.com/cells/nodejs/Style
[15]: https://apireference.aspose.com/cells/nodejs/CellsFactory#createStyle
[16]: https://apireference.aspose.com/cells/nodejs/Workbook#save
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/cells/nodejsjava
[19]: https://forum.aspose.com/
[20]: https://blog.aspose.com/2021/03/05/convert-excel-xlsx-xls-to-pdf-in-node-js/
[21]: https://blog.aspose.com/2020/08/05/create-excel-files-in-node.js/




