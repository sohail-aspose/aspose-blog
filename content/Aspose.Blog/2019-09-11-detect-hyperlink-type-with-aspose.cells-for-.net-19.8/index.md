---
title: 'Detect Hyperlink Type in Excel with Aspose.Cells for .NET'
date: Wed, 11 Sep 2019 11:33:39 +0000
draft: false
url: /2019/09/11/detect-hyperlink-type-with-aspose.cells-for-.net-19.8/
author: Amjad Sahi
summary: ''
tags: ['detect hyperlink type in excel', 'hyperlink in xlsx']
categories: ['Aspose.Cells Product Family']
---

[![Hyperlink type in XLSX][1]](https://www.aspose.com/products/cells/net "Aspose.Cells for .NET API") Guys, in the blog you will learn how to categorize hyperlinks in order to select the appropriate method for processing each of these links. You may also explore and extract embedded MOL file. Moreover, we now provide a solution when rendering bigger files (having millions of pages in the sheet(s)). You may get total pages count before converting to PDF/Image, This is a good thing to know to decide whether to render or not to render. You may have a look at the release notes to get the complete list of features and bug fixes which are part of this new release. So let's not wait another moment to review the [release notes][2].  To get essence of the public release ([Aspose.Cells for .NET v19.8][3], I am giving you preview of the new features and other enhancements available in it.  

## Detect Hyperlink TypeThere can be different types of hyperlinks which can be used in an Excel file like external, cell reference, file path and email. Our new release has introduced an enumerator **TargetModeType** which represents the type of hyperlink. A new property **LinkType** is introduced in Hyperlink class which return the hyperlink type using above mentioned enumerator. See the document on how to [detect different types of hyperlinks][4] for your complete reference. Here is an example which can be used to exercise this new feature. \[gist id="922f990b02cf4e04a328bd6f37029af8" file="Examples-CSharp-Workbook-DetectLinkTypes-1.cs"\]



{{< figure align=center src="images/Screenshot-2019-09-03-at-8.43.27-PM-1024x446.png" alt="Hyperlink in Excel" caption="Program output vs template Excel file">}}


## Get Total Page Count before PDF or Image RenderingWell, the title is explaining this new feature. When a file has too many pages, the process of converting to pdf/image may use too much memory and CPU, and OOM exception may be thrown. Getting total pages count before converting can indicate this risk, and do some actions (e.g. skip this file) or print the selected pages to avoid the undesired results. For example one of my sample Excel file (870 KB) was showing about 38 million pages. Just imagine, what will happen if you come across a conversion containing such a huge number of pages. Following is an example to show the usage of new classes **SheetPrintingPreview** and **WorkbookPrintingPreview**. Both of these classes contain a property **EvaluatedPageCount** which returns the page count of the printout or PDF file. \[gist id="922f990b02cf4e04a328bd6f37029af8" file="Examples-CSharp-Workbook-PrintPreview-1.cs"\] See the document on [printing preview workbook and worksheet][5] for your complete reference.

## Extracting Embedded MOL FileAs you know that molecular data file created in the MDL Molfile format, a chemical file format; contains plain text information and stores information about atoms and bonds; often used as a standard exchange format for molecular information. This type of file can be embedded in the Excel file. In this latest release, support is provided to extract object of such an uncommon type i.e. MOL. The following code snippet demonstrates extracting embedded MOL file and saving it to disk. \[gist id="922f990b02cf4e04a328bd6f37029af8" file="Examples-CSharp-Workbook-ExtractEmbeddedMolFile-1.cs"\] See the document [on extract embedded MOL file][6] for your reference.

## Other Enhancements and Fixes

*   An enhancement is made to Aspose.Cells.GridWeb for compatibility with MVC.
*   Improved performance for calculating large matrix with double values.
*   The document fails to save when saved more than 10 times.
*   Handled an exception when getting image from SheetRender for encrypted ODS file.
*   Handled an excetion when calculating charts on an excel with a number > int.MaxValue.
*   Fixed the error "IndexOutOfRangeException" when using smart marker with a pivot table and saving the workbook.
*   Fixed an error "Index was outside the bounds of the array" while converting XLSX to PDF.
*   Fixed an error "Invalid MsoLineDashStyle string val" when loading an XLSX file format.

To use these features and avail other enhancements and fixes, I recommend you to try the release [Aspose.Cells for .NET v19.8][7]. Moreover, I recommend you to browse [Developers’ Guide][8] for your complete reference on what you can deliver using the APIs. Also, you are always welcome to share your review, concerns or feedback on [forums][9].



[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png "Aspose.Cells for .NET logo"
[2]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+19.8+Release+Notes
[3]: https://www.nuget.org/packages/Aspose.Cells/19.8.0)
[4]: https://docs.aspose.com/display/cellsnet/Detect+Hyperlink+Type
[5]: https://docs.aspose.com/display/cellsnet/Workbook+and+Worksheet+Print+Preview
[6]: https://docs.aspose.com/display/cellsnet/Managing+OLE+Objects#ManagingOLEObjects-ExtractingEmbeddedMOLFile
[7]: https://downloads.aspose.com/cells/net/new-releases/aspose.cells-for-.net-19.8/
[8]: https://docs.aspose.com/display/cellsnet/Developer+Guide
[9]: https://forum.aspose.com/c/cells




