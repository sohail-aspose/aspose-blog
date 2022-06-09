---
title: 'Convert Excel Files to PDF in Node.js'
seoTitle: "Convert Excel to PDF in Node.js | XLSX to PDF or XLS to PDF in Node.js"
description: "Use Node.js spreadsheet manipulation API to convert Excel files to PDF. Convert XLSX to PDF or XLS to PDF in Node.js using advanced conversion options."
date: Fri, 05 Mar 2021 11:24:00 +0000
draft: false
url: /2021/03/05/convert-excel-xlsx-xls-to-pdf-in-node-js/
author: Usman Aziz
summary: 'Excel spreadsheets are commonly used to store and analyze data in the form of rows and columns. However, in various cases, you need to convert the Excel files to PDF before sharing them over the internet. In order to automate Excel to PDF conversion, this article shows **how to convert Excel files to PDF programmatically using Node.js**. Furthermore, advanced options to customize the Excel to PDF conversion are also discussed.'
tags: ['excel to pdf nodejs', 'xls to pdf nodejs', 'xlsx to pdf nodejs']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Convert-Excel-to-PDF.jpg" alt="Convert Excel to PDF in Node.js">}}


Excel spreadsheets are commonly used to store and analyze data in the form of rows and columns. However, in various cases, you need to convert the Excel files to PDF before sharing them over the internet. In order to automate Excel to PDF conversion, this article shows **how to convert Excel files to PDF programmatically using Node.js**. Furthermore, advanced options to customize the Excel to PDF conversion are also discussed.

*   [Node.js Excel to PDF Conversion API][1]
*   [Convert Excel XLSX/XLS to PDF][2]
*   [Advanced Options for Excel XLSX/XLS to PDF][3]
*   [Get a Free API License][4]

## Node.js Excel to PDF Conversion API {#Node.js-Excel-to-PDF-API}

For converting the Excel XLSX/XLS files to PDF, we will use [Aspose.Cells for Node.js via Java][5]. It is a spreadsheet manipulation API that lets you create, read, modify, and convert Excel workbooks seamlessly. You can either [download][6] the API's package or install it use the following [NPM][7] command.

```
> npm install aspose.cells 
```

## Convert Excel XLSX to PDF in Node.js {#Convert-Excel-to-PDF-in-Node.js}

The following are the steps to convert Excel XLSX or XLS files to PDF.

*   Load the Excel file using [Workbook][8] class.
*   Convert Excel file to PDF using [Workbook.save(string, SaveFormat.PDF)][9] method.

The following code sample shows how to convert an Excel XLSX file to PDF.

{{< gist aspose-com-gists 60db4d77167381399d6be40b2b949a07 "excel-to-pdf.js" >}}

### Excel File



{{< figure align=center src="images/Excel-to-PDF.jpg" alt="Node.js Excel to PDF">}}


### Converted PDF



{{< figure align=center src="images/Excel-to-PDF-Converted.jpg" alt="Excel to PDF">}}


## Excel XLSX/XLS to PDF - Advanced Options {#Advanced-Options-for-Excel-XLSX/XLS-to-PDF}

Aspose.Cells also allows you to control the Excel to PDF conversion using different options. For example, you can set PDF compliance, compression, gridlines style, number of pages per sheet, etc. To customize the conversion, the API provides [PdfSaveOptions][10] class.

The following are the steps to convert an Excel file to PDF with advanced options.

*   Load the Excel file using [Workbook][11] class.
*   Create an object of [PdfSaveOptions][12] class.
*   Set the desired options e.g. PDF compliance using [PdfOptions.setCompliance(PdfCompliance)][13] method.
*   Save Excel file as PDF using [Workbook.save(string, PdfSaveOptions)][14] method.

The following code sample shows how to convert Excel to PDF using advanced options.

{{< gist aspose-com-gists 60db4d77167381399d6be40b2b949a07 "excel-to-pdf-advance.js" >}}

## Get a Free API License {#Get-a-Free-API-License}

In order to use the API without evaluation limitations, you can [request a free temporary license][15].

## Conclusion

In this article, you have learned how to convert Excel files to PDF within Node.js applications. Furthermore, you have seen how to control Excel to PDF conversion using advanced options. You can explore more about the Node.js Excel API using the [documentation][16]. Furthermore, you can contact us via our [forum][17] in case of any query.

## See Also

*   [Create Excel XLSX/XLS Files in Node.js Applications – A Complete Guide][18]




[1]: #Node.js-Excel-to-PDF-API
[2]: #Convert-Excel-to-PDF-in-Node.js
[3]: #Advanced-Options-for-Excel-XLSX/XLS-to-PDF
[4]: #Get-a-Free-API-License
[5]: https://products.aspose.com/cells/nodejs-java
[6]: https://downloads.aspose.com/cells/nodejs
[7]: https://www.npmjs.com/package/aspose.cells
[8]: https://apireference.aspose.com/cells/nodejs/Workbook
[9]: https://apireference.aspose.com/cells/nodejs/Workbook#save
[10]: https://apireference.aspose.com/cells/nodejs/PdfSaveOptions
[11]: https://apireference.aspose.com/cells/nodejs/Workbook
[12]: https://apireference.aspose.com/cells/nodejs/PdfSaveOptions
[13]: https://apireference.aspose.com/cells/nodejs/PdfSaveOptions#setCompliance
[14]: https://apireference.aspose.com/cells/nodejs/Workbook#save
[15]: https://purchase.aspose.com/temporary-license
[16]: https://docs.aspose.com/cells/nodejsjava/
[17]: https://forum.aspose.com/
[18]: https://blog.aspose.com/2020/08/05/create-excel-files-in-node.js/





