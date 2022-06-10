---
title: 'Set Default Font in Excel to PDF and Read Apple Numbers Spreadsheet in C# .NET'
date: Mon, 31 Jul 2017 19:55:43 +0000
draft: false
url: /2017/07/31/set-default-font-in-excel-to-pdf-and-read-apple-numbers-spreadsheet-in-csharp-asp.net/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce the release of [Aspose.Cells for .NET v17.7][1]. This release includes some useful features and other enhancements along with some critical bug fixes that further improve the overall stability of the APIs. Please check the [release notes][2] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for .NET. You can also install [Aspose for .NET APIs directly from NuGet repository][3].

## Set Default Font in Excel to PDF or Image

When saving to PDF or image, Aspose.Cells will first try to set Workbook's default font (i.e., Workbook.DefaultStyle.Font). If the workbook's default font still cannot show/render text properly, then Aspose.Cells will try to render with font mentioned against **DefaultFont** attribute in PdfSaveOptions/ImageOrPrintOptions. Aspose.Cells now provides a Boolean property named **CheckWorkbookDefaultFont** in PdfSaveOptions/ImageOrPrintOptions. You can set it to false to let the DefaultFont setting in PdfSaveOptions/ImageOrPrintOptions have priority.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-Fonts-SetDefaultFontPropertyOfPdfSaveOptionsAndImageOrPrintOptions.cs" >}}

Please see this article that explains how to set default font while rendering to PDF and image format.

*   [Set DefaultFont property of PdfSaveOptions and ImageOrPrintOptions to have priority][4]

## Read Numbers Spreadsheet Developed by Apple Inc.

Numbers is a spreadsheet application developed by Apple Inc. Aspose.Cells can read Numbers spreadsheet but it does not support writing to it. It can read Numbers spreadsheet's Data, Style and Formulas.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-LoadingSavingConvertingAndManaging-ReadNumbersSpreadsheet.cs" >}}

For more detail, please see this article.

*   [Read Numbers Spreadsheet Developed by Apple Inc. using Aspose.Cells APIs][5]

## Apply Advanced Filter of Microsoft Excel to Display Records Meeting Complex Criteria

Aspose.Cells allows you to apply the Advanced Filter using the **Worksheet.AdvancedFilter()** method. Just like Microsoft Excel, it accepts the following parameters:  
**_isFilter_** - Indicates whether filtering the list in place.  
**_listRange_** - The list range.  
**_criteriaRange_** - The criteria range.  
**_copyTo_** - The range where copying data to.  
**_uniqueRecordOnly_** - Only displaying or copying unique rows.  
See the following document/article for your reference.

*   [Apply Advanced Filter of Microsoft Excel to Display Records Meeting Complex Criteria][6]

## Implement Errors and Boolean Value in Russian or Any Other Language.

If you are using Microsoft Excel in Russian Locale/Language or any other Locale/Language, it will display errors and Boolean values according to that Locale or Language. You can achieve the similar behavior of Microsoft Excel using Aspose.Cells APIs with **Workbook.Settings.GlobalizationSettings** property. You will have to override the following methods of **GlobalizationSettings** class:  
**_GlobalizationSettings.GetErrorValueString()_**  
_**GlobalizationSettings.GetBooleanValueString()** _  
For more detail, please see this article.

*   [Implement Errors and Boolean Value in Russian or Any Other Language][7]

## Resize GridWeb in the Browser Window

Aspose.Cells.GridWeb provides client-side **_resize()_** function to resize the web-based grid control in the browser. Moreover, you can even make GridWeb control resizable in the browser window. For example, you may use the bottom right handle (via mouse) to customize its width/height in the window. You would need to include/specify jquery Javascript files to make it work in the page source in your project. For more detail, please see this article.

*   [Resize GridWeb in the browser window][8]

## Load and Render PivotTable into Aspose.Cells.GridDesktop

If your Excel file has a Pivot Table, Aspose.Cells.GridDesktop will be able to load and render the PivotTable fine by importing the file into it. Moreover, you will be able to interact the Pivot Table in GUI and manipulate it as you do it in MS Excel. The screenshot shows the rendering of Pivot Table in GridDesktop.



{{< figure align=center src="images/Render-PivotTable-In-GridDesktop-300x159.png" alt="">}}


For more detail, please see this article.

*   [Load and render PivotTable into Aspose.Cells.GridDesktop ][9]

## Other Enhancements and Fixes

There are numerous other important enhancements included in the new release for the users. A few of the worth mentioning features/enhancements are as follows.

*   [Determine if Paper Size of Worksheet is Automatic][10].
*   [Customize Row and Column Captions of Aspose.Cells.GridDesktop Worksheet][11].
*   [Find GridDesktop Version at Runtime][12].
*   Handled "System.ArgumentOutOfRangeException" when loading an MHTML file.
*   Handled NullReferenceException when saving Excel workbook to HTML file format.

Aspose.Cells 17.7 has enhanced its core for more stability as well as fixed many critical bugs. In this release, we have fixed several other issues. For example, issues around reading/writing MS Excel file formats, rendering shapes and drawing objects, resizing ListObject/Table, rendering and manipulating charts, manipulating PivotTables, rendering HTML to Excel and vice versa, [rendering images from Excel worksheets][13], [rendering images files from charts][14] and [exporting Excel workbooks to PDF format][15] have been resolved.

## Changes to the Public API

This version of Aspose.Cells for .NET has made some changes to the Public API. A few of the worth mentioning changes are as follow.

*   Added _GlobalizationSettings.GetBooleanValueString()/GetErrorValueString()_ methods that specifies custom display string value for the cell.
*   Added _PdfSaveOptions/ImageOrPrintOptions.CheckWorkbookDefaultFont_ property that indicates whether to try to use workbook's default font at first to show the characters whose font is not set correctly.
*   Added _FileFormatType.Numbers_, _LoadFormat.Numbers_ and _SaveFormat.Numbers_ enum which represents the Numbers spreadsheet file format by Apple Inc.
*   Added _GridWebInstance.resize()_ function that makes the Aspsoe.Cells.GridWeb control compatible with current browser window's size.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][16].
*   [Aspose.Cells for .NET Download Section][17].
*   [Aspose.Cells for .NET Documentation][18] – up-to-date documentation containing Programmer's Guide, Knowledge Base, and much more.
*   [Aspose.Cells for .NET API Reference Guide][19] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][20] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][21] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/net/new-releases/aspose.cells-for-.net-17.7/
[2]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+17.7+Release+Notes
[3]: https://www.nuget.org/packages/Aspose.Cells/
[4]: https://docs.aspose.com/display/cellsnet/Set+DefaultFont+property+of+PdfSaveOptions+and+ImageOrPrintOptions+to+have+priority
[5]: https://docs.aspose.com/display/cellsnet/Read+Numbers+Spreadsheet+Developed+by+Apple+Inc.+using+Aspose.Cells
[6]: https://docs.aspose.com/display/cellsnet/Apply+Advanced+Filter+of+Microsoft+Excel+to+Display+Records+Meeting+Complex+Criteria
[7]: https://docs.aspose.com/display/cellsnet/Implement+Errors+and+Boolean+Value+in+Russian+or+Any+Other+Language
[8]: https://docs.aspose.com/display/cellsnet/Resize+GridWeb+in+the+browser+window
[9]: https://docs.aspose.com/display/cellsnet/Render+PivotTable+In+GridDesktop
[10]: https://docs.aspose.com/display/cellsnet/Determine+if+Paper+Size+of+Worksheet+is+Automatic
[11]: https://docs.aspose.com/display/cellsnet/Custom+Row+And+Custom+Column+Caption+of+GridDesktop+Worksheet
[12]: https://docs.aspose.com/display/cellsnet/Find+GridDesktop+Version+At+RunTime
[13]: https://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Different+Formats
[14]: https://docs.aspose.com/display/cellsnet/Chart+Rendering
[15]: https://docs.aspose.com/display/cellsnet/Convert+Excel+Workbook+to+PDF
[16]: https://www.aspose.com/products/cells/net
[17]: https://downloads.aspose.com/cells/net
[18]: https://docs.aspose.com/display/cellsnet/home
[19]: https://apireference.aspose.com/
[20]: https://forum.aspose.com/c/cells
[21]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




