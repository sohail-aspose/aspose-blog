---
title: 'Convert PDF to HTML, PDF to Image and HTML to PDF using C# .NET'
date: Thu, 09 Jan 2014 14:33:17 +0000
draft: false
url: /2014/01/09/improved-pdf-to-html-pdf-to-image-and-html-to-pdf-conversion-in-aspose.pdf-for-.net-8.8.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'HTML to PDF', 'PDF to HTML', 'PDF to Image']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


It gives us great pleasure to introduce the release of [Aspose.PDF for .NET 8.8.0][1] with stable PDF to HTML, PDF to image, PDF to PostScript, and HTML to PDF conversion features. The annotation manipulation is also one of the key areas which are specifically improved in this release. The Document Object Model of the Aspose.Pdf namespace has the capability to create tables in PDF documents and while generating the table, you can specify border information for table and cell objects. Recently, one of our customers wanted to add double borders around table and cell objects. We are pleased to share that with Aspose.PDF for .NET 8.8.0, they can. Please take a look over the following code snippet to accomplish this requirement.

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-Tables-SetBorder-SetBorder.cs" >}}

For further details, please visit [Set Border Style, Margins and Padding of the Table (MergedAPI)][2].

## C# PDF to HTML - Save fonts as WOFF or TTF

Aspose.PDF for .NET offers the feature to convert HTML files to PDF and it also provides the feature to transform PDF files to HTML format. During PDF to HTML conversion, any TrueType fonts used in the PDF can be saved on the file system. In Aspose.Pdf for .NET 8.8.0, we have introduced a feature that lets you either save fonts in TTF (True Type Format) or save them as WOFF (Web Open Font Format). In order to accomplish this requirement, we have added the HtmlSaveOptions.FontSavingModes enumerator and the HtmlSaveOptions.FontSavingMode conversion option. The following code snippet shows the steps to save the fonts as TTF when converting PDF files to HTML format.

```
// Output HTML file path information
string outFile = Path.GetFullPath(TestSettings.GetOutputFile("36192.html"));
// Source PDF document
Document doc = new Document(TestSettings.GetInputFile("36192.pdf"));
// Create HtmlSaveOption with tested feature
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.FixedLayout = true;
saveOptions.SplitIntoPages = false;
// Save the fonts as TTF format
saveOptions.FontSavingMode = HtmlSaveOptions.FontSavingModes.AlwaysSaveAsTTF;
string htmlFile = Path.GetFullPath(outFile);
string linkedFilesFolder = Path.GetDirectoryName(htmlFile) + @"\36192_files";

if (Directory.Exists(linkedFilesFolder))
{
    Directory.Delete(linkedFilesFolder, true);
}
// Save the output
doc.Save(outFile, saveOptions);
```

To save the fonts as WOFF format, use this save option:

```
saveOptions.FontSavingMode = HtmlSaveOptions.FontSavingModes.AlwaysSaveAsWoff;
```

In this new release, we have also fixed some issues related to HTML to PDF conversion where multiple DIV tags were not properly rendered. Miscellaneous other formatting issues encountered in earlier versions are also fixed. The PDF to TIFF conversion has been greatly improved to handle complex documents and produce results with high fidelity. Manipulation of annotations (especially annotation import) is improved and issues related to text alignment, padding, text rotation, cloud markup losing its curves and problems related to missing arrows are fixed.

Please download and start exploring the features of [Aspose.PDF for .NET 8.8.0][3].




[1]: https://downloads.aspose.com/pdf/net
[2]: https://docs.aspose.com/display/pdfnet/Manipulate+and+Integrate+Table
[3]: https://downloads.aspose.com/pdf/net




