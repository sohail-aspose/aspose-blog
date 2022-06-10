---
title: 'Disable Pivot Table Ribbon in Excel using Java'
date: Tue, 04 Sep 2018 11:23:34 +0000
draft: false
url: /2018/09/04/paste-text-with-paste-options-and-disable-pivot-table-ribbon-using-aspose.cells-for-java-18.8/
author: Ahsaniqbal
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Cells for Java v18.8][1] having new features, enhancements, and bug fixes to supplement the usability of the product and support the developer's community. New features are always part of our every release to enrich the product.   
Special effort is made to address all the known issues and fulfill enhancement requests for a rapid development of feature-rich market-oriented products. Detailed release notes are published as usual for detailed information about the enhancements, bugs fixing and handling of a variety of exceptions in this new release. For easy access and utilization, Aspose for Java APIs can be directly installed from the Maven repository ([read more][2].

## Disable Pivot Table Ribbon in Excel using Java

Pivot table based reports are useful but prone to error if target users do not have detailed knowledge of Excel to configure these reports. In these circumstances, organizations will want to restrict users from being able to change a pivot table based report. Common pivot table features like adding additional filters, slicers, fields, or changing the order of certain things in the report are mostly not recommended for every user. On the other hand, these users shall also be able to refresh the report and use existing filters or slicers. Aspose.Cells has provided this ability to developers for restricting users from changing these reports while creating them. For this purpose, Excel provides a feature to disable the pivot table ribbon, and the same is provided by Aspose.Cells i.e. developer can disable the ribbon which contains controls to modify these reports.

For a working example along with a template file refer to the following article:

*   [Disable Pivot Table Ribbon][3]

## Applying Text Alignment to Partial Text Inside the TextBox

It is very common to apply different alignments to the partial texts in the text box. This feature was having some issues but now it is reviewed and bugs are removed to incorporate proper alignment.   

For a working example refer to the following article:

*   [Applying text alignment to partial text inside the Textbox][4]  

## Content Copying for Accessibility

This option allows screen reader software to utilize the text within the PDF file for reading.  You can disable it by applying a change permissions password and deselecting a few options in Adobe Acrobat. The same functionality can be achieved using Aspose.Cells for Java now. 

For a working example refer to the following article:

*   [Set content copy for accessibility option][5] 

## Improvements in process interruption 

Reliability and efficiency are the basic requirements by the users for any software product. If some conversion takes too long, sometimes it is required to interrupt this process to return control to the user. This feature is already present but got some performance issues, however, we have further improved it and now can be used without any trouble.  

For a working example refer to the following article:

*   [Aspose.Cells for Java - Interruptible Library][6] 

## Pasting Rows/Columns with Paste Option 

While working with Excel, pasting rows and columns is very common and this feature was introduced in the earliest versions of Aspose.Cells. However limited paste option was available in contrast to Excel where a variety of options are available when we paste data somewhere in Excel. Now Aspose.Cells has provided this feature and you can paste data with multiple options.

For a working example refer to the following article:

*   [Pasting rows and columns with paste options][7] 

## Other Enhancements and Fixes

There are some other enhancements included and a few exceptions handled in the new release for the users. A few of the worth mentioning features and other improvements are as follows.

*   Hyperlinks not working when referenced from other sheets
*   Incorrect alignment issue while rendering to PDF
*   Wrong placement of table data from HTML to Excel file
*   Depiction of slicer control while spreadsheet to HTML conversion
*   Improper gradient color rendering to PDF
*   Improper chart category title display in PDF
*   Wrong border style for merged cells

In Aspose.Cells 18.8, we fixed several important bugs and other issues. For example, issues of not drawing the vertical line at the center of the chart, reading watermark from the file, unnecessary text in property comment, retaining the macros in ODS files, and rendering exception while converting worksheet to the image. 

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

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][8].
*   [Download Aspose.Cells for Java][9].
*   [Aspose.Cells for Java Documentation][10] – up-to-date documentation containing Programmer’s Guide, Knowledge Base, and much more.
*   [Aspose.Cells for Java API Reference Guide][11] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][12] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for Java Examples][13] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://artifact.aspose.com/repo/com/aspose/aspose-cells/18.8/
[2]: https://docs.aspose.com/display/cellsjava/Installation#Installation-InstallingAspose.CellsforJavafromMavenRepository)
[3]: https://docs.aspose.com/display/cellsjava/Disable+Pivot+Table+Ribbons
[4]: https://docs.aspose.com/display/cellsjava/Applying+text+alignment+to+partial+text+inside+the+TextBox
[5]: https://docs.aspose.com/display/cellsjava/Saving+Excel+files+to+CSV%2C+PDF+and+other+formats#SavingExcelfilestoCSV,PDFandotherformats-SetContentCopyForAccessibilityoption
[6]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+-+Interruptible+Library
[7]: https://docs.aspose.com/display/cellsjava/Copying+Rows+and+Columns#CopyingRowsandColumns-PastingRows/ColumnswithPasteOptions
[8]: https://products.aspose.com/cells/java
[9]: https://artifact.aspose.com/repo/com/aspose/aspose-cells/
[10]: https://docs.aspose.com/display/cellsjava/home
[11]: https://apireference.aspose.com/java/cells
[12]: https://forum.aspose.com/c/cells
[13]: https://github.com/aspose-cells/Aspose.Cells-for-Java




