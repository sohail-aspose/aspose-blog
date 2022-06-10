---
title: 'Read or Write SXC and FODS Files using C# with Aspose.Cells for .NET 19.6'
date: Mon, 22 Jul 2019 18:35:42 +0000
draft: false
url: /2019/07/22/read-write-sxc-and-fods-files-with-aspose.cells-for-.net-19.6/
author: Amjad Sahi
summary: ''
tags: ['Read or Write FODS using csharp', 'Read or Write SXC using csharp']
categories: ['Aspose.Cells Product Family']
---

Do you need to process SXC and FODS file formats and want to have an API to handle these files? Aspose.Cells is the right library which will enable you to open or edit and save both OpenOffice/LibreOffice file types. You may also find other features and enhancements in the new Aspose.Cells for .NET v19.6. So let's not wait another moment to review the [release notes][1].  To get complete details of the public release ([Aspose.Cells for .NET v19.6][2], I am giving you a preview of the new features, enhancements, and fixes available in it.

## Read or Write SXC and FODS Files using C#

We always try to provide features that are supported by other spreadsheet handling software. Many users demanded the support of SXC and FODS file types which are very common. So, here we are with the support of these file types in the latest release. Following is a brief description of these types along with the detail of their support in Aspose.Cells.

### SXC Files

Spreadsheet created by StarOffice Calc; supports formulas, functions, charts, and macros; also includes DataPilot tables, which can automatically extract and summarize data from raw data sets. SXC files are also compatible with Apache OpenOffice Calc and can be exported in Microsoft Excel or IBM Lotus 1-2-3 formats.

### FODS Files

Spreadsheet saved in the OpenDocument format, but stored as a flat XML file instead of the [.][3].ZIP container used by .ODS files; allows the spreadsheet information to be more human readable; also can be an easier alternative than the ODS format for generating spreadsheets automatically without needing a spreadsheet editor.

## Generate SXC or FODS File

You can generate SXC and FODS file using FileFormatType as an argument in Workbook constructor i.e. use FileFormatType.SXC and FileFormatType.FODS as an argument.

### Load file

These files can be loaded using enumerator LoadFormat as follows: 

#### SXC File

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-Files-Handling-OpeningSXCFiles-1.cs" >}}

#### FODS File

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-Files-Handling-OpeningFODSFiles-1.cs" >}}

### Save File

The saving file of these types is quite easy by using SaveFormat enumerator while calling the Workbook.Save() function with second argument as SaveFormat.SXC and SaveFormat.FODS.

## Other enhancements and fixes

*   [Draw Slicer while rendering Excel to PDF][4].
*   Export Comments while Saving Excel file to Html.
*   Embedded OOXML file as a package for XLSX.
*   Security warning after re-saving an XLS file format.
*   Problems with medium lines/thick lines when XLSX saved as ODS.
*   Detecting whether the object file is chart or oleobject for ODS.
*   Handled "System.InvalidCastException".
*   Handled "Shape to image error!" when converting XLSX to PDF.
*   Handled an exception "System.StackOverflowException" on rendering an Excel file to PDF file format.

To use these features and avail other enhancements and fixes, I recommend you to try the release [Aspose.Cells for .NET v19.6][5]. Moreover, I recommend you to browse [Developers’ Guide][6] for your complete reference on what you can deliver using the APIs. Also, you are always welcome to share your review, concerns or feedback on [forums][7].




[1]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+19.6+Release+Notes
[2]: https://www.nuget.org/packages/Aspose.Cells/19.6.0)
[3]: https://fileinfo.com/extension/zip
[4]: https://docs.aspose.com/display/cellsnet/Draw+Slicer+while+rendering+Excel+to+PDF
[5]: https://downloads.aspose.com/cells/net/new-releases/aspose.cells-for-.net-19.6/
[6]: https://docs.aspose.com/display/cellsnet/Developer+Guide
[7]: https://forum.aspose.com/c/cells




