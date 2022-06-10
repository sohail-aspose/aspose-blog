---
title: 'Read Encrypted Microsoft Excel 2013 Files, Unhide Rows/Columns to their Original Height/Width and More in Aspose.Cells for Java 7.7.2'
date: Wed, 19 Feb 2014 10:46:04 +0000
draft: false
url: /2014/02/19/read-encrypted-microsoft-excel-2013-files-unhide-rowscolumns-to-their-original-heightwidth-and-other-enhancements-in-aspose.cells-for-java-7.7.2/
author: Amjad Sahi
summary: ''
tags: ['Calculate Excel formulas', 'Encryption', 'Excel Files', 'advanced conditional formatting', 'export Excel workbooks to PDF', 'improved OOXML API', 'manipulate PivotTables', 'render MS Excel file formats', 'render images files from Charts', 'rendering Charts']
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for Java logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Cells-for-Java_100.png)We are pleased to announce the release of Aspose.Cells for Java 7.7.2 with new features, enhancements and bug fixes. This new release supports reading password protected Microsoft Excel 2013 files. We provide the Style.setJustifyDistributed() method so you can apply the justify distributed setting while applying text alignment settings on cells.

We also provide support for B3 (13.9 x 19.7 inches) and Business Card (90 mm x 55 mm) PaperSizeType.

We have enhanced the unhiding rows/columns feature in this release. While making a hidden column or row visible, if you want to restore it to previously assigned width/height or to its original width/height, you can unhide the column or row with a negative width/height. For example, worksheet.getCells().unhideColumn(5, -1);

Moreover, we have removed the hard coded use of the com.sun.image.codec.jpeg.JPEGCodec API.

## Enhancements and Fixes

We have added a number of enhancements and fixes in the new release. For example, you can now print comments in a Microsoft Excel document while rendering to PDF.We have improved the chart to image and [sheet to image][2] modules and fixed issues with manipulating charts and shapes.

Several other important issues have also been addressed. Issues to do with exporting Excel workbooks to PDF format have been resolved. A few other improvements are also made to Aspose.Cells for Java's formula calculation engine. We have fixed a few exceptions when reading and writing Microsoft Excel file formats too.

To see a complete list of enhancements and fixes and to download Aspose.Cells for Java 7.7.2, please visit the [download page][3].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Cells-for-Java_100.png "Aspose.Cells for Java logo"
[2]: https://blog.aspose.com/
[3]: http://www.aspose.com/community/files/72/java-components/aspose.cells-for-java/entry526139.aspx




