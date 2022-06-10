---
title: 'Node.js - Apply Text Alignment to Partial Text inside TextBox in Excel Worksheets'
date: Wed, 05 Sep 2018 18:52:10 +0000
draft: false
url: /2018/09/05/apply-text-alignment-to-partial-text-inside-textbox-and-disable-pivot-table-ribbon-using-aspose.cells-for-javascript-via-java-18.8/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

We are pleased to announce the release of [Aspose.Cells for JavaScript via Java 18.8][1]. This release includes a number of features, enhancements, and bug fixes which further improve the overall stability and usability of the API. Since Aspose.Cells for JavaScript is a subset component, so it includes all the important and useful features present in its native Aspose.Cells for Java, please visit features comparison page for your reference. Aspose.Cells for JavaScript via Java has almost full functionality of Aspose.Cells for Java with a [few limitations, minor API changes and additional requirements][2]. See the following release notes on major features and other improvements for your reference

## Apply Text Alignment to Partial Text Inside the TextBox

It is very common to apply different alignments to the partial texts in the text box. This feature was having some issues but now it is reviewed and bugs are removed to incorporate proper alignment.   

For a working example refer to the following article:

*   [Applying text alignment to partial text inside the Textbox][3]  

## Content Copying for accessibility

This option allows screen reader software to utilize the text within the PDF file for reading.  You can disable it by applying a change permissions password and deselecting a few options in Adobe Acrobat. The same functionality can be achieved using Aspose.Cells for JavaScript via Java now. 

For a working example refer to the following article:

*   [Set content copy for accessibility option][4] 

## Disable Pivot Table Ribbon 

Pivot table based reports are useful but prone to error if target users do not have detailed knowledge of Excel to configure these reports. In these circumstances, organizations will want to restrict users from being able to change a pivot table based report. Common pivot table features like adding additional filters, slicers, fields, or changing the order of certain things in the report are mostly not recommended for every user. On the other hand, these users shall also be able to refresh the report and use existing filters or slicers. Aspose.Cells has provided this ability to developers for restricting users from changing these reports while creating them. For this purpose, Excel provides the feature to disable pivot table ribbon and same is provided by Aspose.Cells i.e. developer can disable the ribbon which contains controls to modify these reports.

For a working example along with a template file refer to the following article:

*   [Disable Pivot Table Ribbon][5]

## Improvements in Process Interruption 

Reliability and efficiency is a basic requirement by the users for any software product. If some conversion takes too long, sometimes it is required to interrupt this process to return control to the user. This feature is already present but got some performance issues, however, we have further improved it and now can be used without any trouble.  

For a working example refer to the following article:

*   [Aspose.Cells for Java - Interruptible Library][6] 

## Pasting Rows/Columns with Paste Option 

While working with Excel, pasting rows and columns is very common and this feature was introduced in the earliest versions of Aspose.Cells. However limited paste option was available in contrast to Excel where a variety of options are available when we paste data somewhere in Excel. Now Aspose.Cells has provided this feature and you can paste data with multiple options.   

For a working example refer to the following article:

*   [Pasting rows and columns with paste options][7] 

## Other Enhancements and Fixes

There are some other enhancements included and a few exceptions handled in the new release for the users. In Aspose.Cells for JavaScript via Java v18.8, we fixed several important bugs and other issues. For example, issues of not drawing the vertical line at the center of the chart, reading watermark from a file, unnecessary text in property comment, retaining the macros in ODS files, and rendering exception while converting worksheet to the image. 

## Changes to the Public API

The following is a list of any changes made to the public API such as added, renamed, removed or deprecated members as well as any non-backward compatible change made to Aspose.Cells for Java:

*   Adds **PdfSecurityOptions.AccessibilityExtractContent,** Permission to copy or extract content (in support of accessibility to disabled users or for other purposes)
*   Adds **SubtotalSetting class, **Represents the setting of subtotal.
*   Adds **Cells.RetrieveSubtotalSetting(CellArea)** method, Retrieves the setting of subtotal
*   Adds overload **Range.ExportDataTable (Aspose.Cells.ExportTableOptions)** method, Supports options of exporting range
*   Adds **WebQueryConnection.IsSameSetting** property and deletes **WebQueryConnection.IsFirstRow** property, Use WebQueryConnection.IsSameSetting property instead
*   Adds **WebQueryConnection.IsXmlSourceData** property and deletes **WebQueryConnection.IsSourceData** property, Use WebQueryConnection.IsXmlSourceData property instead
*   Adds **Shape.IsEquation** property, Indicates whether the shape contains equation
*   Adds overload **Cells.CopyColumns(Int32,Int32,PasteOptions)** and **Cells.CopyRows(Int32,Int32,PasteOptions)** method, Supports paste options when copying rows and columns
*   Adds **Axis.IsAutoTickLabelSpacing** property, Indicates whether tick label spacing is automatic

## Aspose.Cells for JavaScript via Java Resources

The following are the links to some useful resources you may need to accomplish your tasks.

*   Aspose.Cells for JavaScript via Java Online Documentation (Aspose.Cells for JavaScript via Java is ported from Aspose.Cells for Java. So, you can use the same documentation)
*   Features
*   Release Notes
*   [Product Page][8]
*   [Download Aspose.Cells for JavaScript via Java][9]
*   [API Reference Guide][10] 
*   [Free Support Forum][11]
*   [Paid Support Helpdesk][12]




[1]: https://downloads.aspose.com/cells/nodejs
[2]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Node.js+via+Java+Limitations+and+API+Differences
[3]: https://docs.aspose.com/display/cellsjava/Applying+text+alignment+to+partial+text+inside+the+TextBox
[4]: https://docs.aspose.com/display/cellsjava/Saving+Excel+files+to+CSV%2C+PDF+and+other+formats#SavingExcelfilestoCSV,PDFandotherformats-SetContentCopyForAccessibilityoption
[5]: https://docs.aspose.com/display/cellsjava/Disable+Pivot+Table+Ribbons
[6]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+-+Interruptible+Library
[7]: https://docs.aspose.com/display/cellsjava/Copying+Rows+and+Columns#CopyingRowsandColumns-PastingRows/ColumnswithPasteOptions
[8]: https://www.aspose.com/products/cells/javascript
[9]: https://downloads.aspose.com/cells/javascript
[10]: https://apireference.aspose.com/javascript/cells
[11]: https://forum.aspose.com/c/cells
[12]: https://helpdesk.aspose.com/




