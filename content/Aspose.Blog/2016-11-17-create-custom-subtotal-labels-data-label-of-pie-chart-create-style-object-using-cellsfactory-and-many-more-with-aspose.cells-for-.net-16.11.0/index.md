---
title: 'Create Custom Subtotal Labels &amp; Data Label of Pie Chart, Create Style object using CellsFactory and many more with Aspose.Cells for .NET 16.11.0'
date: Thu, 17 Nov 2016 13:00:40 +0000
draft: false
url: /2016/11/17/create-custom-subtotal-labels-data-label-of-pie-chart-create-style-object-using-cellsfactory-and-many-more-with-aspose.cells-for-.net-16.11.0/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce our next version of [Aspose.Cells for .NET v16.11.0][1]. The new release includes some features and other important enhancements with some critical bug fixes. Please see the [release notes][2] in order to know what is new and what has been changed/fixed with this version of Aspose.Cells for .NET. If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you to check the complete [Public API Changes][3] section to know what APIs are changed so far. We have highlighted some valuable features and other enhancements here.

## Create Custom Subtotal Labels

Aspose.Cells for .NET 16.11.0 has added the support for the creation of custom subtotal labels allowing the application developers to customize the labels according to the region or personal preferences. In order to provide this feature, the latest version of the Aspose.Cells for .NET has exposed the GlobalizationSettings class offering the following 2 methods which can be overridden in a custom class to get desired labels for the Subtotals.

*   GlobalizationSettings.GetTotalName: Gets the total name of the function.
*   GlobalizationSettings.GetGrandTotalName: Gets the grand total name of the function.

The GlobalizationSettings class can be used to customize the Subtotal labels by overriding the GlobalizationSettings.GetTotalName & GlobalizationSettings.GetGrandTotalName methods as demonstrated below.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-CustomLabelsSubtotals-GlobalizationSettings.cs" >}}

In order to inject custom labels, it is required to assign the WorkbookSettings.GlobalizationSettings property to an instance of the CustomSettings class defined above, before adding the Subtotals to the worksheet.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-CustomLabelsSubtotals-UsingGlobalizationSettings.cs" >}}

## Render Other Custom Label for Pie Chart

The GlobalizationSettings class also offers the GetOtherName method which is useful to give the "Other" label of Pie charts a custom value. The following snippet defines a custom class and overrides the GetOtherName method to get a custom label based on the system's regional (culture) settings.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-CustomTextForLabels-GlobalizationSettings.cs" >}}

The following snippet loads an existing spreadsheet containing a Pie chart and renders the chart to the image while utilizing the CustomSettings class created above.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-CustomTextForLabels-UsingGlobalizationSettings.cs" >}}

Please check the detailed article on [Introduction to GlobalizationSettings Class][4] if you want to get more in-depth knowledge of the aforementioned usage scenarios.

## Create Style Object with CellsFactory Class

Aspose.Cells 16.11.0 has exposed the CellsFactory class which currently has one method, that is; CreateStyle. The CellsFactory.CreateStyle method can be used to create an instance of Style class without adding it to the pool of workbook styles.

Here is a simple usage scenario of newly exposed APIs to create a simple Style object, whereas a detailed article can be viewed on [Creating Style Object with CellsFactory Class][5].

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-UsingCellsFactory-1.cs" >}}

## Access Hyperlink from a GridWeb

Aspose.Cells.GridWeb for .NET 16.11.0 has exposed GetHyperlink method to the GridHyperlinkCollection class that allows getting the instance of GridHyperlink by either passing an instance GridCell or a pair of integers corresponding to the row-column indices.

Here is a simple usage scenario of GridHyperlinkCollection.GetHyperlink method, whereas a detailed article can be viewed on [Access GridHyperlink from a GridCell Object][6].



## Other Enhancements and Fixes

Aspose.Cells for .NET 16.11.0 has fixed a few critical bugs as well as enhanced its core for more stability. A few of the worth mentioning enhancements are as follow.

*   Support for [MINIFS & MAXIFS functions][7].
*   Ability to [manipulate Workbook's Absolute Path][8].
*   Ability to [implement Subtotal or Grand Total labels in other languages][9].
*   Aspose.Cells for .NET formula calculation engine is enhanced.
*   Handled and fixed a few exceptions, such as, Stack overflow, NullPointerException, IndexOutOfRangeException, System.ArgumentOutOfRangeException and System.ArgumentException, etc. for certain scenarios/cases.

Furthermore, in this release, we have fixed several other issues. For example, issues around reading/writing MS Excel Excel file formats, manipulating and rendering shapes, manipulating PivotTables, copying ranges in the worksheet, rendering to HTML file format, [rendering images from Excel worksheets][10], [rendering images files from charts][11] and [exporting Excel workbooks to PDF format][12] have been resolved.

## Changes to the Public API

This revision of Aspose.Cells for .NET has made some changes to the Public API. A few of the worth mentioning changes are as follow whereas details can be viewed from the [Migration Manual][13].

*   Constructor for the Style class has been marked obsoleted whereas an alternative approach has been exposed that uses the CellsFactory class.
*   The Cell.GetConditionalStyle method has been completely removed from the public APIs because it was obsoleted some time back and an alternative approach has already been exposed by using Cell.GetConditionalFormattingResult method.
*   The Cells.GetMaxDataRowInColumn(int column) method has been removed. It is advised to use the Cells.GetLastDataRow(int) method as an alternative.
*   The PageSetup.Draft property has been removed. It is advised to use the PageSetup.PrintDraft property instead.
*   The AutoFilter.FilterColumnCollection property has been removed while providing the AutoFilter.FilterColumns property to achieve the same goal.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][14].
*   [Aspose.Cells for .NET Download Section][15].
*   [Aspose.Cells for .NET Documentation][16] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][17] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][18] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][19] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/net
[2]: http://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+16.11.0+Release+Notes
[3]: http://docs.aspose.com/display/cellsnet/Migrating+from+Earlier+Versions+of+Aspose.Cells
[4]: http://docs.aspose.com/display/cellsnet/Using+GlobalizationSettings+Class+for+Custom+Subtotal+Labels+and+Other+Label+of+Pie+Chart
[5]: http://docs.aspose.com/display/cellsnet/Create+Style+object+using+CellsFactory+class
[6]: http://docs.aspose.com/display/cellsnet/Access+Hyperlink+object+of+the+GridWeb+Cell
[7]: http://docs.aspose.com/display/cellsnet/Calculation+of+Excel+2016+MINIFS+and+MAXIFS+functions
[8]: http://docs.aspose.com/display/cellsnet/Change+the+Absolute+Path+of+External+Link+Data+Source+File
[9]: http://docs.aspose.com/display/cellsnet/Implement+Subtotal+or+Grand+Total+labels+in+other+languages
[10]: http://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Image
[11]: https://docs.aspose.com/display/cellsnet/Convert+an+Excel+Chart+to+Image
[12]: http://docs.aspose.com/display/cellsnet/Converting+Excel+to+PDF+Files
[13]: http://docs.aspose.com/display/cellsnet/Public+API+Changes+in+Aspose.Cells+16.11.0
[14]: https://products.aspose.com/cells/net
[15]: https://downloads.aspose.com/cells/net
[16]: http://docs.aspose.com/display/cellsnet/home
[17]: https://apireference.aspose.com/net/cells
[18]: http://forum.aspose.com
[19]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




