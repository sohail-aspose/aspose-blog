---
title: 'Convert Excel Files to HTML in Node.js'
seoTitle: "Convert Excel to HTML in Node.js | XLSX or XLS to HTML in Node.js"
description: "Convert Excel files to HTML in Node.js applications. Perform XLS or XLSX to HTML with additions options to enable tooltips, gridlines, hidden sheets, etc."
date: Thu, 11 Feb 2021 03:10:00 +0000
draft: false
url: /2021/02/11/convert-excel-files-to-html-in-node-js/
author: Usman Aziz
summary: 'Excel files are widely used to store and organize the data in the form of worksheets. Furthermore, you can perform various computations as well as analysis of the data. However, in certain cases, you have to convert the Excel files into other formats. For example, you may need to convert an Excel worksheet to HTML or image in order to display it within your web or desktop application. For such cases, this article covers **how to convert Excel files to HTML in Node.js applications**. In addition, you will learn how to use additional options to customize the converted HTML.'
tags: ['excel to html nodejs', 'xls to html nodejs', 'xlsx to html nodejs']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Excel-to-HTML-Logo.jpg" alt="C++ Excel to HTML">}}


Excel files are widely used to store and organize the data in the form of worksheets. Furthermore, you can perform various computations as well as analysis of the data. However, in certain cases, you have to convert the Excel files into other formats. For example, you may need to convert an Excel worksheet to HTML or image in order to display it within your web or desktop application. For such cases, this article covers **how to convert Excel files to HTML in Node.js applications**. In addition, you will learn how to use additional options to customize the converted HTML.

*   [Node.js Excel to HTML Converter API][1]
*   [Convert Excel Files to HTML in Node.js][2]
*   [Enable Gridlines in Excel to HTML Conversion][3]
*   [Show Tooltip in Excel to HTML Conversion][4]
*   [Include Hidden Sheets in Excel to HTML Conversion][5]
*   [Get a Free API License][6]

## Node.js Excel to HTML Converter API {#Node.js-Excel-to-HTML-Converter-API}

[Aspose.Cells for Node.js via Java][7] API is designed to implement spreadsheet automation from within your Node.js applications. It provides a range of features to manipulate Excel files seamlessly. Furthermore, the API allows you to convert Excel files to other formats. In order to use the API, you can download its package from the [Downloads][8] section or use the following [NPM][9] command.

```
> npm install aspose.cells
```

## Convert Excel Files to HTML in Node.js {#Convert-Excel-Files-to-HTML-in-Node.js}

When converting an Excel file to HTML, Aspose.Cells for Node.js via Java creates a separate tab for each worksheet. Thus, you can navigate between the sheets quite easily. The following are the steps to convert an Excel file to HTML.

*   Load Excel file using [Workbook][10] class.
*   Save Excel file as HTML using [Workbook.save(String)][11] method.

The following code sample shows how to convert an Excel file to HTML using Node.js.

{{< gist aspose-com-gists 84db0c74a505955c066e28e16e72a5d0 "excel-to-html.js" >}}

### Excel File



{{< figure align=center src="images/Excel-File.jpg" alt="Excel File">}}


### Converted HTML



{{< figure align=center src="images/Excel-to-HTML.jpg" alt="Excel to HTML">}}


## Enable Gridlines in Excel to HTML Conversion in Node.js {#Enable-Gridlines-in-Excel-to-HTML-Conversion}

By default, the gridlines are disabled in the converted HTML file. However, you can enable them using the [HtmlSaveOptions][12] class. The following are the steps to perform this operation.

*   Load XLSX file using [Workbook][13] class.
*   Create an instance of [HtmlSaveOptions][14] class.
*   Enable gridlines using [HtmlSaveOptions.setExportGridLines(true)][15] method.
*   Save converted HTML using [Workbook.save(String, HtmlSaveOptions)][16] method.

The following code sample shows how to enable gridlines in Excel to HTML conversion.

{{< gist aspose-com-gists 84db0c74a505955c066e28e16e72a5d0 "excel-to-html-gridlines.js" >}}

### Converted HTML



{{< figure align=center src="images/Excel-to-HTML-Gridlines.jpg" alt="Excel to HTML GrdiLines">}}


## Enable Tooltip in XLSX to HTML Conversion in Node.js {#Show-Tooltip-in-Excel-to-HTML-Conversion}

In some cases, the values may exceed the width of the cells in a worksheet. In such situations, you can enable the tooltips to display complete text in the converted HTML. The following are the steps to enable tooltips in Excel to HTML conversion.

*   Load Excel file using [Workbook][17] class.
*   Create an instance of [HtmlSaveOptions][18] class.
*   Use [HtmlSaveOptions.setAddTooltipText(true)][19] method to enable tooltip.
*   Save Excel file as HTML using [Workbook.save(String, HtmlSaveOptions)][20] method.

The following code sample shows how to enable tooltip in Excel to HTML conversion in Node.js.

{{< gist aspose-com-gists 84db0c74a505955c066e28e16e72a5d0 "excel-to-html-tooltip.js" >}}

## Include Hidden Sheets in XLS/XLSX to HTML Conversion {#Include-Hidden-Sheets-in-Excel-to-HTML-Conversion}

Excel workbooks may also contain the hidden sheets that are not included in Excel to HTML conversion by default. In order to render hidden sheets, you can use [HtmlSaveOptions.setExportHiddenWorksheet()][21] method. The following are the steps to perform this operation.

*   Load XLSX file using [Workbook][22] class.
*   Create an instance of [HtmlSaveOptions][23] class.
*   Include hidden sheets using [HtmlSaveOptions.setExportHiddenWorksheet(true)][24] method.
*   Save converted HTML using [Workbook.save(String, HtmlSaveOptions)][25] method.

The following code sample shows how to include hidden sheets in Node.js Excel to HTML conversion.

{{< gist aspose-com-gists 84db0c74a505955c066e28e16e72a5d0 "excel-to-html-hidden-sheets.js" >}}

## Get a Free API License {#Get-a-Free-API-License}

In case you want to try the API without evaluation limitations, you can [get a free temporary license][26].

## Conclusion

Excel to HTML conversion is often used in web applications to display worksheets on web pages. In accordance with that, this article has covered how to convert Excel workbooks to HTML files in Node.js. Furthermore, you have seen how to customize the Excel to HTML conversion with different options. You can explore more about Aspose.Cells for Node.js via Java using [documentation][27].

## See Also

*   [Create Excel Files in Node.js Applications – A Complete Guide][28]




[1]: #Node.js-Excel-to-HTML-Converter-API
[2]: #Convert-Excel-Files-to-HTML-in-Node.js
[3]: #Enable-Gridlines-in-Excel-to-HTML-Conversion
[4]: #Show-Tooltip-in-Excel-to-HTML-Conversion
[5]: #Include-Hidden-Sheets-in-Excel-to-HTML-Conversion
[6]: #Get-a-Free-API-License
[7]: https://products.aspose.com/cells/nodejs-java
[8]: https://downloads.aspose.com/cells/nodejs
[9]: https://www.npmjs.com/package/aspose.cells
[10]: https://apireference.aspose.com/cells/nodejs/Workbook
[11]: https://apireference.aspose.com/cells/nodejs/Workbook#save
[12]: https://apireference.aspose.com/cells/nodejs/HtmlSaveOptions
[13]: https://apireference.aspose.com/cells/nodejs/Workbook
[14]: https://apireference.aspose.com/cells/nodejs/HtmlSaveOptions
[15]: https://apireference.aspose.com/cells/nodejs/HtmlSaveOptions#setExportGridLines
[16]: https://apireference.aspose.com/cells/nodejs/Workbook#save
[17]: https://apireference.aspose.com/cells/nodejs/Workbook
[18]: https://apireference.aspose.com/cells/nodejs/HtmlSaveOptions
[19]: https://apireference.aspose.com/cells/nodejs/HtmlSaveOptions#setAddTooltipText
[20]: https://apireference.aspose.com/cells/nodejs/Workbook#save
[21]: https://apireference.aspose.com/cells/nodejs/HtmlSaveOptions#setExportHiddenWorksheet
[22]: https://apireference.aspose.com/cells/nodejs/Workbook
[23]: https://apireference.aspose.com/cells/nodejs/HtmlSaveOptions
[24]: https://apireference.aspose.com/cells/nodejs/HtmlSaveOptions#setExportHiddenWorksheet
[25]: https://apireference.aspose.com/cells/nodejs/Workbook#save
[26]: https://purchase.aspose.com/temporary-license
[27]: https://docs.aspose.com/cells/nodejsjava/
[28]: https://blog.aspose.com/2020/08/05/create-excel-files-in-node.js/





