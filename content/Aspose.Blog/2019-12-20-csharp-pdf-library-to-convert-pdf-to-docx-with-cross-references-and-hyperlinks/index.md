---
title: 'Convert PDF to DOCX with Cross-References and Hyperlinks using C#'
date: Fri, 20 Dec 2019 06:51:39 +0000
draft: false
url: /2019/12/20/csharp-pdf-library-to-convert-pdf-to-docx-with-cross-references-and-hyperlinks/
author: Usman Aziz
summary: ''
tags: ['Aspose.Pdf for .NET', 'C# PDF Library', 'PDF Cross-References', 'PDF Generator API', 'PDF to DOCX', 'convert pdf to word with hyperlinks']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-net.jpg" alt="XPS Document Manipulation API for C++">}}


We are back with a major release of [Aspose.PDF for .NET][1] as **v19.12** introducing the support of cross-references and hyperlinks when converting PDF to DOCX format. In addition, we have added the strategies for font subset optimization in the PDF documents. Not only this, but we have also provided important bug fixes for PDF to DOCX, PDF to HTML, PDF to TIFF, PDF to PNG, PDF to PPTX, SVG to PDF, and PCL to PDF conversions. So let's have a look at the new features, enhancements, and bug fixes in a bit more detail.

## PDF to DOCX with Cross-References and Hyperlinks in C#

Cross-references in documents are used to refer the reader to some other part or objects such as graphs, charts or figures in the document. The PDF format allows inserting the cross-references in the documents to navigate the user to the referenced content. Similarly, hyperlinks are also used to take the reader to a particular destination inside or outside the document.

_Aspose.PDF for .NET_ supports [converting PDF to Word][2] (DOC, DOCX) formats, however, the previous versions of the API lacked the ability to support hyperlinks and cross-references in the converted Word document. This feature has now been added and the hyperlinks and cross-references are supported in the PDF to Word conversion.

## Font Subsets Optimization in PDF using C#

_Aspose.PDF for .NET_ allows embedding fonts to the PDF documents. The font can be embedded completely or as a subset of the font. However, in some cases, you may want to optimize the fonts by reducing the fully embedded font set to only subsets that are used in the PDF document. In the latest release, we have provided the optimization options to tune the font subset strategies using the [SubsetFonts][3] method. This method accepts [FontSubsetStrategy][4] which has the following variants:

*   SubsetAllFonts - This option will subset all the fonts that are used in the PDF document.
*   SubsetEmbeddedFontsOnly - This option subsets only the fonts which are fully embedded into the PDF document.

The following C# code sample shows how to apply the font subset strategy to optimize the PDF documents.

{{< gist aspose-com-gists 63473b1ba28e09e229cfbf4430eabd8a "Examples-CSharp-AsposePDF-Working-Document-EmbedFontsUsingSubsetStrategy-EmbedFontsUsingSubsetStrategy.cs" >}}

Please visit [this][5] documentation article for more details on this feature.

## Bug Fixes

The following is the list of some important bug fixes we have added to the latest release.

*   PDF to Word - System.ArgumentNullException exception occurs
*   PDF to Word - Hyperlink is lost
*   PDF to PNG - Conversion issue
*   PDF to HTML - Formatting issues in the resultant file
*   PDF to HTML - Hyperlink is removed in the resultant file
*   PDF to HTML - Text is not being rendered properly (character overwrite)
*   TIFF to PDF - Images in PDF are blurred
*   PDF to TIFF - Image conversion issue
*   SVG to PDF - Conversion adds some random lines in output PDF
*   SVG to PDF - Conversion renders the incorrect document
*   SVG to PDF - Resultant PDF appears blank
*   PCL to PDF - Resultant PDF document is missing the text
*   PCL to PDF - Conversion throws SystemException
*   PCL to PDF - An unhandled exception of type ' ' occurs
*   PCL to PDF - Conversion fails
*   PCL to PDF - Output PDF document is not correct
*   PCL to PDF - Output PDF has wrong Fonts layout
*   PCL to PDF - System.SystemException: 'Font Line Printer is absent.'
*   PCL to PDF - The method or operation is not implemented
*   PDF to PPTX - Chart Labels are missing in output
*   Cannot retrieve TextField Value
*   Exception when saving EPUB to HTML
*   Incorrect font used when viewing output HTML in Chrome
*   NullReferenceException occurs when saving PDF
*   Exception when loading a particular LaTeX (.tex) file
*   Exception when accessing page annotations of PDF document with 3D object

For a complete list of bug fixes, please visit the [release notes][6].

Alright! You can [download][7] the latest release of _Aspose.PDF for .NET_ and check out the new features using the source code [examples][8]. Consult the [documentation][9] for more details about every feature along with the code samples. In case you would find anything difficult for you, please feel free to let us know via our [forum][10].




[1]: https://products.aspose.com/pdf/net
[2]: https://docs.aspose.com/
[3]: https://apireference.aspose.com/net/pdf/aspose.pdf.document/idocumentfontutilities/methods/subsetfonts
[4]: https://apireference.aspose.com/net/pdf/aspose.pdf/fontsubsetstrategy
[5]: https://docs.aspose.com/display/pdfnet/Formatting+PDF+Document#FormattingPDFDocument-ImproveFontsEmbeddingusingFontSubsetStrategy
[6]: https://docs.aspose.com/display/pdfnet/Aspose.PDF+for+.NET+19.12+Release+Notes
[7]: https://downloads.aspose.com/pdf/net
[8]: https://github.com/aspose-pdf/Aspose.PDF-for-.NET
[9]: https://docs.aspose.com/display/pdfnet
[10]: https://forum.aspose.com/




