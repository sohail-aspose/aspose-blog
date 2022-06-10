---
title: 'Optimize Excel to PDF File Size and Add Digital Signatures for VBA Projects using C#'
date: Tue, 02 Feb 2016 09:52:00 +0000
draft: false
url: /2016/02/02/optimize-excel-to-pdf-file-size-and-add-digital-signatures-to-excel-vba-project-in-csharp/
author: Amjad Sahi
summary: ''
tags: ['Add Digital Signatures to Excel VBA Project', 'Optimize Excel to PDF File Size']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


Aspose.Cells for .NET 8.7.0 has been released. This release contains some useful features and other enhancements along with critical bug fixes. If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you to check the complete Public API Changes section to know what has been changed in the API so far. We have highlighted some important features (of this month's release) here.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Optimize Excel to PDF File Size using C#

Aspose.Cells APIs have provided an enhancement for the PDF rendering engine in order to reduce the resultant PDF file size. Aspose.Cells for.NET 8.7.0 has exposed the PdfSaveOptions.OptimizationType property along with an enumeration by the name PdfOptimizationType in order to facilitate the application developers to control the resultant PDF file size to a certain extent.

The PdfOptimizationType enumeration has 2 constants at the moment exhibiting the following behavior.

1.  PdfOptimizationType.MinimumSize: API tries to optimize the cell text and cell border records in order to reduce the resultant PDF file size.
2.  PdfOptimizationType.Standard: No optimization is done therefore the resultant file size will be large as compared to PdfOptimizationType.MinimumSize selection.

The following piece of code demonstrates the usage of PdfSaveOptions.OptimizationType property to [minimize the resultant PDF file size][1] while exporting spreadsheets to PDF format.

{{< gist aspose-cells c326c6c668fc372e30569fa9e0f6bf4b "Examples-CSharp-Articles-RenderingAndPrinting-SaveExcelIntoPdfWithOptimizedSize-SaveExcelIntoPdfWithOptimizedSize.cs" >}}

## Re-size Chart's Data Label Shape to Fit Text

Aspose.Cells for .NET 8.7.0 has exposed the Boolean type DataLabels.IsResizeShapeToFitText property in order to mimic Excel's feature of re-sizing data label shapes to fit the text.

Please note, Excel application provides the **Resize shape to fit text** option for chart's data labels to increase the size of the shape so that the text fits inside of it. This option can be accessed on an Excel interface by selecting any of the data labels on the chart. Right-click and select **Format DataLabels** menu. On **Size & Properties** tab, expand **Alignment** node to reveal the related properties including the **Resize shape to fix text** option as highlighted below.



{{< figure align=center src="images/Excel-Resize-Shape-To-Fit-Text.png" alt="">}}


The following piece of code shows the simple usage scenario of DataLabels.IsResizeShapeToFitText property to [re-size the chart's data label shapes to fit text][2].

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-ManageChartsAndShapes-ResizeChartDataLabelToFit-1.cs" >}}

Here is a snapshot showing a simple bar chart before & after executing the above code.



{{< figure align=center src="images/chart-resize-datalabel-shape-to-fit-text.png" alt="">}}


## Enhancements to Protection Module

Aspose.Cells APIs have enhanced the Protection class by introducing some useful properties & methods. Two of the most worth mentioning enhancements are as follow.

### Detect if Worksheet is Password Protected

It is possible to protect the workbooks and worksheets separately. For instance, a spreadsheet may contain one or more worksheets that are password-protected, however, the spreadsheet itself may or may not be protected. Aspose.Cells API for Java has provided the Protection.IsProtectedWithPassword field to [detect if a worksheet is password protected][3]. Boolean type Protection.IsProtectedWithPassword field returns true if Worksheet is password protected and false if not.

### Verify Password Used to Protect the Worksheet

Aspose.Cells for .NET 8.7.0 has exposed the Protection.VerifyPassword method which allows to specify a password as an instance of String and [verifies if same password has been used to protect the worksheet][4]. The Protection.VerifyPassword method returns true if the specified password matches with the password used to protect the given Worksheet, false if specified password does not match.

The following piece of code uses the Protection.VerifyPassword method in conjunction with Protection.IsProtectedWithPassword field to detect the password protection and verifies the password.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-ManagingWorkbooksWorksheets-VerifyPasswordUsedToProtectWorksheets-VerifyPasswordUsedToProtectWorksheets.cs" >}}

## Load or Import Delimited File Containing Formulas

Aspose.Cells for .NET has provided support to identify & parse the formulas while loading CSV/TXT files having delimited plain data. Newly exposed TxtLoadOptions.HasFormula property when set to true directs the API to parse the formulas from the input delimited file and set them to relevant cells without requiring any additional processing.

The following piece of code demonstrates the usage of TxtLoadOptions.HasFormula property to [load and import the CSV with formulas in it][5].

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-ManagingWorkbooksWorksheets-ImportCSVWithFormulas-ImportCSVWithFormulas.cs" >}}

## Create 2-Color Scale Conditional Format

This release of the API has exposed the ColorScale.Is3ColorScale property that can be used to create a 2-Color Scale conditional format. The said property is of type boolean with the default value of true which means that the conditional format will be of 3-Color Scale by default. However, switching the ColorScale.Is3ColorScale property to false will generate a 2-Color Scale conditional format.

Please see the detailed article on [Adding 2 & 3-Color Scale Conditional Formatting][6].

## Other Enhancements & Fixes

The most notable enhancements in this release are as follow:

*   Newly exposed field VbaProject.IsSigned allows to [detect if a given VbaProject is digitally signed or not][7].
*   Newly exposed attribute VbaProject.CertRawData allows to [export VBA Digital Certificate to streams][8].
*   Newly exposed attribute VbaProject.IsValidSigned allows to [determine if the signature is valid][9].
*   Newly exposed method VbaProject.Sign() allows to [digitally sign VBA code project][10].
*   This release has added support for [importing XML map inside an instance of Workbook][11].

We have handled a few exceptions regarding reading/writing Excel files and rendering PivotTables and HTML file format.

In this release, several important issues have been addressed. For example, issues around manipulating Microsoft Excel file formats, manipulating Pivot Tables, applying styles, conditional formatting, [rendering images from Excel worksheets][12], manipulating charts, [rendering images files from charts][13] and [exporting Excel workbooks to PDF format][14] have been resolved. We have further enhanced the Aspose.Cells formula calculation engine and fixed a few issues in this regard.

Moreover, in the new release, we have also fixed a few issues in the web-based grid control provided by Aspose.Cells for .NET.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 8.7.0, please visit the [download page][15].




[1]: https://docs.aspose.com/display/cellsnet/Save+Excel+into+PDF+with+Standard+or+Minimum+Size
[2]: https://docs.aspose.com/display/cellsnet/Resize+Chart's+Data+Label+Shape+To+Fit+Text
[3]: https://docs.aspose.com/display/cellsnet/Detect+if+Worksheet+is+Password+Protected
[4]: https://docs.aspose.com/display/cellsnet/Verify+Password+Used+to+Protect+the+Worksheet
[5]: https://docs.aspose.com/display/cellsnet/Load+or+Import+CSV+file+with+Formulas
[6]: https://docs.aspose.com/display/cellsnet/Adding+2-Color+Scale+and+3-Color+Scale+Conditional+Formattings
[7]: http://docs.aspose.com/display/cellsnet/Check+if+VBA+Code+is+Signed
[8]: http://docs.aspose.com/display/cellsnet/Export+VBA+Certifcate+to+File+or+Stream
[9]: http://docs.aspose.com/display/cellsnet/Check+if+Digital+Signature+of+VBA+Code+is+Valid
[10]: http://docs.aspose.com/display/cellsnet/Digitally+Sign+a+VBA+Code+Project+with+Certificate
[11]: http://docs.aspose.com/display/cellsnet/Import+XML+Map+inside+a+Workbook+using+Aspose.Cells
[12]: http://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Image
[13]: https://docs.aspose.com/display/cellsnet/Convert+an+Excel+Chart+to+Image
[14]: http://docs.aspose.com/display/cellsnet/Converting+Excel+to+PDF+Files
[15]: https://downloads.aspose.com/cells/net




