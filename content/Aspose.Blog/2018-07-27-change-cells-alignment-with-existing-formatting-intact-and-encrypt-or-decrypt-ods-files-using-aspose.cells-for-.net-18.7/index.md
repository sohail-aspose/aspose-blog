---
title: 'Change Cells Alignment with Existing Formatting Intact in Excel using C# .NET'
date: Fri, 27 Jul 2018 11:12:16 +0000
draft: false
url: /2018/07/27/change-cells-alignment-with-existing-formatting-intact-and-encrypt-or-decrypt-ods-files-using-aspose.cells-for-.net-18.7/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


We are pleased to announce the release of [Aspose.Cells for .NET v18.7][1]. Please check the [document][2] on how to install Aspose for .NET APIs directly from NuGet repository. In this release, we have added some utility features for the users. Moreover, we included important fixes and other enhancements in the release. Please check the [release notes][3] in order to get an idea about what is new and what has been enhanced or fixed with this revision of Aspose.Cells for .NET.

## Change Cells Alignment and Keep Existing Formatting

If you need to change the alignment of multiple cells but also want to keep existing formattings intact, Aspose.Cells allows you to do that using the **StyleFlag.Alignments** property. Please note, **StyleFlag** object is passed as a parameter to **Range.ApplyStyle()** method which actually applies the formatting to your desired range of cells. The following sample code loads the sample Excel file, creates the range and center aligns it horizontally and vertically and keeps the existing formatting intact.

{{< gist aspose-com-gists 24a8eac23c3325e20dababecf735a43b "Data-ChangeCellsAlignmentAndKeepExistingFormatting.cs" >}}

Please see the following article for more detail on this topic for your reference.

*   [Change Cells Alignment and Keep Existing Formatting][4]

## Find Maximum Rows and Columns in XLS and XLSX

For your information, there are a different number of rows and columns supported by different MS Excel file formats. For example, XLS supports up to 65536 rows and 256 columns while XLSX supports 1048576 rows and 16384 columns. If you want to know how many rows and columns are supported by a given format, you can use **Workbook.Settings.MaxRow** and **Workbook.Settings.MaxColumn** properties. Please see the following article for more detail on this topic for your reference:

*   [Find Maximum Rows and Columns supported by XLS and XLSX formats][5]

## Specify Author while Write Protecting Workbook

You can specify author name while write protecting your workbook using Aspose.Cells API. Please use **Workbook.Settings.WriteProtection.Author** property for this purpose. Please see the following article for more detail on this topic for your reference:

*   [Specify Author while Write Protecting Workbook][6]

## Encrypt/Decrypt an ODS File

Aspose.Cells allows you to encrypt and decrypt an ODS file. Decrypted ODS file can be opened both in MS Excel and OpenOffice, however encrypted ODS file can only be opened by OpenOffice after providing the password. Excel cannot open the encrypted ODS file and may raise warning message. For encrypting an ODS file, load the file and set the **WorkbookSettings.Password** value to the actual password before saving it. Please see the following article for more detail on this topic for your reference:

*   [Encrypt/Decrypt an ODS file][7]

## Other Enhancements and Fixes

There are some other enhancements included and a few exceptions handled in the new release for the users. A few of the worth mentioning features and other improvements are as follows.

*   Round images become square images in the output PDF.
*   Support Pivot Table Slicers.
*   Using "List<dynamic>" or "List<ExpandoObject>" as DataSource for importing data into worksheet.
*   Handled "Index out of range" exception in SheetRender.ToImage method.
*   Exception: "Invalid parameters for function iferror...." when loading an Excel file.
*   Invalid PatternType string value exception while loading a file.

## Changes to the Public API

The following is a list of any changes made to the public API such as added, renamed, removed or deprecated members as well as any non-backward compatible change made to Aspose.Cells for .NET:

*   Adds **enum StyleFlag.Alignments**, it represents all the settings of alignment.
*   Adds **WorkbookSettings.MaxRow** and **WorkbookSettings.MaxColumn** properties, these attributes gets the max row and column indexes of the workbook.
*   Adds **WriteProtection.Author** property, it gets and sets the author of the write protection.

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][8].
*   [Install Aspose for .NET APIs from NuGet repository][9]
*   [Aspose.Cells for .NET Documentation][10] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][11] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][12] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][13] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Cells/18.7.0
[2]: https://docs.aspose.com/display/cellsnet/Installation#Installation-InstallAspose.Cellsfor.NETthroughNuGet
[3]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+18.7+Release+Notes
[4]: https://docs.aspose.com/display/cellsnet/Change+Cells+Alignment+and+Keep+Existing+Formatting
[5]: https://docs.aspose.com/display/cellsnet/Find+Maximum+Rows+and+Columns+supported+by+XLS+and+XLSX+formats
[6]: https://docs.aspose.com/display/cellsnet/Specify+Author+while+Write+Protecting+Workbook
[7]: https://docs.aspose.com/display/cellsnet/Encrypting+Excel+Files#EncryptingExcelFiles-Encryption/DecryptionofODSfilewithAspose.Cells
[8]: https://products.aspose.com/cells/net
[9]: https://www.nuget.org/packages/Aspose.Cells
[10]: https://docs.aspose.com/display/cellsnet/home
[11]: https://apireference.aspose.com/
[12]: https://forum.aspose.com/c/cells
[13]: https://github.com/aspose-cells/Aspose.Cells-for-.NET




