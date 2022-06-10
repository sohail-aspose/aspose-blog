---
title: 'Update References while Deleting Blank Rows &amp; Columns and other Enhancements with Aspose.Cells for .NET 8.8.2'
date: Wed, 08 Jun 2016 09:56:51 +0000
draft: false
url: /2016/06/08/update-references-while-deleting-blank-rows-columns-and-other-enhancements-with-aspose.cells-for-.net-8.8.2/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for .NET logo][1]](http://www.aspose.com/.net/excel-component.aspx "Aspose.Cells for .NET API")We are pleased to announce our next version of [Aspose.Cells for .NET v8.8.2][2]. This release includes some valuable enhancements and other bug fixes. It also improves the overall stability and usability of the APIs. Please see the release notes in order to get an idea on what is new and what has been changed/fixed with this version of Aspose.Cells for .NET. If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you to check the complete Public API Changes section to know what APIs are changed so far. We have highlighted some important features and other enhancements here.

## Deleting Blank Rows & Columns with Updated References

As per default behaviour, Aspose.Cells APIs delete the blank rows & columns without updating the cell references that may have been effected from the delete process. This could lead to undesired results in certain cases, especially when spreadsheet contains formulas or charts.

Aspose.Cells APIs have tried to overcome the aforementioned situation by exposing the overloaded versions of the Cells.DeleteBlankRows & Cells.DeleteBlankColumns methods with the release of Aspose.Cells for .NET 8.8.2. The new methods can accept an instance of DeleteOptions class and can be used to overcome the situations that could arise due to the broken references in formulas, chart series data and so on. The DeleteOptions class currently has one member, a Boolean type property by the name UpdateReference. If the said property is set to true and the instance of DeleteOptions class is passed to the Cells.DeleteBlankRows & Cells.DeleteBlankColumns methods, the API will internally adjust the formula references (if any) to accommodate the changes.

Below provided code snippet demonstrates the simple usage scenario of newly exposed overloads. If you wish to get more understanding where these methods should be used, please check the detailed article on updating cell references while deleting blank rows & columns.

```
//Create an instance of Workbook & load an existing spreadsheet
var book = new Workbook(dir + "sample.xlsx");

//Access worksheet from which blank rows/columns have to be deleted
var sheet = book.Worksheets[0];

//Access cells of the desired worksheet
var cells = sheet.Cells;

//Create an instance of DeleteOptions class
DeleteOptions options = new DeleteOptions();
//Set UpdateReference property to true;
options.UpdateReference = true;

//Delete all blank rows and columns
cells.DeleteBlankColumns(options);
cells.DeleteBlankRows(options);
```

## Other Enhancements and Fixes

The most notable enhancements in this release are as follow:

*   Ability to render Unicode Supplementary Characters in PDF.

We have also handled a few exceptions regarding sorting Pivot Tables data.

In this release, several important issues have been addressed. For example, issues around reading and writing Microsoft Excel file formats, manipulating PivotTables, manipulating List Objects/Tables, converting spreadsheets to HTML files and vice versa, manipulating and rendering charts and shapes, rendering images from Excel worksheets, rendering images files from charts and exporting Excel workbooks to PDF format have been resolved.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][3].
*   [Aspose.Cells for .NET Download Section][4].
*   Aspose.Cells for .NET Documentation – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][5] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][6] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][7] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png "Aspose.Cells for .NET logo"
[2]: http://www.aspose.com/downloads/cells/net/new-releases/aspose.cells-for-.net-8.8.2/
[3]: http://www.aspose.com/.net/excel-component.aspx
[4]: http://www.aspose.com/downloads/cells/net
[5]: http://www.aspose.com/api/net/cells
[6]: https://forum.aspose.com/
[7]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




