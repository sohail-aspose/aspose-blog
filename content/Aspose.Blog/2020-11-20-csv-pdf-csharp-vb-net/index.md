---
title: 'Convert CSV to PDF or PDF to CSV Programmatically using C# VB.NET'
seoTitle: "Convert CSV to PDF or PDF to CSV Programmatically using C# VB.NET"
description: "Convert CSV to PDF and PDF to CSV Programmatically using C# or VB.NET. Comma separated values and other delimiters can be converted easily."
date: Fri, 20 Nov 2020 16:07:51 +0000
draft: false
url: /2020/11/20/csv-pdf-csharp-vb-net/
author: Farhan Raza
summary: '[**CSV**][1] files often contain tabular data where the values are usually separated by comma delimiter. You can convert a [**CSV**][2] file to PDF as well as a PDF file to a CSV file using C# or VB.NET. Aspose APIs offer a lot of file manipulation and conversion features. Let us explore the CSV and PDF conversion.'
tags: ['C# CSV to PDF', 'C# PDF to CSV', 'CSV to PDF', 'CSV to PDF C#', 'Convert CSV to PDF', 'Convert PDF to CSV', 'PDF to CSV', 'PDF to CSV C#']
categories: ['Aspose.PDF Product Family', 'Aspose.Cells Product Family']
---

[CSV][3] files often contain tabular data where the values are usually separated by comma delimiter. You can convert a CSV file to [PDF][4] as well as a PDF file to a CSV file using [C#][5] or [VB.NET][6]. Aspose APIs offer a lot of file manipulation and conversion features. Let us explore the following headings to learn CSV and PDF conversion:

*   [CSV to PDF and PDF to CSV Converter - API Installation][7]
*   [Convert CSV to PDF File Programmatically using C# or VB.NET][8]
*   [Convert PDF to CSV File Programmatically using C# or VB.NET][9]

## CSV to PDF and PDF to CSV Converter - API Installation {#section1}

You need to install [Aspose.Cells for .NET][10] as well as [Aspose.PDF for .NET][11] API in your environment. You can quickly configure these APIs either by downloading the DLL files from the [Downloads section][12], or you can run the following commands in NuGet Package Manager under the Tools menu in Microsoft Visual Studio IDE.

*   _PM> Install-Package Aspose.Cells_
*   _PM> Install-Package Aspose.Pdf_

After configuring the APIs successfully, we are all set to perform the inter-conversion of CSV and PDF files.

## Convert CSV to PDF File Programmatically using C# or VB.NET {#section2}

CSV files contain comma-separated values which are usually differentiated by comma. Moreover, each row in a CSV file denotes a tuple or row of data. You can easily convert a CSV file to a PDF document programmatically using C# or VB.NET languages. You can control which symbol do you want to set as a separator character using TxtLoadOptions.Separator property. Likewise, you can also set a string value as a separator delimiter using TxtLoadOptions.SeparatorString property. You need to follow the steps below for converting a CSV file to PDF:

1.  Initialize [TxtLoadOptions][13] class object
2.  Specify delimiter using the [Separator][14] property
3.  Load input CSV file
4.  Save the output PDF file

The following code snippet is based on these steps which shows how to convert a CSV to PDF Programmatically using C# or VB.NET:

{{< gist aspose-com-gists e7836763c0ea85cdb50c9cf4f34c40d6 "CSVtoPDF.cs" >}}

**_Input CSV File_**

```
My Data,,,,,,,

Items A,Items B,Items C,Items D,Items E,Items F,Items G,Items H
12,23,33,66,11,87,99,33
23,22,33,77,31,22,45,56
34,11,12,23,22,34,11,12
45,43,54,88,36,45,45,37
65,65,65,65,13,65,9,35
34,22,27,22,32,23,23,32
213,186,224,341,145,276,232,205
```

**_Output PDF File Screenshot_**



{{< figure align=center src="images/Convert-CSV-PDF-Csharp.png" alt="Convert CSV PDF csharp">}}


## Convert PDF to CSV File Programmatically using C# or VB.NET {#section3}

PDF files can contain data in the form of a table. You can convert such PDF file to CSV in your .NET applications. You have already installed Aspose.PDF for .NET API using the NuGet command that we have discussed in the Installation section above. Below are the steps for converting a PDF to CSV file:

1.  Initialize [ExcelSaveOptions][15] class object
2.  Set [ExcelFormat.CSV][16] format for the output file
3.  Load input PDF file
4.  Save output CSV file

The code below shows how to convert PDF to CSV programmatically using C# or VB.NET:

{{< gist aspose-com-gists e7836763c0ea85cdb50c9cf4f34c40d6 "PDFtoCSV.cs" >}}

## Conclusion

In this article, we have explored how to convert CSV to PDF and PDF to CSV programmatically using C# or VB.NET in your .NET applications. We have learned how to parse a character or a string delimiter in the CSV files. Moreover, you can reach us out at [Free Support Forum][17] for any further help.

## See Also

[Convert CSV to Excel Files or Excel to CSV using C# VB.NET][18]




[1]: https://docs.fileformat.com/spreadsheet/csv/
[2]: https://docs.fileformat.com/pdf/
[3]: https://docs.fileformat.com/spreadsheet/csv/
[4]: https://docs.fileformat.com/pdf/
[5]: https://docs.fileformat.com/programming/cs/
[6]: https://docs.fileformat.com/programming/vb/
[7]: #section1
[8]: #section2
[9]: #section3
[10]: https://products.aspose.com/cells/net
[11]: https://products.aspose.com/pdf/net
[12]: https://releases.aspose.com/
[13]: https://apireference.aspose.com/cells/net/aspose.cells/txtloadoptions
[14]: https://apireference.aspose.com/cells/net/aspose.cells/txtloadoptions/properties/separator
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf/excelsaveoptions
[16]: https://apireference.aspose.com/pdf/net/aspose.pdf.excelsaveoptions/excelformat
[17]: https://forum.aspose.com/
[18]: https://blog.aspose.com/2020/11/17/csv-excel-csharp-vb-net/





