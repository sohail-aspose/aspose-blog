---
title: 'Adjust Excel Workbook Compression Level using C#'
date: Tue, 29 Oct 2019 15:34:08 +0000
draft: false
url: /2019/10/29/adjust-workbook-compression-level-with-aspose.cells-for-.net-19.9/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

Guys, in the blog you will learn how to adjust the workbook compression level. You can also avail the useful feature to print multiple copies of a workbook and support for reading and rendering controls of ODS file. We suggest you to have a look at the release notes to get the complete list of features, enhancements and other fixes which are part of this new release. Let's not wait another moment to review the [release notes][1].  To get essence of the public release ([Aspose.Cells for .NET v19.9][2], I am giving you preview of the new features and other enhancements available in it.

## Adjust Excel Workbook Compression Level using C#

The compression level of the workbook is an important factor while working with larger workbooks. You should have control over setting the priority to create either small file with little more time or create files quickly but having a comparatively large file size. Aspose.Cells have now provided this control such that the developer will have the control to adjust the compression level. A new enumerator [OoxmlCompressionType][3] is provided which can be used to set the compression level. Following members are available under this enumerator.

*   **Level1**: The fastest but least effective compression.
*   **Level2**: A little slower, but better, than level 1.
*   **Level3**: A little slower, but better, than level 2.
*   **Level4**: A little slower, but better, than level 3.
*   **Level5**: A little slower than level 4, but with better compression.
*   **Level6**: A good balance of speed and compression efficiency.
*   **Level7**: Pretty good compression!
*   **Level8**: Better compression than Level7!
*   **Level9**: The "best" compression, where best means greatest reduction in the size of the input data stream. This is also the slowest compression.

Following example can be used to exercise this new exciting feature by changing the compression type and comparing the file size with the time taken to create this file.

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-Workbook-AdjustCompressionLevel-1.cs" >}}  
See the document [Adjust workbook compression level][4] for your reference.

## Print Multiple Copies of a Worksheet

Aspose.Cells provides the ability to print multiple copies of a worksheet by using the **SheetRender.ToPrinter(PrintSettings PrinterSettings)** method/overload. The following code snippet demonstrates the use of SheetRender.ToPrinter(PrintSettings PrinterSettings) method to print multiple copies of a worksheet.

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-Worksheets-PrintSheetWithAdditionalSettings-1.cs" >}}  
See the document [Print multiple copies of a worksheet][5] for your reference.

## Other Enhancements and Fixes

*   Support reading and rendering Control of ODS files.
*   PivotTables did not retain multiple select options after processing smart markers.
*   Hyperlinks lost when importing data from DataTable.
*   Contents overflow from the page during PDF conversion.
*   Setting the font and font size of Drawing.TextBox was not working in ODS.
*   Fixed an issue where OLE object link was not accessible from XLS file.
*   Filter connections on pivot chart lost settings on save after refreshing pivot tables.
*   The setting “Hide items with no data” in slicer lost after refreshing pivot tables.




[1]: https://docs.aspose.com/cells/net/aspose-cells-for-net-19-9-release-notes/
[2]: https://www.nuget.org/packages/Aspose.Cells/19.9.0)
[3]: https://apireference.aspose.com/net/cells/aspose.cells/ooxmlcompressiontype
[4]: https://docs.aspose.com/cells/net/adjust-workbook-compression-level/
[5]: https://docs.aspose.com/cells/net/print-multiple-copies-of-a-worksheet/




