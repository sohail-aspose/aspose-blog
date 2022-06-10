---
title: 'PDF/A-1a Compliance, Custom Page Size Options and Copy Page Setup Settings in Java'
date: Thu, 01 Jun 2017 10:30:40 +0000
draft: false
url: /2017/06/01/pdfa-1a-compliance-custom-page-size-options-and-copy-page-setup-settings-supported-in-java/
author: Amjad Sahi
summary: ''
tags: ['Convert Excel to PDFA-1a in Java', 'Custom Page Size in Excel to PDF', 'Java Excel Library']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


Aspose team is pleased to announce the release of [Aspose.Cells for Java 17.5][1]. This release includes many new features and enhancements along with some critical bug fixes that further improve the overall stability of the API. We also recommend our clients [use the powerful Aspose for Java APIs directly in their Maven Projects with simple configurations][2]. Please check the [release notes][3] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Java. Here is a look at the major features in this release.

## Support PDF/A-1a compliance in PdfSaveOptions

Aspose.Cells now allows you to create PDF with PDF/A-1a – Level A (accessible) conformance. It already supports PDF/A-1b – Level B (basic) conformance. Following code snippet demonstrates how to convert an Excel file to PDF compatible with PDFA-1a.

```
//Open an Excel file.
Workbook wb = new Workbook("Book1.xlsx");
 
//Create pdf save options and set its compliance to PDFA-1a.
PdfSaveOptions opts = new PdfSaveOptions();
opts.setCompliance(PdfCompliance.PDF_A_1_A);
 
//Save the output pdf
wb.save("outputCompliancePdfA1a.pdf", opts);
```

Please see this article that explains how to convert your Excel file into PDF with PDF/A-1a conformance.

*   [Convert Excel file to PDF format compatible with PDFA-1a][4]

## Remove existing Printer Settings in Excel file

Sometimes developers want to remove existing Printer Settings in Excel file. These settings are found inside the “\[file "root"\]\\xl\\printerSettings” folder in the form of .bin files. Aspose.Cells can remove existing printer settings in the Excel workbook. For more detail, please see this article.

*   [Remove Existing PrinterSettings of Worksheets in Excel file][5]

## Implement Custom Page Size Options for the Worksheet

There is no direct option available to create custom paper sizes in MS Excel, however, you can set custom paper size of your desired worksheets when rendering Excel file to the PDF file format. This document explains how to set a custom paper size of a worksheet using Aspose.Cells APIs.

*   [Implement Custom Paper Size of Worksheet for Rendering][6]

## Shift First Row down when inserting Cells Data Table Rows

Earlier, Aspose.Cells does not shift first row down when inserting rows. But for some users' requirements, it has supported this feature now. Please see this article for more detail about this feature. It also shows an example of ICellsDataTable implementation.

*   [Export HTML String Value of the Cells to the DataTable][7]

## Copy Page Setup Settings from Source Worksheet into Destination Worksheet

When you copy the worksheet into another worksheet, then page setup settings of the source worksheet are not copied to the destination worksheet. Please use PageSetup.copy() method to copy the setting of the page setup from source to destination worksheet. Please see the following article for more detail.

*   [Copy Page Setup Settings from Source Worksheet into Destination Worksheet][8]

## Changes to the Public API

This version of Aspose.Cells for Java has made some changes to the Public API. A few of the worth mentioning changes are as follow.

*   Added _PageSetup.copy(PageSetup source,CopyOptions copyOptions)_ method that copies the settings of the Page Setup.
*   Added _PageSetup.customPaperSize()_ method that sets the custom paper size, in the unit of inches.
*   Added _PageSetup.getPrinterSettings()/setPrinterSettings()_ property that gets and sets the settings of the default printer.
*   Added enum member _PdfCompliance.PDF\_A\_1\_A_ that represents PDF format compatible with PDFA-1a.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][9].
*   [Aspose.Cells for Java Download Section][10].
*   [Aspose.Cells for Java Documentation][11] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][12] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][13] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][14] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Java Examples][15] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/java/new-releases/aspose.cells-for-java-17.5/
[2]: https://blog.aspose.com/2014/08/12/aspose-for-maven-aspose-cloud-maven-repository/
[3]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+17.5+Release+Notes
[4]: https://docs.aspose.com/display/cellsjava/Convert+Excel+file+to+PDF+format+compatible+with+PDFA-1a
[5]: https://docs.aspose.com/display/cellsjava/Remove+Existing+PrinterSettings+of+Worksheets+in+Excel+file
[6]: https://docs.aspose.com/display/cellsjava/Implement+Custom+Paper+Size+of+Worksheet+for+Rendering
[7]: https://docs.aspose.com/display/cellsjava/Shift+First+Row+down+when+inserting+Cells+Data+Table+Rows
[8]: https://docs.aspose.com/display/cellsjava/Copy+Page+Setup+Settings+from+Source+Worksheet+into+Destination+Worksheet
[9]: https://products.aspose.com/cells/java
[10]: https://downloads.aspose.com/cells/java
[11]: https://docs.aspose.com/display/cellsjava/home
[12]: https://apireference.aspose.com/java/cells
[13]: https://forum.aspose.com/c/cells
[14]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/
[15]: https://github.com/asposecells/Aspose_Cells_Java




