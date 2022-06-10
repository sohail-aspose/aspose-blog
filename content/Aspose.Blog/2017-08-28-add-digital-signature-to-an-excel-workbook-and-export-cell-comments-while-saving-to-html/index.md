---
title: 'Add Digital Signature to an Excel Workbook and Export Cell Comments while saving to HTML - Aspose.Cells for .NET 17.8'
date: Mon, 28 Aug 2017 12:14:28 +0000
draft: false
url: /2017/08/28/add-digital-signature-to-an-excel-workbook-and-export-cell-comments-while-saving-to-html/
author: Amjad Sahi
summary: ''
tags: ['Add digital signatures to Excel', 'Sign Excel in CSharp']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce the release of [Aspose.Cells for .NET v17.8][1]. This release includes a few valuable features and other enhancements along with critical bug fixes that further improve the overall stability of the APIs. Please check the [release notes][2] in order to get an idea about what is new and what has been enhanced or fixed with this revision of Aspose.Cells for .NET. You can also install [Aspose for .NET APIs directly from NuGet repository][3].

## Add Digital Signature to Excel File in C#

Aspose.Cells provides the _Workbook.AddDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)_ method that lets you to add digital signature to an already signed Excel file.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Workbook-AddDigitalSignatureToAnAlreadySignedExcelFile.cs" >}}

Please see the document/article (with attachments) that explains on how to add Digital Signature to an already signed Excel file for your complete reference.

*   [Add Digital Signature to an already signed Excel file][4]

## Disable Downlevel Revealed Comments while saving to HTML

When you save your Excel file to HTML, then Aspose.Cells reveals Downlevel conditional comments. These conditional comments are mostly relevant to older versions of Internet Explorer and are irrelevant to modern web browsers. Aspose.Cells allows you to eliminate these Downlevel Revealed Comments by setting the `HtmlSaveOptions.DisableDownlevelRevealedComments` property to true. For more detail, please see this article.

*   Disable Downlevel Revealed Comments while saving to HTML

## Export Comments while Saving Excel file to Html

When you save your Excel file into HTML, comments are not exported by default. However, Aspose.Cells allows you to export comments in the output HTML using the `HtmlSaveOptions.IsExportComments` property. If you set it true, then HTML will also display comments present in your Excel file. the following document/article for your reference.

*   Export Comments while Saving Excel file to Html

## Output Blank Page when there is Nothing to Print

If a sheet is empty, then Aspose.Cells will not print anything when you export worksheet to image format. You can change this behavior by using the `ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint` property. When you will set it to true, it will print the blank page. For more detail, please see this article.

*   [Output Blank Page when there is Nothing to Print][5]

## Using CustomImplementationFactory to create custom implementation of Memory Stream

Aspose.Cells provides an API named `CellsHelper.CustomImplementationFactory` which enables you to provide custom implementation, such as using Recyclable memory implementation instead of the default MemoryStream. This feature is useful when the memory is not contiguous in your environment. For more detail, please see this article.

*   [Using CustomImplementationFactory to create custom implementation of Memory Stream][6]

## Create, Remove and Get GridCell Comments - Aspose.Cells.GridWeb

The web based grid control provided by Aspose.Cells for .NET allows you to create, remove and get cell comments inside the worksheet. For more detail, please see this article.

*   [Create Remove and Get GridCell Comments][7]

## Other Enhancements and Fixes

There are some important enhancements included in the new release for the users. A few of the worth mentioning features/enhancements are as follow.

*   [Default Font and Font Color of the GridDesktop][8].
*   Handled "Shape to image Error" when rendering a XLSX file to PDF file format .
*   Handled NullReferenceException when opening an Excel file.
*   Handled an exception on opening the template XLSB file (Office 365 (1707 update)).

Aspose.Cells 17.8 has enhanced its core for more stability as well as fixed many critical bugs. In this release, we have fixed several other issues. For example, issues around reading/writing MS Excel file formats(XLS, XLSX, XLSB, ODS, SpreadsheetML etc.), grouping rows and columns, applying data validation, rendering shapes and drawing objects, manipulating ListObjects/Tables, reading and rendering HTML, rendering and manipulating charts, manipulating PivotTables, [rendering images from Excel worksheets][9], [rendering images files from charts][10] and [exporting Excel workbooks to PDF format][11] have been resolved.

## Changes to the Public API

This version of Aspose.Cells for .NET has made some changes to the Public API. A few of the worth mentioning changes are as follow:

*   Added _HtmlSaveOptions.IsExportComments_ property, it indicates if exporting comments when saving file to HTML, the default value is false.
*    Added _HtmlSaveOptions.DisableDownlevelRevealedComments_ property, it indicates if disabling Downlevel-revealed conditional comments when exporting file to HTML, the default value is false.
*   Added _CustomImplementationFactory_ class, it provides an API for the user to extend/improve the component's ability by some special implementations for some special situations. For example, when there is enough memory on the system but probably not enough contiguous memory for processing large file, user may use _RecyclableMemoryStream_ instead of _MemoryStream_ to avoid the System.OutOfMemoryException.
*   Added _CellsHelper.CustomImplementationFactory_ property, it gets/sets the _CustomImplementationFactory_ instance used by Aspose.Cells component.
*    Added _Workbook.AddDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)_ method, it adds digital signature to an already signed OOXML spreadsheet file (Excel2007 and later).
*    Added _ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint_ property, it indicates whether to output a blank page when there is nothing to print.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][12].
*   [Aspose.Cells for .NET Download Section][13].
*   [Aspose.Cells for .NET Documentation][14] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][15] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][16] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][17] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/net/new-releases/aspose.cells-for-.net-17.8/
[2]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+17.8+Release+Notes
[3]: https://www.nuget.org/packages/Aspose.Cells/
[4]: https://docs.aspose.com/display/cellsnet/Add+Digital+Signature+to+an+already+signed+Excel+file
[5]: https://docs.aspose.com/display/cellsnet/Output+Blank+Page+when+there+is+Nothing+to+Print
[6]: https://docs.aspose.com/display/cellsnet/Using+CustomImplementationFactory+to+create+custom+implementation+of+Memory+Stream
[7]: https://docs.aspose.com/display/cellsnet/Create+Remove+and+Get+GridCell+Comments
[8]: https://docs.aspose.com/display/cellsnet/Default+Font+and+Font+Color+of+the+GridDesktop
[9]: https://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Different+Formats
[10]: https://docs.aspose.com/display/cellsnet/Chart+Rendering
[11]: https://docs.aspose.com/display/cellsnet/Convert+Excel+Workbook+to+PDF
[12]: https://products.aspose.com/cells/net
[13]: https://downloads.aspose.com/cells/net
[14]: https://docs.aspose.com/display/cellsnet/home
[15]: https://apireference.aspose.com/
[16]: https://forum.aspose.com/c/cells
[17]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




