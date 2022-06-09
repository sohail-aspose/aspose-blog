---
title: 'Convert Excel Files to PDF on Linux using .NET'
seoTitle: "Convert Excel to PDF on Linux | .NET Spreadsheet API for Linux"
description: "Learn how to convert Excel XLSX or XLS file to PDF on Linux platform. Convert XLSX or XLS files to PDF with additional options."
date: Tue, 12 Oct 2021 14:17:23 +0000
draft: false
url: /2021/10/12/convert-excel-files-to-pdf-on-linux/
author: Usman Aziz
summary: '[PDF][1] is a popular file format which is widely used to share or print documents. In various cases, the documents of other file formats, such as spreadsheets, are converted to PDF. In this article, you are going to learn **how to convert Excel files to PDF programmatically on the Linux platform**. We will perform this conversion using a .NET spreadsheet manipulation API named [Aspose.Cells for .NET][2].'
tags: ['excel to pdf on linux', 'xls to pdf on linux', 'xlsx to pdf on linux']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Excel-to-PDF-Linux.jpg" alt="Excel to PDF Linux">}}


[PDF][3] is a popular file format which is widely used to share or print documents. In various cases, the documents of other file formats, such as spreadsheets, are converted to PDF. In this article, you are going to learn **how to convert Excel files to PDF programmatically on the Linux platform**. We will perform this conversion using a .NET spreadsheet manipulation API named [Aspose.Cells for .NET][4].

*   [Excel to PDF Converter API for Linux][5]
*   [Convert an Excel File to PDF on Linux][6]
*   [Customize Excel to PDF Conversion][7]

## .NET Excel to PDF Converter API for Linux {#Excel-to-PDF-Converter-API-for-Linux}

[Aspose.Cells for .NET][8] is a powerful and widely used class library that offers a range of spreadsheet manipulation features. Using the API, you can create, manipulate, and convert Excel files. Before we begin the demonstration of how to convert Excel files to PDF, you need to set up the .NET environment on Linux, which can be done within a few minutes. The following are the prerequisites that you would need to prepare the environment.

*   [Visual Studio Code][9]
*   [C# Extension][10]
*   [.NET 5.0 SDK][11]

Learn [how to create a console application on Linux][12] using Visual Studio Code.

Once you have completed setting up the environment, you can proceed to install Aspose.Cells for .NET in your application. For this, you can use the [NuGet Package Manager extension][13] for Visual Studio Code and install the API via [NuGet][14].

## Convert an Excel File to PDF on Linux {#Convert-an-Excel-File-to-PDF-on-Linux}

The following are the steps to convert an Excel XLSX/XLS file to PDF on Linux using Aspose.Cells for .NET.

1.  Create an instance of [Workbook][15] class and initialize it with the Excel file's path.
2.  Convert Excel to PDF using [Workbook.Save(string, SaveFormat)][16] method.

The following code sample shows how to convert an Excel file to PDF.

{{< gist aspose-com-gists b602d39a748d19d9a8bea05b56f83105 "excel-to-pdf.cs" >}}

## Customize Excel to PDF Conversion {#Set-PDF-Compliace-in-Excel-to-PDF-Conversion}

You can also set the additional options to customize the Excel to PDF conversion. For example, you can set the compliance level of the converted PDF document. The following are the steps to define additional options in Excel to PDF conversion on Linux.

1.  Create an instance of [Workbook][17] class and initialize it with the Excel file's path.
2.  Create an instance of [PdfSaveOptions][18] class and set options such as [PdfSaveOptions.Compliance][19].
3.  Convert Excel to PDF using [Workbook.Save(string, PdfSaveOptions)][20] method.

The following code sample shows how to set PDF compliance in Excel to PDF conversion.

{{< gist aspose-com-gists b602d39a748d19d9a8bea05b56f83105 "excel-to-pdf-customized.cs" >}}

## Get a Free License {#Get-a-Free-License}

You can get a [temporary license][21] and use Aspose.Cells for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to convert Excel files to PDF on Linux. Moreover, you have seen how to set additional options in Excel to PDF conversion. Besides, you can explore more about Aspose.Cells for .NET using the [documentation][22]. Also, you can ask your questions via our [forum][23].

## See Also

*   [Create, Read, and Edit Excel Spreadsheets in ASP.NET MVC][24]
*   [Create Excel Files in C# without MS Office][25]




[1]: https://docs.fileformat.com/pdf/
[2]: https://products.aspose.com/cells/net
[3]: https://docs.fileformat.com/pdf/
[4]: https://products.aspose.com/cells/net
[5]: #Excel-to-PDF-Converter-API-for-Linux
[6]: #Convert-an-Excel-File-to-PDF-on-Linux
[7]: #Set-PDF-Compliace-in-Excel-to-PDF-Conversion
[8]: https://products.aspose.com/cells/net
[9]: https://code.visualstudio.com/
[10]: https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp
[11]: https://dotnet.microsoft.com/download
[12]: https://docs.microsoft.com/en-us/dotnet/core/tutorials/with-visual-studio-code
[13]: https://marketplace.visualstudio.com/items?itemName=jmrog.vscode-nuget-package-manager
[14]: https://www.nuget.org/packages/Aspose.Cells
[15]: https://apireference.aspose.com/net/cells/aspose.cells/workbook
[16]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/3
[17]: https://apireference.aspose.com/net/cells/aspose.cells/workbook
[18]: https://apireference.aspose.com/cells/net/aspose.cells/pdfsaveoptions
[19]: https://apireference.aspose.com/cells/net/aspose.cells/pdfsaveoptions/properties/compliance
[20]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/4
[21]: https://purchase.aspose.com/temporary-license
[22]: https://docs.aspose.com/cells/net
[23]: https://forum.aspose.com/
[24]: https://blog.aspose.com/2021/08/25/create-read-edit-excel-spreadsheet-in-asp-net-mvc/
[25]: https://blog.aspose.com/2020/01/21/create-excel-xls-xlsx-programmatically-in-csharp-net/




