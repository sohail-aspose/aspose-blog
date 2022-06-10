---
title: 'Resample Images in Excel to PDF Conversion and Other Enhancements in Aspose.Cells for .NET 7.6.0'
date: Wed, 23 Oct 2013 19:24:38 +0000
draft: false
url: /2013/10/23/resampling-of-the-images-in-excel-to-pdf-conversion-supported-along-with-other-valuable-enhancements-included-in-aspose.cells-for-.net-7.6.0/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for .NET logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png)Aspose.Cells for .NET 7.6.0 has been released. The new release lets you select a different paper source when printing worksheets. Moreover, the collection objects are now Lambda/Linq friendly. We have added some significant enhancements for reading non-native Microsoft Excel files: now the component throws the appropriate exception when loading such files. We have improved the module for inserting OLE objects.

This release, also supports resampling images added to PDF documents to reduce the overall file size and improve performance. So, if you want to compress images while saving Excel to PDF format, you may use the feature, see the sample code below:

```
 Workbook workbook = new Workbook(filename);
PdfSaveOptions options = new PdfSaveOptions();
options.SetImageResample(300, 70);
workbook.Save(“out.pdf”, options); 
```

We have fixed a few exceptions as well when reading/writing Excel files and refreshing pivot tables in the template files.

In this release, several important issues have been addressed. For example, issues around rendering Microsoft Excel file formats, rendering and manipulating pivot tables, converting Excel files to HTML format, rendering and manipulating charts, rendering image files from charts and exporting Excel workbooks to PDF format have been resolved. A few improvements are also made pertaining to the formula calculation engine.

We have made a few enhancements and fixed some bugs regarding context menu in IE8 browser type. We fix an issue for the **Undo** button while calculating formulas in the web based Grid control provided by Aspose.Cells for .NET.  We also included a few enhancements regarding formula calculations and formatting while importing Excel file in the desktop based Grid control provided by Aspose.Cells for .NET.

To see a complete list of enhancements and fixes and to download Aspose.Cells for .NET 7.6.0, please visit the [download page][2].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png "Aspose.Cells for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.cells-for-.net/entry502011.aspx




