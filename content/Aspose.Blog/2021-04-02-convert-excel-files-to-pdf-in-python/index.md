---
title: 'Convert Excel Files to PDF in Python'
seoTitle: "Convert Excel to PDF in Python | XLSX to PDF, XLS to PDF in Python"
description: "Use Python Excel API to convert Excel files to PDF in Python. Convert XLSX to PDF or XLS to PDF from within your Python applications without MS Office."
date: Fri, 02 Apr 2021 11:31:00 +0000
draft: false
url: /2021/04/02/convert-excel-files-to-pdf-in-python/
author: Usman Aziz
summary: 'Nowadays, [PDF][1] has become a standard file format for exchanging documents. Various popular document formats are converted to PDF before they are shared over the Internet. Excel to PDF is one of the popular conversion scenarios in which worksheets are converted to read-only PDF pages. In accordance with that, this article covers **how to convert Excel XLSX or XLS files to PDF using Python**.'
tags: ['excel to pdf python', 'xls to pdf python', 'xlsx to pdf python']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Convert-Excel-to-PDF.jpg" alt="Excel to PDF Python">}}


Nowadays, [PDF][2] has become a standard file format for exchanging documents. Various popular document formats are converted to PDF before they are shared over the Internet. Excel to PDF is one of the popular conversion scenarios in which worksheets are converted to read-only PDF pages. In accordance with that, this article covers **how to convert Excel XLSX or XLS files to PDF using Python**.

*   [Python Excel to PDF Converter API][3]
*   [Convert Excel XLSX to PDF][4]
*   [Advanced XLSX/XLS to PDF Conversion in Python][5]
*   [Get a Free API License][6]

**Info**: Aspose developed a free online web app that allows you to [view PDFs online][7], another that allows you to [convert PDFs to video][8], and one that allows you to [edit PDFs online][9].

## Python Excel to PDF Converter API {#Python-Excel-to-PDF-Converter-API}

For Excel to PDF conversion, we'll use [Aspose.Cells for Python via Java][10] API. It is a powerful spreadsheet manipulation API that lets you create, process, and convert Excel files from within your Python applications. You can install the API using the following pip command.

*   `pip install aspose-cells`

## Convert Excel XLSX to PDF using Python {#Convert-Excel-XLSX-to-PDF-using-Python}

The following are the steps to convert an Excel XLSX file to PDF using Python.

*   Load the Excel XLSX file using the [Workbook][11] class.
*   Convert XLSX to PDF using [Workbook.save(fileName, SaveFormat.PDF)][12] method.

The following code sample shows how to convert an Excel XSLX file to PDF.

{{< gist aspose-com-gists aa32e346fae9721e49032e37600a339e "xlsx-to-pdf.py" >}}

### Excel File



{{< figure align=center src="images/Excel-to-PDF.jpg" alt="Excel to PDF">}}


### Converted PDF



{{< figure align=center src="images/Excel-to-PDF-Converted.jpg" alt="Converted PDF">}}


## Advanced XLSX/XLS to PDF Conversion in Python {#Advanced-XLSX/XLS-to-PDF-Conversion-in-Python}

Aspose.Cells for Python via Java also allows you to customize the XLSX to PDF conversion using different options. For example, you can set PDF compliance, compression, gridlines style, number of pages per sheet, etc. for the converted PDF file. The [PdfSaveOptions][13] class is used to set these options.

The following are the steps to use advanced options in XLSX to PDF conversion in Python.

*   Load the Excel XLSX file using the [Workbook][14] class.
*   Create an instance of [PdfSaveOptions][15] class.
*   Use _PdfSaveOptions_ object to set options, e.g. set PDF compliance using [PdfOptions.setCompliance(PdfCompliance)][16] method.
*   Save XLSX as PDF using [Workbook.save(fileName, saveOptions)][17] method.

The following code sample shows how to use advanced options in Excel XLSX to PDF conversion.

{{< gist aspose-com-gists aa32e346fae9721e49032e37600a339e "xlsx-to-pdf-advanced.py" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [request a temporary license][18] in order to use the API without evaluation limitations.

## Conclusion

In this article, you have learned how to convert Excel XLSX or XLS to PDF using Python. Furthermore, the advanced options to control the Excel to PDF conversion are also discussed with the help of the code sample. You can explore more about Aspose.Cells for Python via Java using the [documentation][19]. In case you would have any queries, contact us via our [forum][20].

## See Also

*   [Create MS Excel Files using Python – Python Excel API][21]
*   [Read Excel Files in Python][22]
*   [Add Watermark to Excel Files in Python][23]
*   [Add Comments in Excel Worksheets in Python][24]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #Python-Excel-to-PDF-Converter-API
[4]: #Convert-Excel-XLSX-to-PDF-using-Python
[5]: #Advanced-XLSX/XLS-to-PDF-Conversion-in-Python
[6]: #Get-a-Free-API-License
[7]: https://products.aspose.app/slides/viewer/pdf
[8]: https://products.aspose.app/slides/video/pdf
[9]: https://products.aspose.app/slides/editor/pdf
[10]: https://products.aspose.com/cells/python-java/
[11]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[12]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String,%20int)
[13]: https://apireference.aspose.com/cells/python/asposecells.api/PdfSaveOptions
[14]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[15]: https://apireference.aspose.com/cells/python/asposecells.api/PdfSaveOptions
[16]: https://apireference.aspose.com/cells/python/asposecells.api/pdfsaveoptions#Compliance
[17]: https://apireference.aspose.com/cells/python/asposecells.api/workbook#save(java.lang.String,%20com.aspose.cells.SaveOptions)
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/cells/pythonjava/
[20]: https://forum.aspose.com/
[21]: https://blog.aspose.com/2020/08/19/create-excel-xls-xlsx-using-python-excel-api/
[22]: https://blog.aspose.com/2021/12/09/read-excel-files-using-python/
[23]: https://blog.aspose.com/2021/05/07/add-watermark-to-excel-worksheets-in-python/
[24]: https://blog.aspose.com/2021/06/15/add-comments-in-excel-worksheets-using-python/





