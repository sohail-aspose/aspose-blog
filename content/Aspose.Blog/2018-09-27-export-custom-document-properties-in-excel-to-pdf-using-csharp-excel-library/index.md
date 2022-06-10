---
title: 'Export Custom Document Properties in Excel to PDF using C#'
date: Thu, 27 Sep 2018 15:38:48 +0000
draft: false
url: /2018/09/27/export-custom-document-properties-in-excel-to-pdf-using-csharp-excel-library/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce the release of [Aspose.Cells for .NET v18.9][1], the MS Excel file formats API that provides the ability to create, manipulate, convert or render MS Excel spreadsheets, and more importantly - is fully documented. Please check the [document][2] on how to install Aspose for .NET APIs directly from the NuGet repository. We have added a few important features while keeping the product more stable and feature-rich API. In this release, we have also added some useful enhancements and resolved a number of issues. Please check the [release notes][3] which cover all the new features, enhancements, and list of bugs that are resolved in this new version. Exceptions handling empowers the developers to keep control of the applications and assist users in a better way to continue using the application without any interruption. We have resolved many exceptions to achieve this goal. You will get an idea about what is new and what has been enhanced or fixed with this revision of Aspose.Cells for .NET.

## Export Custom Document Properties in Excel to PDF

Many documents can have custom properties that were not made a part of the output PDFs earlier. Now we have provided this feature to maintain the precious information through custom properties by exporting these to the PDF files. These properties can be observed in Adobe Acrobat Reader by clicking on File and then Custom tab page in the properties sheet.   

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Files-Utility-ExportCustomPropertiesToPdf-1.cs" >}}

For a working example refer to the following article:

*   [Export custom document properties to PDF][4]

## Get XML Path from List Object/Table

XML data can be imported to worksheets where sometimes the XML path is required from the ListObjects of the worksheet. This feature is available in MS Excel by using an expression like **Sheet1.ListObjects(1).XmlMap.DataBinding**. We are glad to share that this feature is available now in Aspose.Cells as well. 

For a working example refer to the following article:

*   [Get XML path from ListObject/Table][5] 

## Create Safe Sheet Names 

Sometimes there is a need for assigning the sheet name at runtime. In this scenario, there may be sheet names that may contain some additional characters like <>+(?”. You might need to replace any such character, which is not allowed as a sheet name with some preset character. Similarly, the length may increase to more than 31 characters which need to be truncated. Apache POI provides certain features of creating safe names, hence similar feature is provided by Aspose.Cells to handle all these issues.

For a working example along with a template file refer to the following article:

*   [Create safe sheet names similar to Apache POI][6]

## Enhanced filters like Contains, Not Contains, Blank and Non-Blank 

We have increased the range of auto filters like filtering based on fill color, date, dynamic date, number, and texts. These filters were already part of our previous releases. The need was felt to add filters like blank/non-blank and custom filters with contains and not-contains. This time these filters are added along with sample files so that these features can be tested easily. 

For a working example refer to the following article:

*   [Filtering with Blanks/Non-Blanks and custom contains/Not-Contains][7] 

## Retrieve Query Table Result Range 

QueryTable represents a worksheet table built from data returned from an external data source, such as an SQL Server or a Microsoft Access database. Aspose.Cells provides an option to read the address i.e. result range of cells for a query table.  

For a working example refer to the following article:

*   [Retrieve range of query table][8] 

## Other Enhancements and Fixes

There are some other enhancements included and a few exceptions handled in the new release for the users. A few of the worth mentioning features and other improvements are as follows.

*   Support stock chart in ODS file
*   Included unsigned Dlls of Aspose.Cells
*   Add Row.FirstDataCell property to retrieve the first data cell in the row
*   Handled exception when converting an XLSX file to PDF file format 
*   Handled ArgumentOutOfRangeException while calling Slicer.Refresh()
*   Handled exception when retrieving the URL of the list object's XML data binding map
*   Handled System.OverflowException while calling Chart.Calculate
*   Handled exception while saving the document

In Aspose.Cells 18.9, we fixed several important bugs and other issues. For example, issues around reading/writing MS Excel file formats, applying conditional formatting, setting borders in ODS file, reading/writing HTML files, manipulating List Object/Table, adding OLE packages, rendering and manipulating charts and shapes, manipulating PivotTables, [rendering images from Excel worksheets][9], [rendering images files from charts][10] and [exporting Excel workbooks to PDF format][11] have been resolved in the release. 

## Changes to the Public API

The following is a list of any changes made to the public API such as added, renamed, removed or deprecated members as well as any non-backward compatible change made to Aspose.Cells for .NET:

*   Adds **CellsHelper.CreateSafeSheetName(string nameProposal)/CreateSafeSheetName(string nameProposal, char replaceChar) methods **,Methods for user's convenience to create valid sheet name
*   Adds **Row.FirstDataCell, **Gets the first non-blank cell in the row.
*   Adds **MapChartLabelLayout enum, **Represents the label layout type of the map chart
*   Adds **MapChartProjectionType enum**, Represents the projection type of the map chart
*   Adds **MapChartRegionType enum**, Represents the region type of the map chart
*   Adds **QuartileCalculationType enum**, Represents the quartile calculation type of the chart
*   Adds **Series.LayoutProperties property and class SeriesLayoutProperties**, Represents the layout properties of the series
*   Adds **TickLabels.IsAutomaticRotation property**, Indicates whether the rotation of the tick labels is automatic
*   Adds **FilterOperatorType.BeginsWith, Contains, EndsWith and NotContains enum**, Represents the text filter operator type
*   Adds **Cell.GetDisplayStyle(bool) method**, Gets the display style of the cell
*   Adds **GlobalizationSettings.GetStandardHeaderFooterFontStyleName(string localFontStyleName) method**, Gets standard English font style name (Regular, Bold, Italic) for Header/Footer according to given locale font style name
*   Adds **PdfCustomPropertiesExport enum**, Specifies the way CustomDocumentPropertyCollection are exported to PDF file
*   Adds **PdfSaveOptions.CustomPropertiesExport property**, Gets or sets a value determining the way CustomDocumentPropertyCollection are exported to PDF file. Default value is None
*   Adds **class XmlDataBinding**, Represents XML Data Binding information
*   Adds ListObject.XmlMap property, Gets an XmlMap used for this list
*   Adds XmlDataBinding.Url property, Gets source URL of this data binding
*   Adds **XmlMap.DataBinding property**, Gets an XmlDataBinding of this map

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][12].
*   [Install Aspose for .NET APIs from NuGet repository][13]
*   [Aspose.Cells for .NET Documentation][14] – up-to-date documentation containing Programmer's Guide, Knowledge Base, and much more.
*   [Aspose.Cells for .NET API Reference Guide][15] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][16] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][17] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Cells/18.9.0
[2]: https://docs.aspose.com/display/cellsnet/Installation#Installation-InstallAspose.Cellsfor.NETthroughNuGet
[3]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+18.9+Release+Notes
[4]: https://docs.aspose.com/display/cellsnet/Convert+Excel+Workbook+to+PDF#ConvertExcelWorkbooktoPDF-ExportCustompropertiestoPDF
[5]: https://docs.aspose.com/display/cellsnet/Query+Cell+Areas+Mapped+to+Xml+Map+Path+using+Worksheet.XmlMapQuery+method#QueryCellAreasMappedtoXmlMapPathusingWorksheet.XmlMapQuerymethod-GetXMLpathfromListObject/Table
[6]: https://docs.aspose.com/display/cellsnet/Names+and+Indices#NamesandIndices-Createsafesheetnames
[7]: https://docs.aspose.com/display/cellsnet/Data+Filtering#DataFiltering-Blanks
[8]: https://docs.aspose.com/display/cellsnet/Reading+and+Writing+Query+Table+of+Worksheet
[9]: https://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Different+Image+Formats
[10]: https://docs.aspose.com/display/cellsnet/Chart+Rendering
[11]: https://docs.aspose.com/display/cellsnet/Convert+Excel+Workbook+to+PDF
[12]: https://products.aspose.com/cells/net
[13]: https://www.nuget.org/packages/Aspose.Cells
[14]: https://docs.aspose.com/display/cellsnet/home
[15]: https://apireference.aspose.com/
[16]: https://forum.aspose.com/c/cells
[17]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




