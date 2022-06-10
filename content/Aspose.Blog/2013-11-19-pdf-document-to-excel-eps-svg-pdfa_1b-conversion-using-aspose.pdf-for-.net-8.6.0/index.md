---
title: 'Convert PDF Document to Excel, EPS, SVG, PDF/A_1b Using Aspose.Pdf for .NET 8.6.0'
date: Tue, 19 Nov 2013 11:19:25 +0000
draft: false
url: /2013/11/19/pdf-document-to-excel-eps-svg-pdfa_1b-conversion-using-aspose.pdf-for-.net-8.6.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Convert PDF to EPS', 'Convert PDF to SVG', 'EPS', 'PDF to Excel conversion', 'convert pdf to excel']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="PDF to Excel, PDF to EPS, PDF to SVG">}}


The Aspose team is excited to announce the release of [Aspose.PDF for .NET 8.6.0][1]. This release includes a very exciting and demanding feature that lets you convert a PDF file to an Excel spreadsheet. Using this new release, developers can convert PDF documents to XLS format, where each individual pages in the PDF file appears as a separate worksheet. The following code snippet shows how to use this feature.

## Convert PDF to Excel

The following code sample shows how to convert PDF to Excel XLS in C#.

```
// Load PDF document
Aspose.Pdf.Document doc = new Aspose.Pdf.Document(@"C:\input.pdf");
// Instantiate ExcelSave Option object
Aspose.Pdf.ExcelSaveOptions excelsave = new ExcelSaveOptions();
// Save the output in XLS format
doc.Save("c:/resultant.xls", excelsave);
```

## Convert PDF to PS or EPS

The earlier versions of Aspose.PDF for .NET supports [converting PDF files to PS format][2] and to convert the PDF document to EPS format, you only have to change PrintFileName as shown below.

```
PrinterSettings.PrintFileName ="Hello.eps";
```

The only difference between ways of getting PS and EPS files are in the Printer Options. Please take a look of the Printing to EPS section of [Using LaTeX with EPS Figures][3]. By default '**HP LaserJet 2300 Series PS**' printer and any other PS printer creates PS files. You can change the PostScript Output Option to Encapsulated Postscript (EPS) to save EPS files.

## Convert PDF to SVG

It's been possible to convert SVG to PDF with Aspose.Pdf for quite some time. In this release, we have introduced the feature to directly save PDF files to SVG format. The following code snippet shows the simple code lines to convert PDF to SVG in C#.

```
// Load PDF document
Aspose.Pdf.Document doc = new Aspose.Pdf.Document(@"C:\TableResult.pdf");
Aspose.Pdf.SvgSaveOptions saveOptions = new Aspose.Pdf.SvgSaveOptions();
// Do not compress SVG image to Zip archive
saveOptions.CompressOutputToZipArchive = false;
// Output file name
string outFileName = @"C:\output.svg";
doc.Save(outFileName, saveOptions);
```

During PDF to HTML conversion, you can also specify a separate folder for image files. Further details can be found in the [PDF to HTML conversion][4] topic.

This release is a great improvement on earlier releases and provides much better support for PDF to PDF/A\_1b, PDF to XPS, TIFF to PDF, XSL-FO to PDF, text extraction and other features. Please be the first to download and start exploring the new features of [Aspose.PDF for .NET 8.6.0][5].




[1]: https://downloads.aspose.com/pdf/net
[2]: https://docs.aspose.com/display/pdfnet/Working+with+Document+Conversion
[3]: http://embedded.eecs.berkeley.edu/concurrency/latex/latexWithEPS.html
[4]: https://docs.aspose.com/display/pdfnet/Convert+PDF+file+into+HTML+format
[5]: https://downloads.aspose.com/pdf/net




