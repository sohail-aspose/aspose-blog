---
title: 'Convert DICOM to PDF Aspose.PDF for .NET 17.10'
date: Tue, 14 Nov 2017 18:08:09 +0000
draft: false
url: /2017/11/14/dicom-image-to-pdf-conversion-and-print-dialog-presets-properties-with-aspose.pdf-for-.net-17.10/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Convert DICOM images to PDF in Csharp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-net.jpg" alt="Aspose.Pdf for .NET logo">}}


We are very much excited to announce the release of [Aspose.PDF for .NET 17.10][1] which offers various enhancements and fixes related to issues reported in previous release versions. We are always striving to make the API robust enough to cater to a wide variety of input documents and with every new release, the API is becoming more stable, as new enhancements and bug fixes are being introduced.

## Convert DICOM to PDF in C#

Digital Imaging and Communications in Medicine (DICOM) is a standard for storing and transmitting medical images enabling the integration of medical imaging devices such as scanners, servers, workstations, printers, etc. Aspose.PDF for .NET is capable of [converting various image formats to PDF][2] and other supported formats. Recently we received a requirement to convert DICOM images to PDF format, so in order to cater to this scenario, we are pleased to announce the support of this format. In order to accomplish this requirement, please try using the following code snippet

```
string outputFile = @"c:\mr-shoulder.pdf";
using (Document pdfDocument = new Document())
{
     pdfDocument.Pages.Add();
     Aspose.Pdf.Image image = new Aspose.Pdf.Image();
     image.FileType = ImageFileType.Dicom;
     image.File = @"c:\mr-shoulder.dcm";
     pdfDocument.Pages[1].Paragraphs.Add(image);
     // Save output as PDF format
     pdfDocument.Save(outputFile);
}
```

## Set Print Dialog Presets Properties

Recently one of the customers shared a **requirement to change DuplexMode** property to the duplex of Print Dialog Presets (In Adobe Acrobat choose File > Properties -> Advanced tab). Whereas in the Print Dialog (Presets section) of PDF document, the default value is set to simplex. We can set the Duplex property of PrinterSettings object while printing through the PdfViewer class but the API lacked the feature to set PDF document property. Therefore, in order to accomplish this requirement, support is provided in API and the following code snippet can be used.

```
string outputFile = @"c:\35297.pdf";
using (Document doc = new Document())
{
       doc.Pages.Add();
       doc.Duplex = PrintDuplex.DuplexFlipLongEdge;
       doc.Save(outputFile);
}
```

#### PdfContentEditor Approach```
string outputFile = @"c:\old_file.pdf";
string outputFile1 = @"c:\new_file.pdf";
using (PdfContentEditor ed = new PdfContentEditor())
{
       ed.BindPdf(outputFile);
       if ((ed.GetViewerPreference() & ViewerPreference.DuplexFlipShortEdge) > 0)
       {
           Console.WriteLine("The file has duplex flip short edge");  
       }    
       ed.ChangeViewerPreference(ViewerPreference.DuplexFlipShortEdge);
       ed.Save(outputFile1);
}
```

## Vertical Alignment Property for Row Instance

In legacy Aspose.Pdf.Generator, we had a VerticalAlign property on row objects and in order to provide a similar feature in the new Document Object Model of Aspose.PDF namespace, we have added a similar property for Aspose.Pdf.Row instance.

```
// Load source PDF document
Aspose.Pdf.Document doc = new Aspose.Pdf.Document();
doc.Pages.Add();
// Initializes a new instance of the Table
Aspose.Pdf.Table table = new Aspose.Pdf.Table();
// Set the table border color as LightGray
table.Border = new Aspose.Pdf.BorderInfo(Aspose.Pdf.BorderSide.All, .5f, Aspose.Pdf.Color.FromRgb(System.Drawing.Color.LightGray));
// set the border for table cells
table.DefaultCellBorder = new Aspose.Pdf.BorderInfo(Aspose.Pdf.BorderSide.All, .5f, Aspose.Pdf.Color.FromRgb(System.Drawing.Color.LightGray));
// create a loop to add 10 rows
for (int row_count = 1; row_count < 10; row_count++)
{
    // add row to table
    Aspose.Pdf.Row row = table.Rows.Add();
    // set vertical alignment for Row instance
    row.VerticalAlignment = VerticalAlignment.Center;
    // add table cells
    row.Cells.Add("Column (" + row_count + ", 1)");
    row.Cells.Add("Column (" + row_count + ", 2)");
    row.Cells.Add("Column (" + row_count + ", 3)");
}
// Add table object to first page of input document
doc.Pages[1].Paragraphs.Add(table);
// Save updated document containing table object
doc.Save("document_with_table.pdf"); 
```

## Miscellaneous fixes

Apart from the above-mentioned improvements, the API is improved to generate better results for PDF to SVG or SVG to PDF conversion and it has also been improved to accept password in a foreign language when encrypting or decrypting PDF files. The PDF to PDF/A compliance conversion is improved to cater to more scenarios and for other inter file format conversion scenarios, there have been significant efforts towards the stability of PDF to HTML conversion feature.

As it is always recommended to use the latest release of our API's, so we suggest you please download the latest release of [Aspose.PDF for .NET 17.10][3] and check [Release Notes][4] section for the list of issues fixed in Aspose.Pdf for .NET 17.10

*   [Home page for Aspose.PDF for .NET][5]
*   [Download Aspose.PDF for .NET][6]
*   [Aspose.PDF product family forum][7]– Post your technical questions and queries, or any other problem you faced while running Aspose.Pdf APIs.
*   [Aspose.PDF for .NET online documentation][8]– help documentation and API reference documents.
*   [Enable Blog Subscription][9]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Pdf APIs, new features, fixes and other API related topics by subscribing to Aspose.Pdf blog.
*   [Aspose.PDF for .NET Examples][10] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/pdf/net/new-releases/aspose.pdf-for-.net-17.10/
[2]: https://docs.aspose.com/
[3]: https://downloads.aspose.com/pdf/net/new-releases/aspose.pdf-for-.net-17.10/
[4]: https://docs.aspose.com/display/pdfnet/Aspose.Pdf+for+.NET+17.10+Release+Notes
[5]: https://products.aspose.com/pdf/net
[6]: https://downloads.aspose.com/pdf/net
[7]: https://forums.aspose.com/c/pdf
[8]: https://docs.aspose.com/display/pdfnet/Home
[9]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/
[10]: https://github.com/aspose-pdf/Aspose.Pdf-for-.NET




