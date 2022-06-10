---
title: 'Generate Multi-Column PDF Document using C# or VB.NET'
date: Wed, 22 Apr 2015 07:08:34 +0000
draft: false
url: /2015/04/22/generate-multi-column-pdf-using-csharp-or-vb.net-pdf-library/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Generate Multi-Column PDF using Csharp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


We are pleased to announce the release of another exciting version of [Aspose.PDF for .NET 10.3.0][1] which is a better and an optimized version, as compared to earlier releases. This new release provides some great features and enhancements, which keeps this API high among the list of its competitors. At Aspose, we are always striving to provide high demanding features, with such ease that our customers can accomplish their requirements, with a minimal set of code lines, even with a couple of code lines. Isn't that exciting!

## Create a Multi-Column PDF using C#

Magazines and newspapers mostly have news; mostly displayed in multiple columns on the single pages instead of the books where text paragraphs are mostly printed on the whole pages from left to the right position. Many document processing applications like Microsoft Word and Adobe Acrobat Writer allow users to create multiple columns on a single page and then add data to them. Aspose.Pdf for .NET also offers the feature to create multiple columns inside the pages of PDF documents. For related details, please visit Create Multi-Column PDF document.

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-Text-CreateMultiColumnPdf-CreateMultiColumnPdf.cs" >}}

## PDF to PPTX Conversion in C#

We have an API named [Aspose.Slides][2] which provides the feature to create as well as manipulate existing MS PowerPoint presentations. It also offers the feature to convert PPT/PPTX files to PDF format, so that the resultant file can be viewed across multiple platforms, without compromising the layout/formatting of the document. We know that PDF is one of the widely used file format for data sharing because it ensures the document structure/contents remain intact when viewing the file over various platforms/devices and even it does not matter what your regional or personal system preferences are. In order to deal with PDF format, Aspose.Pdf for .NET is one of the great API's in the industry to facilitate users to programmatically create as well as manipulate any existing PDF files. Recently many of our customers requested a feature to transform PDF files to PPTX format, and we are pleased to share that this new release of Aspose.Pdf for .NET offers this great feature. So in order to accomplish this requirement, you only need to instantiate an object of **PptxSaveOptions** class and pass it as the second argument to Document.Save(..) method. For further details, please take a look over [Convert PDF to PPTX][3].

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-DocumentConversion-PDFToPPT-PDFToPPT.cs" >}}

## Attachment Support in PDF/A Format

PDF/A is a widely used standard to preserve data inside the document for the long term and also to ensure the integrity of data inside the document (the document is not modified, once its compliance is set to PDF/A format). Recently we have come across a requirement to provide support for attachments in PDF/A files and as per Adobe Community post, PDF/A\_3a compliance format supports the feature to attach any file type as an attachment. Please visit the following link for further details on [Convert PDF File to PDF-A][4].

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-DocumentConversion-PDFToPDFA-PDFToPDFA.cs" >}}

## OTF Fonts support

Aspose.Pdf for .NET offers the feature to use Custom/TrueType fonts while creating/manipulating PDF file contents so that file contents are displayed using contents other than default system fonts. Starting this release, we have also provided the support for Open Type Fonts. For further details, please visit How to use OTF fonts.

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-Text-AddText-OTFFont.cs" >}}

## Make FindFont(...) Method Case Insensitive

The **FindFont(..)** method of **Aspose.Pdf.Text.FontRepository** class provides the capabilities to find specific font from system font repository (i.e. C:/Windows/Fonts/). The method is case-sensitive and requires an exact Font file name. In this new release, we have provided an overloaded method public static Font FindFont(string fontName, bool ignoreCase), which takes second argument to specify either the font name should be case-sensitive or not. When using True as the second argument, a case insensitive name can be provided.

```
//Create new document instance
Document pdfDocument = new Document();
// add page to pages collection of PDF file
Aspose.Pdf.Page page = pdfDocument.Pages.Add();
// create TextFragment instnace with sample text
TextFragment fragment = new TextFragment("Sample Text in OTF font");
// find font inside system font directory
fragment.TextState.Font = FontRepository.FindFont("HelveticaNeueLT Pro 45 Lt",true);
// specify to emend font inside PDF file, so that its displayed properly,
// even if specific font is not installed/present over target machine
fragment.TextState.Font.IsEmbedded = true;
// add TextFragment to paragraphs collection of Page instance
page.Paragraphs.Add(fragment);
// save resultant file
pdfDocument.Save("c:/pdftest/OTF_Font_Tes.pdf");
```

## Miscellaneous fixes

As well as the enhancements and features discussed above, there have been specific improvements for PDF to HTML and HTML to PDF conversion features. Among these fixes, the PCL to PDF, SVG to PDF, PDF to Excel, PDF to DOC, PDF to TIFF and TIFF to PDF conversion, conversion of PDF to PDF/A compliant documents, text replacement, rendering PDF files to XPS format are also improved. Please download and try the latest release of [Aspose.PDF for .NET 10.3.0][5].




[1]: https://downloads.aspose.com/pdf/net
[2]: https://products.aspose.com/slides/net
[3]: https://docs.aspose.com/display/pdfnet/Convert+PDF+to+PowerPoint+PPTX
[4]: https://docs.aspose.com/display/pdfnet/Convert+PDF+file+to+other+Formats
[5]: https://downloads.aspose.com/pdf/net




