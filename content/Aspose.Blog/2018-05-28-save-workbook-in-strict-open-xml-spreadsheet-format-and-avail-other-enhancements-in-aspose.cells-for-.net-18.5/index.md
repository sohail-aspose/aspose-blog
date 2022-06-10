---
title: 'Save Excel Workbook as Strict Open XML Format in C# using Aspose.Cells for .NET'
date: Mon, 28 May 2018 15:23:02 +0000
draft: false
url: /2018/05/28/save-workbook-in-strict-open-xml-spreadsheet-format-and-avail-other-enhancements-in-aspose.cells-for-.net-18.5/
author: Amjad Sahi
summary: ''
tags: ['Excel to Strict Open XML', 'Save Excel workbooks as Strict Open XML']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce the release of [Aspose.Cells for .NET v18.5][1]. Please check the [document][2] on how to install Aspose for .NET APIs directly from the NuGet repository. In this release, we have added a few valuable features. We also included some important fixes and other enhancements for the users. Please check the [release notes][3] in order to get an idea about what is new and what has been enhanced or fixed with this revision of Aspose.Cells for .NET.

## Save Excel Workbook to Strict Open XML Spreadsheet

Aspose.Cells now allows you to save the workbook in Strict Open XML Spreadsheet format. This feature was demanded by certain users. This can be accomplished by **Workbook.Settings.Compliance** property. If you set its value as _OoxmlCompliance.Iso29500\_2008\_Strict_, then the output Excel file will be saved in Strict Open XML Spreadsheet format.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "LoadingSavingConvertingAndManaging-SaveWorkbookToStrictOpenXMLSpreadsheetFormat.cs" >}}

Please see the following article for more detail on this topic for your reference.

*   [Save Workbook to Strict Open XML Spreadsheet Format][4]

## Specify Individual or Private Set of Fonts for Workbook Rendering

Generally, you specify the fonts directory or list of fonts for all the workbooks but sometimes, you have to specify individual or private set of fonts for your desired workbooks. Aspose.Cells provides **IndividualFontConfigs** class that can be used to specify the individual or private set of fonts for your workbook. Please see the following article for more detail on this topic for your reference:

*   [Specify Individual or Private Set of Fonts for Workbook Rendering][5]

## Specify the Far East and Latin Name of the Font in Text Options of Shape

Sometimes you want to display text in Far East language font e.g. Japanese, Chinese, Thai, etc. Aspose.Cells provides **TextOptions.FarEastName** property that can be used to specify the font name of the Far East language. Besides, you can also specify the Latin font name using **TextOptions.LatinName** property. Please see the following article for more detail on this topic for your reference:

*   [Specify the Far East and Latin Name of the Font in Text Options of Shape][6]

## Other Enhancements and Fixes

There are some other enhancements included and a few exceptions handled in the new release for the users. A few of the worth mentioning features and other improvements are as follows.

*   Aspose.Cells formula calculation engine is enhanced and we have added more advanced formulas/functions to the [supported list][7].
*   Handled an exception "Invalid formula..." when refreshing pivot chart data.
*   Handled NullReferenceExceptions on opening MS Excel files on Mono Ubuntu Linux.
*   Handled an exception when using ListObject.ConvertToRange method.

In Aspose.Cells 18.5, we fixed several important bugs and other issues. For example, issues around reading/writing MS Excel file formats, manipulating PageSetup options, Smart Markers, manipulating ListObject/Tables, rendering and manipulating charts and shapes, manipulating PivotTables, [rendering images from Excel worksheets][8], [rendering images files from charts][9] and [exporting Excel workbooks to PDF format][10] have been resolved in the release.

## Changes to the Public API

This version of Aspose.Cells for .NET has made some changes to the Public API. A few of the worth mentioning changes are as follow:

*   Added **Cell.IsTableFormula/IsArrayFormula** (new properties) to replace older **Cell.IsInTable/IsInArray**, it indicates whether one cell is part of the table formula or array formula.
*   Added **IndividualFontConfigs** class, it represents Font configs for each workbook object.
*   Added **OoxmlCompliance** enum and **WorkbookSettings.Compliance** property, it supports Strict Open XML Spreadsheet.
*   Added **GroupShape.Ungroup()** method, it ungroups shapes.
*   Added **MsoFormatPicture.Gamma** property, it gets and sets the gamma of the picture.
*   Added **TextOptions.FarEastName** and **TextOptions.LatinName** properties, these attributes get and set the Far East and Latin name of the font.
*   Deleted obsoleted **FontSetting.ShapeFont** property.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][11].
*   [Install Aspose for .NET APIs from NuGet repository][12]
*   [Aspose.Cells for .NET Documentation][13] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][14] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][15] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][16] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Cells/18.5.1
[2]: https://docs.aspose.com/display/cellsnet/Installation#Installation-InstallAspose.Cellsfor.NETthroughNuGet
[3]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+18.5+Release+Notes
[4]: https://docs.aspose.com/display/cellsnet/Save+Workbook+to+Strict+Open+XML+Spreadsheet+Format
[5]: https://docs.aspose.com/display/cellsnet/Specify+Individual+or+Private+Set+of+Fonts+for+Workbook+Rendering
[6]: https://docs.aspose.com/display/cellsnet/Specify+the+Far+East+and+Latin+Name+of+the+Font+in+Text+Options+of+Shape
[7]: https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions
[8]: https://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Different+Formats
[9]: https://docs.aspose.com/display/cellsnet/Chart+Rendering
[10]: https://docs.aspose.com/display/cellsnet/Convert+Excel+Workbook+to+PDF
[11]: https://products.aspose.com/cells/net
[12]: https://www.nuget.org/packages/Aspose.Cells
[13]: https://docs.aspose.com/display/cellsnet/home
[14]: https://apireference.aspose.com/
[15]: https://forum.aspose.com/c/cells
[16]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




