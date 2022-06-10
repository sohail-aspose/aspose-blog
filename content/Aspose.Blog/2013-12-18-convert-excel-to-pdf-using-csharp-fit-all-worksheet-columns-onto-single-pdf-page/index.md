---
title: 'C# Excel to PDF - Fit All Worksheet Columns onto Single PDF Page'
date: Wed, 18 Dec 2013 10:12:14 +0000
draft: false
url: /2013/12/18/convert-excel-to-pdf-using-csharp-fit-all-worksheet-columns-onto-single-pdf-page/
author: Amjad Sahi
summary: ''
tags: ['Calculate Excel formulas', 'Embed Ole Objects', 'Encryption', 'Excel Files', 'Fit all worksheet columns in one PDF page', 'Smart Markers', 'advanced conditional formatting', 'export Excel workbooks to PDF', 'generate password protected Excel files', 'hide/unhide rows and columns', 'improved OOXML API', 'manipulate PivotTables', 'render MS Excel file formats', 'render images files from Charts', 'rendering Charts', 'select range of cells', 'web based grid control']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


Aspose.Cells for .NET 7.7.0 has been released. This new release supports [fitting all worksheet columns on single PDF page][1]. This is a useful feature when you want to generate a PDF file that fits all columns on a worksheet onto a single page. We provide PdfSaveOptions.AllColumnsInOnePagePerSheet property which performs complex calculations, such as the height and width of the resultant PDF page to fit all the columns in.

We also provide a feature for [detecting file format type and checking if the file is encrypted][2]. Sometimes you need to detect a file's format before opening it because the file extension does not guarantee that the file content is appropriate. The file might be encrypted (a password-protected file), so it can't be read directly or isn't available to us. Aspose.Cells provide the FileFormatUtil.DetectFileFormat static method and some relevant APIs that you can use to process documents. The following sample code illustrates how to detect a file format (using the file path: you may also use streams) and check its extension.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-ManagingWorkbooksWorksheets-DetectFileFormatAndEncryption-DetectFileFormatAndEncryption.cs" >}}

```
//Detect a file's format type
FileFormatInfo info = FileFormatUtil.DetectFileFormat("e:\\test2\\Book1.xlsx");

//Gets the detected load format
Console.WriteLine("The spreadsheet format is: " + FileFormatUtil.LoadFormatToExtension(info.LoadFormat));

//Check if the file is encrypted or not.
Console.WriteLine("The file is encrypted: " + info.IsEncrypted);
```

## Several Enhancements and Fixes

While [making a hidden column visible][3] you can now restore it to the previously assigned width or its original width. All you need to do is unhide the column with a negative width.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-RowsColumns-Hiding-UnhidingRowsAndColumns-1.cs" >}}

In the new version, we also support double underline while rendering images from sheets and converting Microsoft Excel files to PDF format.

In this release, several important issues have been addressed. For example, issues around rendering Microsoft Excel file formats (XLS, XLSX, ODS, CSV, XLSB etc.), [rendering and manipulating pivot tables][4], [rendering images from Excel worksheets][5], reading and writing HTML files, rendering shapes and controls, Smart Markers, manipulating embedded OLE objects, rendering and manipulating charts, and [exporting Excel workbooks to PDF format][6] have been resolved. A few improvements are also made pertaining to the formula calculation engine of Aspose.Cells for .NET.

We have made a few enhancements regarding auto-adjusting columns and rows and inserting rows in the web-based grid control provided by Aspose.Cells for .NET. Now, you can move left with SHIFT + TAB, or up with SHIFT + ENTER just as in Microsoft Excel. We have also fixed a few issues regarding numbers formatting in GridWeb.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 7.7.0, please visit the [download page][7].




[1]: https://docs.aspose.com/display/cellsnet/Fit+all+Worksheet+Columns+on+single+PDF+page
[2]: https://docs.aspose.com/display/cellsnet/How+to+Detect+a+file+format+and+check+if+the+file+is+Encrypted
[3]: https://docs.aspose.com/display/cellsnet/Hiding+and+Showing+Rows+and+Columns
[4]: https://docs.aspose.com/display/cellsnet/Pivot+Tables
[5]: http://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Image
[6]: http://docs.aspose.com/display/cellsnet/Converting+Excel+to+PDF+Files
[7]: https://downloads.aspose.com/cells/net




