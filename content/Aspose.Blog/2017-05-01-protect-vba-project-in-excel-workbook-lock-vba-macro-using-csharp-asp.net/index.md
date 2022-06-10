---
title: 'Protect VBA Project in Excel Workbook and Lock it for Viewing using C# .NET'
date: Mon, 01 May 2017 15:26:55 +0000
draft: false
url: /2017/05/01/protect-vba-project-in-excel-workbook-lock-vba-macro-using-csharp-asp.net/
author: Amjad Sahi
summary: ''
tags: ['Protect VBA project in Excel in csharp', 'Secure Excel VBA project', 'password protect VBA code in Excel']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce our next version of [Aspose.Cells for .NET v17.4.0][1]. The new release includes some valuable features and other enhancements with critical bug fixes. We have added certain features regarding protection of VBA projects in Excel workbooks. There is also an enhancement for data sorting and custom pattern formatting. Our clients may [get the powerful Aspose for .NET APIs directly from NuGet repository][2]. Please see the detailed [release notes][3] in order to get an idea about what is new and what has been fixed with this version of Aspose.Cells for .NET. The release notes also list any changes made to the public API such as added, renamed, removed or deprecated members (if any) as well as any non-backward compatible change made to Aspose.Cells for .NET.

## Protect VBA Project in Excel Workbook using C#

Aspose.Cells now supports the feature of protecting the VBA (Visual Basic for Applications) Project of Excel Workbook and locking it for viewing. Besides, you can also find if an existing VBA project is already protected and locked for viewing. Please see these articles for a reference.

*   [Password Protect the VBA Project of Excel Workbook][4]
*   [Check if VBA Project is Protected and Locked for Viewing][5]
*   [Find out if VBA Project is Protected][6]

The following C# code snippet demonstrates how to protect your Excel Workbook VBA Project dynamically using Aspose.Cells and lock it for viewing.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Examples-CSharp-WorkbookVBAProjectPassword-ProtecttheVBAProjectofExcelWorkbook.cs" >}}

## Specifying Sort Warning While Sorting Data

Aspose.Cells already supports Data Sorting, however earlier you could not sort your textual data as numerical data. For this purpose, Aspose.Cells implemented the **DataSorter.SortAsNumber** property. Whenever you sort textual data that looks like a number, MS-Excel shows this warning. **DataSorter.SortAsNumber** property implements this MS-Excel warning.



{{< figure align=center src="images/sort-textual-data-as-numbers-300x208.png" alt="Protect Excel VBA in C#">}}


Please see this article for more help relating to this topic.

*   [Specifying Sort Warning While Sorting Data][7]

## Specifying DBNum Custom Pattern Formatting

Aspose.Cells supports the **DBNum** custom pattern formatting. For example, if your cell value is **123** and you specify its custom formatting as **\[DBNum2\]\[$-804\]General** then it will be displayed like **壹佰贰拾叁**. You can specify the custom formatting of your cell using Cell.GetStyle() method and Style.Custom attribute.

*   [Specifying DBNum Custom Pattern Formatting][8]

## Other Enhancements and Fixes

Aspose.Cells for .NET 17.4.0 has enhanced its core for more stability as well as fixed many critical bugs. Moreover, there are numerous minor enhancements in order to improve the overall usage of the API. A few of the worth mentioning enhancements are as follows.

*   [Set Column Header ToolTip][9].
*   Sparklines disappear after re-saving and rendering to PDF.
*   Formatting error inside shapes texts when Excel is converted to PDF.
*   VbaProject.Sign causes an exception.
*   Re-adding a picture to the same XLS throws a Null Reference error.

Furthermore, in this release, we have fixed several other issues. For example, issues around reading/writing MS Excel file formats, manipulating Pivot Tables, applying formatting to cells, manipulating Ole Objects and shapes, rendering and manipulating charts, rendering HTML to Excel and vice versa, rendering images from Excel worksheets, [rendering images files from charts][10] and exporting Excel workbooks to PDF format have been resolved. The formula calculation engine is enhanced too in the new release.

## Changes to the Public API

This version of Aspose.Cells for .NET has made some changes to the Public API. A few of the worth mentioning changes are as follow:

*   VbaProject.Protect(bool islockedForViewing,string password) method is added.
*   VbaProject.IsProtected property is added.
*   VbaProject.IslockedForViewing property is added.
*   CopyOptions.ExtendToAdjacentRange property is added.
*   DataSorter.SortAsNumber property is added.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][11].
*   [Aspose.Cells for .NET Download Section][12].
*   [Aspose.Cells for .NET Documentation][13] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][14] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][15] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][16] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/net
[2]: https://www.nuget.org/packages/Aspose.Cells/
[3]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+17.4.0+Release+Notes
[4]: https://docs.aspose.com/display/cellsnet/Password+Protect+the+VBA+Project+of+Excel+Workbook
[5]: https://docs.aspose.com/display/cellsnet/Check+if+VBA+Project+is+Protected+and+Locked+for+Viewing
[6]: https://docs.aspose.com/display/cellsnet/Find+out+if+VBA+Project+is+Protected
[7]: https://docs.aspose.com/display/cellsnet/Specifying+Sort+Warning+While+Sorting+Data
[8]: https://docs.aspose.com/display/cellsnet/Specifying+DBNum+Custom+Pattern+Formatting
[9]: https://docs.aspose.com/display/cellsnet/Set+Column+Header+Tip
[10]: https://docs.aspose.com/display/cellsnet/Convert+an+Excel+Chart+to+Image
[11]: https://www.aspose.com/products/cells/net
[12]: https://downloads.aspose.com/cells/net
[13]: http://docs.aspose.com/display/cellsnet/home
[14]: https://apireference.aspose.com/cells/net
[15]: https://forum.aspose.com/
[16]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




