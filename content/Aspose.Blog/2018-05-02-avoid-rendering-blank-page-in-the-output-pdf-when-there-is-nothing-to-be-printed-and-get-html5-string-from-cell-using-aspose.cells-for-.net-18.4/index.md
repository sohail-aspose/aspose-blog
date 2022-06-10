---
title: 'Avoid Rendering Blank Page in Output PDF when Excel File is Empty - Aspose.Cells for .NET 18.4'
date: Wed, 02 May 2018 12:24:34 +0000
draft: false
url: /2018/05/02/avoid-rendering-blank-page-in-the-output-pdf-when-there-is-nothing-to-be-printed-and-get-html5-string-from-cell-using-aspose.cells-for-.net-18.4/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce the release of [Aspose.Cells for .NET v18.4][1]. Please check the [document][2] on how to install Aspose for .NET APIs directly from the NuGet repository. In this release, we have added some worthy features and other enhancements for the users. Please check the [release notes][3] in order to get an idea about what is new and what has been enhanced or fixed with this revision of Aspose.Cells for .NET.

## Avoid Blank Page in Output PDF when Worksheet is Empty

When the Excel file is empty and the user saves it to PDF using Aspose.Cells, it renders the blank page in output PDF. Sometimes, this default behavior is undesirable. Aspose.Cells provides the **PdfSaveOptions.OutputBlankPageWhenNothingToPrint** property to deal with this issue. If you will set it as false, then CellsException will occur whenever there is nothing to print in the output PDF.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Rendering-AvoidBlankPageInOutputPdfWhenThereIsNothingToPrint.cs" >}}

Please see the following article for more detail on this topic for your reference.

*   [Avoid Blank Page in Output PDF when there is Nothing to Print][4]

## Find Type of X and Y Values of Points in Chart Series

Sometimes, you want to know the type of X and Y values of chart points in a series. Aspose.Cells provides **ChartPoint.XValueType** and **ChartPoint.YValueType** properties that can be used for this purpose. Please note, you will have to call **Chart.Calculate()** method before you could use these properties effectively. Please see the following article for more detail on this topic for your reference:  

*   [Find Type of X and Y Values of Points in Chart Series][5]

## Get HTML5 String from Cell

Aspose.Cells returns the HTML string of the cell using the string **GetHtmlString (bool html5)** method. If you pass "false" as parameter, it will return you Normal HTML but if you pass "true" as parameter, it will return Html5 string. Please see the following article for more detail on this topic for your reference:

*   [Get HTML5 string from Cell][6]

## Hiding Overlaid Content with CrossHideRight while Saving to HTML

When you save your MS Excel file to HTML, you can specify different cross types for cell strings. By default, Aspose.Cells generates HTML as per Microsoft Excel but when you change cross-type to **CrossHideRight** then it hides all the strings from the right side of the cell which are overlaid or overlapping with cell string. Please see the following article for more detail on this topic for your reference:

*   Hiding Overlaid Content with CrossHideRight while saving to Html

## Specify the Language of the Excel File using Built-In Document Properties

You can change the Language of MS Excel file by right-clicking the file and then selecting Properties > Details and then editing the Language field. Please use **BuiltInDocumentPropertyCollection.Language** property to change it programmatically using Aspose.Cells APIs. Please see the following article for more detail on this topic for your reference:

*   [Specify the Language of the Excel File using BuiltIn Document Properties][7]

## Create Chart PDF with Desired Page Size

You can create a chart's PDF file with your desired page size using Aspose.Cells and specify how you want to align the chart inside the page like top, bottom, center, left, right, etc. Besides this, the output chart can be created in stream or on disk. Please see the following article for more detail on this topic for your reference:

*   [Create Chart PDF with Desired Page Size][8]

## Get All Hidden Rows Indices after Refreshing AutoFilter

When you apply the auto filter on worksheet cells, then some of the rows get hidden automatically. But it might be the case that some of the rows are already hidden manually by MS Excel end user and they are not hidden by auto filter feature. It, therefore, makes difficult to know which of the rows are hidden by an auto filter and which rows are hidden manually by MS Excel end user. Aspose.Cells deals with this problem using the **int\[\] AutoFilter.Refresh(bool hideRows)** method. This method returns the row indices of all the rows that are hidden by an auto filter and not by the manual way in MS Excel. Please see the following article for more detail on this topic for your reference:

*   [Get All Hidden Rows Indices after Refreshing AutoFilter][9]

## Rotate Text with Shape inside the Worksheet

You can add text inside any shape using Microsoft Excel. If you add shape using the older Microsoft Excel 2003, then the text will not rotate with shape. But if you add shape using newer versions of Microsoft Excel e.g. 2007, 2010, 2013 or 2016, etc. then the text will be rotated with shape. You can control if the text should rotate with the shape or not using the **ShapeTextAlignment.RotateTextWithShape** property. Please see the following article for more detail on this topic for your reference:

*   [Rotate Text with Shape inside the Worksheet][10]

## Read/Write TSV (Tab-Separated Values) Files 

Tab-Separated Values (TSV) file (similar to Tab Delimited) contains spreadsheet data but without formattings. Aspose.Cells does support to read and write TSV file format type, it includes relevant member (TSV) in both LoadFormat and SaveFormat Enumerations. See the following sample code for your reference.

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-Files-Handling-OpeningTSVFiles-1.cs" >}}

Please see the following article for more detail on this topic for your reference.

*   [Opening Tab-Separated Values (TSV) Files][11]Files)

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][12].
*   [Install Aspose for .NET APIs from NuGet repository][13]
*   [Aspose.Cells for .NET Documentation][14] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][15] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][16] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][17] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Cells/18.4.0
[2]: https://docs.aspose.com/display/cellsnet/Installation#Installation-InstallAspose.Cellsfor.NETthroughNuGet
[3]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+18.4+Release+Notes
[4]: https://docs.aspose.com/display/cellsnet/Avoid+Blank+Page+in+Output+Pdf+when+there+is+Nothing+to+Print
[5]: https://docs.aspose.com/display/cellsnet/Find+Type+of+X+and+Y+Values+of+Points+in+Chart+Series
[6]: https://docs.aspose.com/display/cellsnet/Get+HTML5+string+from+Cell
[7]: https://docs.aspose.com/display/cellsnet/Specify+the+Language+of+the+Excel+File+using+BuiltIn+Document+Properties
[8]: https://docs.aspose.com/display/cellsnet/Create+Chart+PDF+with+Desired+Page+Size
[9]: https://docs.aspose.com/display/cellsnet/Get+All+Hidden+Rows+Indices+after+Refreshing+AutoFilter
[10]: https://docs.aspose.com/display/cellsnet/Rotate+Text+with+Shape+inside+the+Worksheet
[11]: https://docs.aspose.com/display/cellsnet/Opening+Files+with+Different+Formats#OpeningFileswithDifferentFormats-OpeningTab-SeparatedValues(TSV
[12]: https://products.aspose.com/cells/net
[13]: https://www.nuget.org/packages/Aspose.Cells
[14]: https://docs.aspose.com/display/cellsnet/home
[15]: https://apireference.aspose.com/
[16]: https://forum.aspose.com/c/cells
[17]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




