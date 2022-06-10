---
title: 'Export Custom Properties in Excel to PDF and Create Safe Sheet Names in Java'
date: Thu, 27 Sep 2018 15:59:24 +0000
draft: false
url: /2018/09/27/export-custom-properties-to-pdf-and-create-safe-sheet-names-using-aspose.cells-for-java-v18.9/
author: Ahsaniqbal
summary: ''
tags: ['Create Safe Sheet Names in Java', 'Export Custom Properties in Excel in Java', 'Java Excel Library']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="">}}


We are back with pleasure to present another enhanced version [Aspose.Cells for Java v18.9][1] containing a lot of new features, enhancements, and bug fixes as usual. These new features will strengthen our developer's community to enhance their solutions and provide more advanced level products to their customers. We always prefer resolving the bugs which are reported by our precious developers to avoid missing any milestone in their development lifecycles and make the customers happy by providing bug-free products. Enhancements are another direction that we always follow to enrich our existing features and increase usability.

The detailed [release notes][2] are provided which cover all the new features, enhancements and list of bugs that are resolved in this new version. Exceptions handling empowers the developers to keep control of the applications and assist users in a better way to continue using the application without any interruptions. We have resolved many exceptions to achieve this goal. For easy access and utilization, Aspose for Java APIs can be directly installed from Maven repository for which check this [document][3].

## Export Custom Document Properties in Excel to PDF

Many documents can have custom properties that were not made part of the PDFs earlier. Now we have provided this feature to maintain the precious information through custom properties by exporting them to the PDF files. These properties can be observed in Adobe Acrobat Reader by clicking on File and then Custom tab page in the properties sheet.   

For a working example refer to the following article:

*   [Export custom document properties to PDF][4]

## Create Safe Sheet Names in Excel using C#

Sometimes there is a need for assigning the sheet name at runtime. In this scenario, there may be sheet names that may contain some additional characters like <>+(?”. There is a need to replace any such character, which is not allowed as a sheet name with some preset character provided by the user. Similarly, the length may increase to more than 31 characters which need to be truncated. Apache POI provides certain features of creating safe names, hence similar feature is provided by Aspose.Cells to handle all these issues.

For a working example along with a template file refer to the following article:

*   [Create safe sheet names similar to Apache POI][5]

## Get XML Path from List Object/Table

XML data can be imported to worksheets where sometimes the XML path is required from the ListObjects of the worksheet. This feature is available in Excel by using an expression like Sheet1.ListObjects(1).XmlMap.DataBinding. We are glad to share that this feature is available now in Aspose.Cells as well. 

For a working example refer to the following article:

*   [Get XML path from ListObject/Table][6]  

## Enhanced filters like Contains, Not Contains, Blank and Non-Blank 

We have increased the range of auto filters like filtering based on fill color, date, dynamic date, number, and texts. These filters were already part of our previous releases. The need was felt to add filters like blank/non-blank and custom filters with contains and not-contains. This time these filters are added along with sample files so that these features can be tested easily. 

For a working example refer to the following article:

*   [Filtering with Blanks/Non-Blanks and custom contains/Not-Contains][7] 

## Retrieve Query Table Result Range 

QueryTable represents a worksheet table built from data returned from an external data source, such as an SQL server or a Microsoft access database.  Aspose.Cells provides an option to read the address i.e. result range of cells for a query table.  

For a working example refer to the following article:

*   [Retrieve range of query table][8] 

## Other Enhancements and Fixes

There are some other enhancements included and a few exceptions handled in the new release for the users. A few of the worth mentioning features and other improvements are as follows.

*   Chart in PDF is not generating from the Excel template 
*   Duplicate legend item text in the chart in Excel to PDF conversion 
*   Waterfall chart not rendered properly after changing the chart data 
*   Wrong value retrieved for border style 
*   Wrong bottom border style returned for merged cell 
*   Gray borders appear after reading cell style in the worksheet 
*   PasteType.VALUES\_AND\_NUMBER\_FORMATS is not working fine 
*   Exception: "FormulaBuildUnknown formula token0" on Name.getRefersTo() 
*   Chart.calculate method causes OutOfMemoryError 

In Aspose.Cells 18.9, we fixed several important bugs and other issues. For example, issues of not showing chart table in converted PDF, Issues in Cells.deleteRow() not displaying charts while converting ODS to PDF and error by MS Excel while loading file after setting autofilters. 

## Changes to the Public API

The following is a list of any changes made to the public API such as added, renamed, removed or deprecated members as well as any non-backward compatible change made to Aspose.Cells for Java:

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
*   Adds **PdfSaveOptions.CustomPropertiesExport property**, Gets or sets a value determining the way CustomDocumentPropertyCollection are exported to PDF file. The default value is None
*   Adds **class XmlDataBinding**, Represents XML Data Binding information
*   Adds **ListObject.XmlMap property**, Gets an XmlMap used for this list
*   Adds **XmlDataBinding.Url property**, Gets source URL of this data binding
*   Adds **XmlMap.DataBinding property**, Gets an XmlDataBinding of this map

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][9].
*   [Download Aspose.Cells for Java][10].
*   [Aspose.Cells for Java Documentation][11] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][12] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][13] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for Java Examples][14] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://artifact.aspose.com/repo/com/aspose/aspose-cells/18.9/
[2]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+18.9+Release+Notes
[3]: https://docs.aspose.com/display/cellsjava/Installation#Installation-InstallingAspose.CellsforJavafromMavenRepository
[4]: https://docs.aspose.com/display/cellsjava/Saving+Excel+files+to+CSV%2C+PDF+and+other+formats#SavingExcelfilestoCSV,PDFandotherformats-ExportCustompropertiestoPDF
[5]: https://docs.aspose.com/display/cellsjava/Names+and+Indices#NamesandIndices-Createsafesheetnames
[6]: https://docs.aspose.com/display/cellsjava/Query+Cell+Areas+Mapped+to+Xml+Map+Path+using+Worksheet.XmlMapQuery+method#QueryCellAreasMappedtoXmlMapPathusingWorksheet.XmlMapQuerymethod-GetXMLpathfromListObject/Table
[7]: https://docs.aspose.com/display/cellsjava/Data+Filtering#DataFiltering-Blanks
[8]: https://docs.aspose.com/display/cellsjava/Reading+and+Writing+Query+Table+of+Worksheet
[9]: https://products.aspose.com/cells/java
[10]: https://artifact.aspose.com/repo/com/aspose/aspose-cells/
[11]: https://docs.aspose.com/display/cellsjava/home
[12]: https://apireference.aspose.com/java/cells
[13]: https://forum.aspose.com/c/cells
[14]: https://github.com/aspose-cells/Aspose.Cells-for-Java




