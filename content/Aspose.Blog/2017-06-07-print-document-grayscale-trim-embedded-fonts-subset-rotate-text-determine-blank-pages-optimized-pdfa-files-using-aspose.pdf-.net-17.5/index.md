---
title: 'Print PDF Document in Grayscale and Optimized PDF/A using C#'
date: Wed, 07 Jun 2017 20:41:47 +0000
draft: false
url: /2017/06/07/print-document-grayscale-trim-embedded-fonts-subset-rotate-text-determine-blank-pages-optimized-pdfa-files-using-aspose.pdf-.net-17.5/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-net.jpg" alt="">}}


The new release of Aspose.PDF for .NET 17.5 has been published with exciting new features, some minor enhancements and fixes related to bugs reported in earlier release versions. In every new release, we try our best to publish a better, stable and exciting release which can facilitate our customers and help them to accomplish great features in less amount of time. The ease of use and rich support contents including product support documentation are among the salient features of our API's and we always strive to enrich the programmers guide with detailed articles explaining steps to use new and existing features of APIs. This new release version also contains some promising features which were recently requested by our customers.

## Print a PDF Document as Grayscale into C#

PdfViewer class in Aspose.Pdf.Facades offers the feature to print the PDF documents. We can print the file to default attached printer or any other printer already configured with the system and during file printing, the API prints the file in default colors. However we recently received a requirement to print the file in Grayscale and in order to accomplish this requirement, we have introduced **PrintAsGrayscale** property in **PdfViewer** class. The following code snippet can be used to print the file in Grayscale.

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-Working-Document-ConvertFromRGBToGrayscale-ConvertFromRGBToGrayscale.cs" >}}

Another option can be to [Convert a PDF from RGB colorspace to Grayscale][1] and simply call PDF printing routine.

## Trim Fully Embed Fonts to Subsets Only

Aspose.Pdf for .NET provides the capabilities of [Working with Text elements][2]. Some of the salient features include [Addition Text to PDF file][3], [Extraction of Text from PDF file][4], [Searching and getting Text from PDF file][5] and [Replacement of Text inside the PDF document][6]. During PDF file creation, we can specify a custom font to be used inside the document and this feature can be accomplished while using **TextState.Font** property of **TextFragment** object which takes **FontRepository.FindFont("TimesNewRoman");** object as an argument. The font name which we want to use during PDF creation can be provided as an argument to **FindFont(...)** method. When using custom font inside PDF file, we need to either Embed it or add it's subset so that when viewing the document on a system which do not have the font used inside PDF document, the layout is not disturbed. In order to embed the font inside PDF document, we need to set the value of **TextFragment.TextState.Font.IsEmbedded** property as **True** and in order to add subset of custom font inside PDF file, we need to set the value of **TextFragment.TextState.Font.IsSubset** to **True**.

However please note that when we add the font as Embedded resource inside PDF file, the complete font is included in the document and the size of the document may become larger. However when using a Subset of font, only the glyph of the font used inside the document is embedded, rather than a complete font.

Aspose.Pdf for .NET provides a variety of features to deal with fonts in PDF document. Some of the salient features include

*   [Embedding Fonts while creating PDF][7]
*   [Embedding Fonts in an existing PDF file][8]
*   [Replace fonts in existing PDF file][9]
*   [Remove Unused Fonts from PDF File][10]

If we open any PDF document in Adobe Acrobat/Reader, and check PDF file properties using File -> Properties menu option, when we click on the "Fonts" tab, we can see fonts that have been embedded inside the document. Some may be fully embedded ("Embedded") and others may be partially embedded ("Embedded Subset"). Apart from the above-mentioned capabilities, we may come across a requirement to take fully embedded font sets and trim them down to subsets only.

Currently, Aspose.Pdf for .NET controls font subsetting declared in interface Document.IDocumentFontUtilities. Every object of type Aspose.Pdf.Document has property FontUtilities of type IDocumentFontUtilities. This interface includes method SubsetFonts(FontSubsetStrategy subsetStrategy). The Parameter subsetStrategy helps to tune subset strategy and currently, two variants of font subsetting are supported. At the moment, it is possible to subset all fonts used by document(strategy SubsetAllFonts) or to subset only fully embedded fonts(or font subsets which are larger than is required by current document).

*   **SubsetAllFonts** - All the fonts will be embedded into document as font subset is embedded into PDF document by definition
*   **SubsetEmbeddedFontsOnly** - This process will not affect fonts which are not embedded into document.

The following code snippet can be used to reduce fully embedded font sets to only those subsets that are used:

```
Document doc = new Document(dataDir + "input.pdf");
// All fonts will be embedded as subset into document in case of SubsetAllFonts.
doc.FontUtilities.SubsetFonts(Document.FontSubsetStrategy.SubsetAllFonts);
// Font subset will be embedded for fully embedded fonts but fonts which are not embedded into document will not be affected.
doc.FontUtilities.SubsetFonts(Document.FontSubsetStrategy.SubsetEmbeddedFontsOnly);
doc.Save(dataDir + "Output_out.pdf"); 
```

## Rotation of Text in PDF

We can add a text inside PDF file using TextFragment or TextBuilder objects. When using TextBuilder, we simply need to add TextFragments to TextBuilder object using AppendText(..) method and we do not need to exclusively add TextBuilder object to Paragraphs collection of page instance. However, when only using the TextFragment object, we need to add it to paragraphs collection of Page instance. Recently we received a requirement to rotate the text inside PDF document. In order to accomplish this requirement, we have added a Rotation property to TextParagraph and TextFragments objects. It expects value of rotation angle specified in degrees and will work in PDF document generation scenarios.  
Specified below is the code snippet to rotate text when using TextFragment and TextBuilder objects.

```
//open document
Document pdfDocument = new Document();
//get particular page
Page pdfPage = (Page)pdfDocument.Pages.Add();

//create text fragment
TextFragment textFragment1 = new TextFragment("main text");
textFragment1.Position = new Position(100, 600);

//set text properties
textFragment1.TextState.FontSize = 12;
textFragment1.TextState.Font = FontRepository.FindFont("TimesNewRoman");

//create rotated text fragment
TextFragment textFragment2 = new TextFragment("rotated text");
textFragment2.Position = new Position(200, 600);

//set text properties
textFragment2.TextState.FontSize = 12;
textFragment2.TextState.Font = FontRepository.FindFont("TimesNewRoman");
textFragment2.TextState.Rotation = 45;

//create rotated text fragment
TextFragment textFragment3 = new TextFragment("rotated text");
textFragment3.Position = new Position(300, 600);

//set text properties
textFragment3.TextState.FontSize = 12;
textFragment3.TextState.Font = FontRepository.FindFont("TimesNewRoman");
textFragment3.TextState.Rotation = 90;

// create TextBuilder object
TextBuilder textBuilder = new TextBuilder(pdfPage);
// append the text fragment to the PDF page
textBuilder.AppendText(textFragment1);
textBuilder.AppendText(textFragment2);
textBuilder.AppendText(textFragment3);
//save document
pdfDocument.Save("TextFragmentTests_Rotated1.pdf"); 
```

For further details on supporting same feature with various approaches, please visit [Rotate Text Inside PDF][11]

## Detect Blank Pages in PDF

There are scenarios where PDF documents may contain blank pages and customers may have a requirement to determine the blank pages inside the document. One of the approaches is to iterate through each page of the document, identify any images and determine if the images have a white color or different colors, try parsing text content and determine the length of extracted text and every-time we need to write the complete code snippet. However, we have introduced a build-in feature in API to accomplish this requirement. The IsBlank(..) method of Page object can be used to fulfill this requirement where it takes an argument for the threshold level.

```
string inputFileName = @"c:\sample.pdf";
// load existing PDF file
Document pdfDocument = new Document(inputFileName);
// determine if first page fo document is blank where we can define the threshold level
bool isBlank = pdfDocument.Pages[1].IsBlank(0.01d);
// determine if second page is blank or not
isBlank = pdfDocument.Pages[2].IsBlank(0.01d); 
```

## Miscellaneous Fixes

Apart from the above-mentioned improvements, the PDF to Image conversion, Text extraction, Text replacement, PDF to Image conversion, PDF file signing, PDF to HTML, Rotation of table object, PDF form filling, PDF file merge and import of Annotations are also improvement areas. Its always recommended to use the latest release of our API's, so we suggest you to please download the latest release of [Aspose.PDF for .NET 17.5][12] and check [Release Notes][13] section for list of issues fixed in Aspose.Pdf for .NET 17.5

*   [Home page for Aspose.Pdf for .NET][14]
*   [Download Aspose.Pdf for .NET][15]
*   [Aspose.Pdf product family forum][16]– Post your technical questions and queries, or any other problem you faced while running Aspose.Pdf APIs.
*   [Aspose.Pdf for .NET online documentation][17]– help documentation and API reference documents.
*   [Enable Blog Subscription][18]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Pdf APIs, new features, fixes and other API related topics by subscribing to Aspose.Pdf blog.
*   [Aspose.Pdf for .NET Examples][19] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://docs.aspose.com/display/pdfnet/Optimize+PDF+Document#OptimizePDFDocument-ConvertaPDFfromRGBcolorspacetoGrayscale
[2]: https://docs.aspose.com/display/pdfnet/Working+with+Text
[3]: https://docs.aspose.com/display/pdfnet/Add+Text+to+a+PDF+file
[4]: https://docs.aspose.com/display/pdfnet/Extract+Text+from+PDF
[5]: https://docs.aspose.com/display/pdfnet/Search+and+Get+Text+from+Pages+of+a+PDF+Document
[6]: https://docs.aspose.com/display/pdfnet/Replace+Text+in+a+PDF+Document
[7]: https://docs.aspose.com/display/pdfnet/Formatting+PDF+Document#FormattingPDFDocument-EmbeddingFontswhilecreatingPDF
[8]: https://docs.aspose.com/display/pdfnet/Formatting+PDF+Document#FormattingPDFDocument-EmbeddingFontsinanexistingPDFfile
[9]: https://docs.aspose.com/display/pdfnet/Replace+Text+in+a+PDF+Document#ReplaceTextinaPDFDocument-ReplacefontsinexistingPDFfile
[10]: https://docs.aspose.com/display/pdfnet/Replace+Text+in+a+PDF+Document#ReplaceTextinaPDFDocument-RemoveUnusedFontsfromPDFFile
[11]: https://docs.aspose.com/display/pdfnet/Rotate+Text+Inside+PDF
[12]: https://downloads.aspose.com/pdf/net/new-releases/aspose.pdf-for-.net-17.5/
[13]: https://docs.aspose.com/display/pdfnet/Aspose.Pdf+for+.NET+17.5+Release+Notes
[14]: https://www.aspose.com/products/pdf/net
[15]: https://downloads.aspose.com/pdf/net
[16]: https://forums.aspose.com/c/pdf
[17]: https://docs.aspose.com/display/pdfnet/Home
[18]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/
[19]: https://github.com/aspose-pdf/Aspose.Pdf-for-.NET




