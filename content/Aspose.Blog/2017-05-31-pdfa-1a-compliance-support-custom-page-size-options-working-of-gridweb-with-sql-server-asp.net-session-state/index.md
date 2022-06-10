---
title: 'PDF/A-1a Compliance, and Working of GridWeb with SQL Server ASP.NET Session State'
date: Wed, 31 May 2017 15:22:28 +0000
draft: false
url: /2017/05/31/pdfa-1a-compliance-support-custom-page-size-options-working-of-gridweb-with-sql-server-asp.net-session-state/
author: Mshakeel Faiz
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce the release of [Aspose.Cells for .NET v17.5][1]. This release includes many new features and enhancements along with some critical bug fixes that further improve the overall stability of the API. Please check the [release notes][2] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for .NET. You can also install [Aspose for .NET APIs directly from NuGet repository][3].

## Support PDF/A-1a Compliance in PdfSaveOptions

Aspose.Cells now allows you to create PDF with PDF/A-1a – Level A (accessible) conformance. It already supports PDF/A-1b – Level B (basic) conformance. Following code snippet demonstrates how to convert an Excel file to PDF compatible with PDFA-1a.

```
//Open an Excel file.
Workbook wb = new Workbook("e:\\test2\\Book1.xlsx");

//Create pdf save options and set its compliance to PDFA-1a.
PdfSaveOptions opts = new PdfSaveOptions();
opts.Compliance = PdfCompliance.PdfA1a;

//Save the output pdf.
wb.Save("e:\\test2\\out1.pdf", opts);
```

Please see this article that explains how to convert your Excel file into PDF with PDF/A-1a conformance.

*   [Convert Excel file to PDF format compatible with PDFA-1a][4]

## Remove Existing Printer Settings in Excel Workbook

Sometimes developers want to remove existing Printer Settings in Excel file. These settings are found inside the “\[file "root"\]\\xl\\printerSettings” folder in the form of .bin files. Aspose.Cells can remove existing printer settings in the Excel workbook. For more detail, please see this article.

*   [Remove Existing PrinterSettings of Worksheets in Excel file][5]

## Implement Custom Page Size Options for the Worksheet

There is no direct option available to create custom paper sizes in MS Excel, however, you can set custom paper size of your desired worksheets when rendering Excel file to PDF file format. This document explains how to set custom paper size of a worksheet using Aspose.Cells APIs.

*   [Implement Custom Paper Size of Worksheet for Rendering][6]

## Export HTML String Value of the Cells to the DataTable

Using Aspose.Cells APIs, developers can fill a DataTable with corresponding HTML strings (based on cells values) while exporting worksheet data. This document explains how to export HTML strings for the formatted cells data to fill a DataTable using Aspose.Cells APIs.

*   [Export HTML String Value of the Cells to the DataTable][7]

## Working of GridWeb when ASP.NET Session State Mode is SQL Server

If you want to use SQL Server or StateServer to hold sessions, use GridWeb Session Mode. The GridWeb control now supports serializing its data to SQL Server or StateServer. For detail, please see this article.

*   [Working of GridWeb when ASP.NET Session state mode is SQL Server][8]

## Shift First Row Down when Inserting Cells Data Table Rows

Earlier, Aspose.Cells does not shift first row down when inserting rows. But for some users' requirements, it has supported this feature now. Please see this article for more detail about this feature. It also shows an example of ICellsDataTable implementation.

*   [Export HTML String Value of the Cells to the DataTable][9]

## Copy Page Setup Settings from Source Worksheet into Destination Worksheet

When you copy the worksheet into another worksheet, then page setup settings of the source worksheet are not copied to the destination worksheet. Please use PageSetup.Copy() method to copy the setting of the page setup from source to destination worksheet. Please see the following article for more detail.

*   [Copy Page Setup Settings from Source Worksheet into Destination Worksheet][10]

## Changes to the Public API

This version of Aspose.Cells for .NET has made some changes to the Public API. A few of the worth mentioning changes are as follow.

*   Added _ExportTableOptions.ExportAsHtmlString_ property that exports the HTML string value of the cells to the DataTable.
*   Added _PageSetup.Copy(PageSetup source,CopyOptions copyOptions)_ method that copies the settings of the Page Setup.
*   Added _PageSetup.CustomPaperSize()_ method that sets the custom paper size, in the unit of inches.
*   Added _PageSetup.PrinterSettings_ property that gets and sets the settings of the default printer.
*   Added enum member _PdfCompliance.PdfA1a_ that represents PDF format compatible with PDFA-1a.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][11].
*   [Aspose.Cells for .NET Download Section][12].
*   [Aspose.Cells for .NET Documentation][13] – up-to-date documentation containing Programmer's Guide, Knowledge Base, and much more.
*   [Aspose.Cells for .NET API Reference Guide][14] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][15] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][16] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/net/new-releases/aspose.cells-for-.net-17.5/
[2]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+17.5+Release+Notes
[3]: https://www.nuget.org/packages/Aspose.Cells/
[4]: https://docs.aspose.com/display/cellsnet/Convert+Excel+file+to+PDF+format+compatible+with+PDFA-1a
[5]: https://docs.aspose.com/display/cellsnet/Remove+Existing+PrinterSettings+of+Worksheets+in+Excel+file
[6]: https://docs.aspose.com/display/cellsnet/Implement+Custom+Paper+Size+of+Worksheet+for+Rendering
[7]: https://docs.aspose.com/display/cellsnet/Export+HTML+String+Value+of+the+Cells+to+the+DataTable
[8]: https://docs.aspose.com/display/cellsnet/Working+of+GridWeb+when+ASP.NET+Session+state+mode+is+SQL+Server
[9]: https://docs.aspose.com/display/cellsnet/Shift+First+Row+down+when+inserting+Cells+Data+Table+Rows
[10]: https://docs.aspose.com/display/cellsnet/Copy+Page+Setup+Settings+from+Source+Worksheet+into+Destination+Worksheet
[11]: https://www.aspose.com/products/cells/net
[12]: https://downloads.aspose.com/cells/net
[13]: https://docs.aspose.com/display/cellsnet/home
[14]: https://apireference.aspose.com/
[15]: https://forum.aspose.com/c/cells
[16]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




