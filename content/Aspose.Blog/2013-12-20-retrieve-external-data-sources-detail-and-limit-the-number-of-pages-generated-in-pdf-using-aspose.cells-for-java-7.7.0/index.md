---
title: 'Retrieve External Data Source Details and Limit the Number of Pages Generated in PDF with Aspose.Cells for Java 7.7.0'
date: Fri, 20 Dec 2013 09:29:11 +0000
draft: false
url: /2013/12/20/retrieve-external-data-sources-detail-and-limit-the-number-of-pages-generated-in-pdf-using-aspose.cells-for-java-7.7.0/
author: Amjad Sahi
summary: ''
tags: ['Calculate Excel formulas', 'Chart to Image', 'Excel Files', 'Excel to PDF', 'Limit the number of pages generated', 'OOXML API', 'Sheet to Image', 'export Excel workbooks to PDF', 'render MS Excel file formats', 'render images files from Charts', 'rendering Charts', 'retrieve External Data Sources Details']
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for Java logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Cells-for-Java_100.png)We are pleased to announce the release of Aspose.Cells for Java 7.7.0. In this release, we have added a feature that lets you retrieve external data source details. Sometimes, you may want to retrieve details from external data sources, for example if you want to read the SQL connection data. This may include any or all type of data that is required to establish a connection with an SQL Server, such as the server URL, user name, underlying table name, SQL query, query type, the location of the table, etc.

In the new version, you can limit the number of pages generated in Excel to PDF conversion. You can print a range of pages to the output PDF file using this new feature. Aspose.Cells allows you to set a limit on how many pages are generated when converting a Microsoft Excel spreadsheet to PDF file format. The following sample code illustrates how to limit the number of pages in the output PDF file that is generated from an Excel template file.

```
//Open an Excel file
Workbook wb = new Workbook("Sample1.xlsx");
//Instantiate the PdfSaveOption
PdfSaveOptions options = new PdfSaveOptions();

//Print only Page 3 and Page 4 in the output PDF
//Starting page index (0-based index)
options.setPageIndex(2); 
//Number of pages to be printed
options.setPageCount(2);

//Save the PDF file
wb.save("outPDF1.pdf", options); 
```

We have also added a number of enhancements in the new release. We have improved the chart to image and [sheet to image][2] modules.

This release is also a maintenance release that contains fixes for issues reported in earlier versions. In this release, we have fixed the issues with manipulating charts and shapes. Several other important issues have also been addressed. For example, issues to do with rendering Microsoft Excel file formats, rendering images from Excel worksheets, rendering shapes and controls and exporting Excel workbooks to PDF format have been resolved. A few improvements have also been made to Aspose.Cells for Jav's formula calculation engine.

To see a complete list of enhancements and fixes and to download Aspose.Cells for Java 7.7.0, please visit the [download page][3].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Cells-for-Java_100.png "Aspose.Cells for Java logo"
[2]: https://blog.aspose.com/
[3]: http://www.aspose.com/community/files/72/java-components/aspose.cells-for-java/entry514784.aspx




