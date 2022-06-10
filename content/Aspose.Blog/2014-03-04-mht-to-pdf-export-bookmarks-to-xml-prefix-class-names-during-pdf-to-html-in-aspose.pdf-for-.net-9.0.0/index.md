---
title: 'Convert MHT to PDF, Export Bookmarks to XML, Prefix Class Names During PDF to HTML Conversion in Aspose.Pdf for .NET 9.0.0'
date: Tue, 04 Mar 2014 05:51:11 +0000
draft: false
url: /2014/03/04/mht-to-pdf-export-bookmarks-to-xml-prefix-class-names-during-pdf-to-html-in-aspose.pdf-for-.net-9.0.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Convert MHT to PDF in Java', 'Export bookmarks from PDF to XML', 'convert PDF to HTML']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


The conversion of HTML to PDF and PDF to HTML are one of the features most requested by our customers. Although the HTML format is quite complex because there are so many custom tags and their exact rendering inside PDF is a complex job, our developers are working to provide support for all HTML tags.

Many of our customers generate PDF files and want to display them ins web browsers. One approach is to load custom PDF viewing controls provided by Adobe or other companies or, the PDF files can be converted to HTML format and then HTML can be rendered in the web browser. The simplest conversion of PDF to HTML can be accomplished with two-lines of code and the output can be displayed in a web browser.

## Advanced PDF to HTML Conversion

You can also use the advanced features offered by our API during PDF to HTML conversion. Some of the recent enhancements include:

*   [Add the ability to prefix CSS class names in style.css][1]
*   [Add a prefix to import directives][2]

## MHT to PDF conversion

Another exciting feature introduced in [Aspose.PDF for .NET 9.0.0][3] is the conversion of MHT to PDF format. The single web archive can now be converted to PDF format using MhtLoadOptions class.

```
string inFile = "@F:\\ExternalTestsData\\email.mht";
string outFile = "@F:\\ExternalTestsData\\email.pdf";
MhtLoadOptions options = new MhtLoadOptions();
// Load PDF document
Aspose.Pdf.Document document = new Document(inFile, options);
// Save the output as PDF document
document.Save(outFile);
```

For further details, please take a look at [Convert MHT to PDF Format][4]

## Working with Digital Signatures

Aspose.Pdf for .NET provides the capability to digitally sign PDF files by [adding digital signatures][5]. While adding a signature, we add signer information and assign an image for the signature's appearance. The recent release of Aspose.Pdf for .NET now offers the feature to extract signature information from digitally signed PDF file. For further details, please visit:

*   [How to extract signature information using the PdfFileSignature class][6]
*   [Extract image from signature field using the PdfFileSignature class][7]

## Export Bookmarks to XML

As well as the features mentioned above, other enhancements have also been introduced in this release. The methods ExportBookmarksToXML(...) and ImportBookmarksWithXML(...) with Stream arguments are implemented in the PdfBookmarkEditor class. So now extracted bookmarks can be saved into stream object.

```
PdfBookmarkEditor editor = new PdfBookmarkEditor();
Document pdf = new Aspose.Pdf.Document("36394.pdf");
editor.BindPdf(pdf);
MemoryStream ms = new MemoryStream();
editor.ExportBookmarksToXML(ms);
```

For more information, please take a look at [Export Bookmarks to XML Format.][8]

## Improved Performance for PDF Concatenation

In some cases, when there are a lot of outlines, users may disable them by setting CopyOutlines to false and improve performance of concatenation. Therefore, the CopyOutlines property has been added in PdfFileEditor class.

```
PdfFileEditor pfe = new PdfFileEditor();
string[] files = Directory.GetFiles(dir);
pfe.CopyOutlines = false;
pfe.Concatenate(files, TestSettings.GetOutputFile("out.pdf"));
```

Be the first to download and start exploring the features of [Aspose.PDF for .NET 9.0.0][9].




[1]: https://docs.aspose.com/display/pdfnet/Convert+PDF+File+into+HTML+Format#ConvertPDFFileintoHTMLFormat-PDFtoHTML-PrefixCSSClassNamesinstyle.css
[2]: https://docs.aspose.com/display/pdfnet/Convert+PDF+File+into+HTML+Format#ConvertPDFFileintoHTMLFormat-PDFtoHTML-AddaPrefixtoImportDirectives
[3]: https://downloads.aspose.com/pdf/net
[4]: http://docs.aspose.com/display/pdfnet/Convert+MHT+to+PDF+format
[5]: https://docs.aspose.com/display/pdfnet/Digitally+sign+PDF+file
[6]: https://docs.aspose.com/display/pdfnet/Extract+Image+and+Signature+Information
[7]: https://docs.aspose.com/display/pdfnet/Extract+Image+and+Signature+Information
[8]: https://docs.aspose.com/display/pdfnet/Import+and+Export+Bookmarks
[9]: https://downloads.aspose.com/pdf/net




