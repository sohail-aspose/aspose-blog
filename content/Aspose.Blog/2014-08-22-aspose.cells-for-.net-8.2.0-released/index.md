---
title: 'Aspose.Cells for .NET 8.2.0 Released'
date: Fri, 22 Aug 2014 14:09:21 +0000
draft: false
url: /2014/08/22/aspose.cells-for-.net-8.2.0-released/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for .NET logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png)Aspose.Cells for .NET 8.2.0 has been released. This release contains some useful features and other improvements.  It also includes over 40 fixes and other enhancements. Below, we list some major features and other enhancements in this month’s release.

## Extended Support for Multi-Threading Environment

Aspose.Cells for .NET API is equally useful in multi-threading environment as well as in a single threaded execution plan. However, with recent changes to the core makes the API more reliable to read cell values in multiple threads simultaneously. Aspose.Cells for .NET has exposed the MultiThreadReading property for the Cells class in order to make sure that the correct cell values are always returned when API has to work in a multi-threading environment. For better elaboration, have a look at the detailed article on Simultaneously Reading Cell Values with Multiple Threads.

## Add Useful Overloads to AutoFitRows and AutoFitColumns methods

Now you may also use new overloads (we have included in the new release) i.e., AutoFitRows(int startRow, int endRow, AutoFitterOptions options)/AutoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options) from the list(s) if you need to auto-fit your selected rows/columns with your desired AutoFitterOptions on accordingly.

## Other Enhancements and Fixes

In the new version, we have fixed a few exceptions that occurred while opening Microsoft Excel files. We have fixed the Out of Memory exception while converting and Excel file to PDF file format. We have also improved the performance while manipulating large Excel files.

In this release, several important issues have been addressed. For example, issues around reading/ writing MS Excel files (XLS, XLSX, XLSM, ODS etc.), copying worksheets, manipulating style and formatting in the cells and shapes, rendering and manipulating pivot tables, manipulating shapes and other drawing objects, rendering images from Excel worksheets, manipulating charts, rendering images files from charts, Page Setup options and exporting Excel workbooks to PDF format have been resolved. We have also fixed a few issues regarding Aspose.Cells formula calculation engine.

We have also fixed a few issues in the web based Grid control provided by Aspose.Cells for .NET.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 8.2.0, please visit the [download page][2].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png "Aspose.Cells for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.cells-for-.net/entry566569.aspx




