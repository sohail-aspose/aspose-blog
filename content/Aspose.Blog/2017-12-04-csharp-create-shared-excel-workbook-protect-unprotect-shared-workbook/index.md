---
title: 'Create and Protect a Shared Excel Workbook in C#'
date: Mon, 04 Dec 2017 10:28:03 +0000
draft: false
url: /2017/12/04/csharp-create-shared-excel-workbook-protect-unprotect-shared-workbook/
author: Amjad Sahi
summary: ''
tags: ['Create a shared Excel Workbook', 'Protect or unprotect shared Excel workbooks']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce the release of [Aspose.Cells for .NET v17.11][1]. Please check the [release notes][2] in order to get an idea about what is new and what has been enhanced or fixed with this revision of Aspose.Cells for .NET. You can also install [Aspose for .NET APIs directly from NuGet repository][3].

## Create and Protect a Shared Excel Workbook in C#

Microsoft Excel allows you to create a shared workbook. When you share the workbook, then more than one user can edit the workbook. Aspose.Cells enables you to create a shared workbook with Workbook.Settings.Shared property. You can protect or unprotect a shared workbook.

### Create a Shared Excel Workbook

\[gist id="24a8eac23c3325e20dababecf735a43b" file="Examples-CSharp-Workbook-CreateSharedWorkbook.cs"\]

### Protect a Shared Excel Workbook

\[gist id="24a8eac23c3325e20dababecf735a43b" file="Examples-CSharp-Workbook-PasswordProtectOrUnprotectSharedWorkbook.cs"\]

For more detail on the features, please see these articles/documents for your reference.

*   [Create a Shared Workbook with Aspose.Cells][4]
*   [Password Protect or Unprotect the Shared Workbook][5]

## Determine Smart Art Shape and Convert it to Group Shape

Smart Art shapes are special shapes that allow you to create complex diagrams automatically. Aspose.Cells allows you to detect Smart Art shapes and convert them to Group shape. You can find if the shape is a smart art shape or normal shape using **Shape.IsSmartArt** property. You can also convert Smart Art Shape into Group Shape using the **Shape.GetResultOfSmartArt()** method. It will enable you to handle smart art shape like a group shape. Consequently, you will have access to the individual parts or shapes of the group shape. The following sample code loads a template file containing a smart art shape. It then converts the determine the smart art shape and convert into group shape.

\[gist id="24a8eac23c3325e20dababecf735a43b" file="Examples-CSharp-DrawingObjects-ConvertSmartArtToGroupShape.cs"\]

Please see the documents/articles with attachments and screenshots on how to determine Smart Art Shape and how to convert Smart Art Shape into Group Shape for your complete reference.

*   [Determine if a Shape is Smart Art Shape][6]
*   [Convert the Smart Art to Group Shape][7]

## Find the Root Element Name of XML Map

Aspose.Cells allows you to find the root element name of XML map using **XmlMap.RootElementName** property. For more detail, please see this article.

*   [Find the Root Element Name of Xml Map][8]

## Ignore Errors while Rendering Excel to PDF

You can ignore all errors during the conversion process using the **PdfSaveOptions.IgnoreError** property. This way, the conversion process will be completed smoothly without throwing any error or exception but data loss may occur. For more detail, please see this article.

*   [Ignore Errors while Rendering Excel to Pdf][9]

## Query Cell Areas Mapped to Xml Map Path

You can query cell areas mapped to the XML map path with Aspose.Cells using the **Worksheet.XmlMapQuery()** method. If the path exists, it will return the list of cell areas related to that path inside the XML map. For more detail, please see this article.

*   [Query Cell Areas Mapped to Xml Map Path using Worksheet.XmlMapQuery method][10]

## Render Sequence of Pages using PageIndex and PageCount Properties

Aspose.Cells allows you to render a sequence of pages of your Excel file to images using **ImageOrPrintOptions.PageIndex** and **ImageOrPrintOptions.PageCount** properties. These properties are useful when there are so many pages in your worksheet but you need to render a few pages only. This will not only save the processing time but also saves the memory consumption of the rendering process. For more detail, please see this article.

*   [Render Sequence of Pages using PageIndex and PageCount Properties of ImageOrPrintOptions][11]

## Other Enhancements and Fixes

There are some other enhancements included and other exceptions handled in the new release for the users. A few of the worth mentioning features and enhancements are as follows.

*   [Copy Paste Behavior Of EnableClipboardCopyPaste and PasteType GridDesktop Properties][12].
*   Handled exception when using PivotTable.RefreshData.
*   Handled System.ArgumentOutOfRangeException when XLSB is converted to PDF.
*   Handled exception while loading the output XLS file (with OLE Objects, images, etc. excluded).

In Aspose.Cells 17.11 we fixed some important bugs and other issues. For example, issues around reading/writing MS Excel file formats, data validation, rendering Excel to HTML and vice versa, applying formattings/style, rendering shapes and drawing objects, rendering and manipulating charts, manipulating PivotTables, auto-fitting rows/columns, [rendering images from Excel worksheets][13], [rendering images files from charts][14] and [exporting Excel workbooks to PDF format][15] have been resolved. The Aspose.Cells formula calculation engine is also improved.

## Changes to the Public API

This version of Aspose.Cells for .NET has made some changes to the Public API. A few of the worth mentioning changes are as follow:

*   Added **Shape.GetResultOfSmartArt()** method,  it converts smart art to a group shape.
*   Added **Shape.IsSmartArt** property, it indicates whether the shape is smart art.
*   Added **Workbook.ProtectSharedWorkbook()** and **Workbook.UnprotectSharedWorkbook()** method, these methods protect and unprotect the shared workbook.
*   Added **ImageOrPrintOptions.PageIndex** property, it gets or sets the 0-based index of the first page to save.
*   Added **ImageOrPrintOptions.PageCount** property, it gets or sets the number of pages to save.
*   Added **PdfSaveOptions.IgnoreError** property, it indicates if you need to hide the error while rendering.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][16].
*   [Aspose.Cells for .NET Download Section][17].
*   [Aspose.Cells for .NET Documentation][18] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][19] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][20] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][21] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.



[1]: https://downloads.aspose.com/cells/net/new-releases/aspose.cells-for-.net-17.11/
[2]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+17.11+Release+Notes
[3]: https://www.nuget.org/packages/Aspose.Cells/
[4]: https://docs.aspose.com/display/cellsnet/Create+Shared+Workbook+with+Aspose.Cells
[5]: https://docs.aspose.com/display/cellsnet/Password+Protect+or+Unprotect+the+Shared+Workbook
[6]: https://docs.aspose.com/display/cellsnet/Determine+if+Shape+is+Smart+Art+Shape
[7]: https://docs.aspose.com/display/cellsnet/Convert+the+Smart+Art+to+Group+Shape
[8]: https://docs.aspose.com/display/cellsnet/Find+the+Root+Element+Name+of+Xml+Map
[9]: https://docs.aspose.com/display/cellsnet/Ignore+Errors+while+Rendering+Excel+to+Pdf
[10]: https://docs.aspose.com/display/cellsnet/Query+Cell+Areas+Mapped+to+Xml+Map+Path+using+Worksheet.XmlMapQuery+method
[11]: https://docs.aspose.com/display/cellsnet/Render+Sequence+of+Pages+using+PageIndex+and+PageCount+Properties+of+ImageOrPrintOptions
[12]: https://docs.aspose.com/display/cellsnet/Copy+Paste+Behavior+Of+EnableClipboardCopyPaste+and+PasteType+GridDesktop+Properties
[13]: https://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Different+Formats
[14]: https://docs.aspose.com/display/cellsnet/Chart+Rendering
[15]: https://docs.aspose.com/display/cellsnet/Convert+Excel+Workbook+to+PDF
[16]: https://www.aspose.com/products/cells/net
[17]: https://downloads.aspose.com/cells/net
[18]: https://docs.aspose.com/display/cellsnet/home
[19]: https://apireference.aspose.com/
[20]: https://forum.aspose.com/c/cells
[21]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




