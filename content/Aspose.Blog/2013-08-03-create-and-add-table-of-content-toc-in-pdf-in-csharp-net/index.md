---
title: 'Create and Add Table of Content (TOC) in PDF using C#'
date: Sat, 03 Aug 2013 07:52:34 +0000
draft: false
url: /2013/08/03/create-and-add-table-of-content-toc-in-pdf-in-csharp-net/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---

We are very much excited to announce the release of [Aspose.PDF for .NET 8.3.0][1] which comes with a great set of features and enhancements. For quite some time, Aspose.PDF for .NET has provided the capability to generate a table of content when creating a new PDF document as described in [Manipulating List of Contents][2]. However, in this new release, we have introduced the capability to create a table of contents inside an existing PDF document. The Document class in the Aspose.Pdf namespace gives the power to create as well as manipulate existing PDF files, so we added Heading and TocInfo classes to allow creating TOC in existing PDF files. Further details regarding this feature can be found over [Add TOC in existing PDF][3].

## Add TOC in an Existing PDF

Aspose.PDF API allows you to add a table of content either when creating a PDF, or to an existing file. The _ListSection_ class in the Aspose.Pdf.Generator namespace allows you to create a table of contents when creating a PDF from scratch. To add headings, which are elements of the TOC, use the _Aspose.Pdf.Generator.Heading_ class. The following code sample shows how to add TOC in a PDF using C#:

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-Working-Document-AddTOC-AddTOC.cs" >}}

## Loading Font from Stream

When adding text to existing PDF files, we specify the font information for the TextFragment being added. Therefore we can either specify the font location from a file path or reference it from a stream object. The following code snippet shows how to load the font from a Stream object.

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-Text-AddText-LoadingFontFromStream.cs" >}}

## Set Margin for Text Paragraph

When adding text to an existing PDF file using TextFragment, we can specify the obsolete position of the fragment using the Position property of TextFragment.

```
// Load existing PDF files
Document doc = new Document(inFile);
// Get reference of first page of PDF
Page page = (Page)doc.Pages\[1\];
// Create text builder for specific page
TextBuilder builder = new TextBuilder(page);
// Create text paragraph
TextParagraph paragraph = new TextParagraph();
paragraph.Rectangle = new Aspose.Pdf.Rectangle(100, 600, 200, 700);
// Set the margin for paragraph
paragraph.Margin = new Aspose.Pdf.MarginInfo(5, 10, 10, 15);
// Set the wordwrap mode
paragraph.FormattingOptions.WrapMode = TextFormattingOptions.WordWrapMode.DiscretionaryHyphenation;
// Append lines to TextFragment
paragraph.AppendLine("the quick brown fox jumps over the lazy dog");
paragraph.AppendLine("line2");
paragraph.AppendLine("line3");
// Add paragraph
builder.AppendParagraph(paragraph);
// Save the resultant PDF files
doc.Save(outFile);
```

As well as the above features, we have also introduced many enhancements in terms of performance when converting large text files to PDF format, PDF to XPS conversion, PDF to TIFF conversion, HTML to PDF conversion and much more. Please download and evaluate the latest release of [Aspose.PDF for .NET 8.3.0][4].




[1]: https://downloads.aspose.com/pdf/net
[2]: https://docs.aspose.com/display/pdfnet/Manipulate+PDF+Document#ManipulatePDFDocument-WorkingwithTOC
[3]: https://docs.aspose.com/display/pdfnet/Manipulate+PDF+Document#ManipulatePDFDocument-WorkingwithTOC
[4]: https://downloads.aspose.com/pdf/net




