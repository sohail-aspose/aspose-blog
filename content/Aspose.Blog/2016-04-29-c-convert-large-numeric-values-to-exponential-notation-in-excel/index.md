---
title: 'Convert Large Numeric Values to Exponential Notation in Excel using C#'
date: Fri, 29 Apr 2016 11:31:57 +0000
draft: false
url: /2016/04/29/c-convert-large-numeric-values-to-exponential-notation-in-excel/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce our next version of Aspose.Cells for .NET v8.8.0. This release contains some valuable features along with critical bug fixes and other enhancements. Please see the [release notes][1] in order to get an idea of what is new and what has been fixed with this version of Aspose.Cells for .NET. If you are planning to upgrade the Aspose.Cells for .NET API to the latest revision, we would strongly suggest you to check the complete [Public API Changes][2] section to know what APIs are changed so far. We have highlighted some important features and other enhancements here.

## Control the Conversion of Large Numeric Value to Exponential Notation

As per default behavior, if a numeric value is larger than the threshold, the API converts such values to exponential notation while importing HTML segment/files to Aspose.Cells object model. In the past, we could use HTMLLoadOptions.ConvertNumericData property to control the conversion of textual values to numeric data, however, this approach has its own drawbacks. For instance, if there are more than one column containing the numeric values, setting the HTMLLoadOptions.ConvertNumericData property to false will direct the Aspose.Cells APIs to keep all values in textual format. In such a case, all formatting from the numeric values will be lost.

In order to handle the situations where users wish to retain the format of all numeric values as well as keep the data in its original state, the Aspose.Cells for .NET 8.8.0 has exposed the HTMLLoadOptions.KeepPrecision property. The Boolean property allows controlling the conversion of large numeric values to exponential notation. When set to true, the numeric values larger than 15 digits will be imported as it is.

Here is the simple usage scenario demonstrating the usage of HTMLLoadOptions.KeepPrecision property to avoid the conversion of large numbers to exponential notation while importing data from Html.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-AvoidExponentialNotationWhileImportingFromHtml-1.cs" >}}

## Delete Redundant Spaces in Excel to HTML

Aspose.Cells for .NET 8.8.0 has exposed the HTMLLoadOptions.DeleteRedundantSpaces property to control the preservation of redundant spaces after the line break tag (<BR> tag) in HTML. If the aforementioned property is set to true the API will delete all the redundant spaces while importing the HTML in Aspose.Cells object mode. The HTMLLoadOptions.DeleteRedundantSpaces property has the default value is false, which means, all the redundant spaces are preserved in the resultant spreadsheet.

## Detect if Cell Value Starts with Single Quote

Aspose.Cells for .NET 8.8.0 has exposed the Style.QuotePrefix property to detect if the cell value starts with a single quote mark. With previous versions of Aspose.Cells APIs, it was not possible to distinguish between the text values, such as sample and 'sample.

Here is the simple usage scenario of Style.QuotePrefix property to [find if the cell value starts with a single quote mark][3].

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Articles-FindIfCellValueStartsWithSingleQuote-FindIfCellValueStartsWithSingleQuote.cs" >}}

## Other Enhancements and Fixes

The most notable other enhancements in this release are as follows:

*   Ability to [use image markers while grouping data in smart markers][4].
*   Ability to [find Query Tables and List Objects related to external data connections][5].
*   The improved PDF rendering engine for chart objects.

We have also handled a few exceptions regarding reading/writing MS Excel files, rendering Excel files to PDF and refreshing Pivot Tables.

In this release, several important issues have been addressed. For example, issues around manipulating Microsoft Excel file formats, importing and converting HTML files, manipulating and rendering shapes, [rendering images from Excel worksheets][6], manipulating charts, [rendering images files from charts][7] and [exporting Excel workbooks to PDF format][8] have been resolved. The Aspose.Cells formula calculation engine is also enhanced in this release.

Moreover, in the new release, we have added session timeout alert in the web-based grid control provided by Aspose.Cells for .NET. We also fixed a few issues regarding data validations and GridWeb's context menu.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 8.8.0, please visit the [download page][9].




[1]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+8.8.0+Release+Notes
[2]: https://docs.aspose.com/display/cellsnet/Migrating+from+Earlier+Versions+of+Aspose.Cells
[3]: https://docs.aspose.com/display/cellsnet/Find+if+the+cell+value+starts+with+single+quote+mark
[4]: https://docs.aspose.com/display/cellsnet/Using+Image+Markers+while+Grouping+Data+in+Smart+Markers
[5]: https://docs.aspose.com/display/cellsnet/Find+Query+Tables+and+List+Objects+related+to+External+Data+Connections
[6]: https://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Different+Image+Formats
[7]: https://docs.aspose.com/display/cellsnet/Convert+an+Excel+Chart+to+Image
[8]: https://docs.aspose.com/display/cellsnet/Convert+Excel+Workbook+to+PDF
[9]: http://downloads.aspose.com/cells/net




