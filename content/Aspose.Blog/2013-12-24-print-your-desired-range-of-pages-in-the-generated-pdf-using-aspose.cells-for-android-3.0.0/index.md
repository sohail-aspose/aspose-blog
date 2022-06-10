---
title: 'Print a Range of Excel Sheets to PDF using Aspose.Cells for Android 3.0.0'
date: Tue, 24 Dec 2013 12:34:24 +0000
draft: false
url: /2013/12/24/print-your-desired-range-of-pages-in-the-generated-pdf-using-aspose.cells-for-android-3.0.0/
author: Amjad Sahi
summary: ''
tags: ['Calculate Excel formulas', 'Chart to Image', 'Excel Files', 'Excel to PDF', 'Limit the number of pages generated', 'OOXML API', 'Sheet to Image', 'export Excel workbooks to PDF', 'render MS Excel file formats', 'render images files from Charts', 'rendering Charts', 'retrieve External Data Sources Details']
categories: ['Aspose.Cells Product Family']
---

We are pleased to announce the release of Aspose.Cells for Android 3.0.0. In this release, you can [print a desired number of pages generated in Microsoft Excel to PDF][1]. Aspose.Cells allows you to specify how many pages are generated when converting an Excel spreadsheet to PDF file format. The following sample code illustrates on how to limit the number of pages in the output PDF file that is generated from an Excel template file:

```
String sdCardPath = Environment.getExternalStorageDirectory().getPath()+ File.separator; CellsHelper.setFontDir(sdCardPath + "fonts"); 
//Open an Excel file
Workbook wb = new Workbook(sdCardPath + "Book1.xlsx"); 
//Instantiate the PdfSaveOption 
PdfSaveOptions options = new PdfSaveOptions();
//Print only Page 3 and Page 4 in the output PDF
//Starting page index (0-based index)
options.setPageIndex(2);
//Number of pages to be printed
options.setPageCount(2);
//Save the PDF file
wb.save(sdCardPath + "outPDF1.pdf", options); 
```

We now also support retrieving external d[a][2]ta source details. For example, you may want to read out SQL connection data. This may include any or all type of data that is required to establish a connection with SQL Server, for example the server's URL, user name, underlying table name, SQL query, query type, the location of the table, and so on.

We have also done a number of enhancements in the new release. We have improved the Excel to PDF, chart to image and sheet to image modules. We have enhanced the performance of these features in the new release as well. Moreover, certain improvements are also made pertaining to the formula calculation engine of Aspose.Cells for Android.

To see a complete list of enhancements and fixes and to download Aspose.Cells for Android 3.0.0, please visit the [download page][3].




[1]: https://docs.aspose.com/cells/java/limit-the-number-of-pages-generated-excel-to-pdf-conversion/
[2]: https://docs.aspose.com/cells/java/retrieving-external-data-sources-details/
[3]: http://www.aspose.com/community/files/74/android-components/aspose.cells-for-android/entry515659.aspx




