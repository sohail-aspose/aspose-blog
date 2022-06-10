---
title: 'Compress Files when Embedding in C# with Aspose.PDF for .NET'
date: Fri, 05 Dec 2014 07:04:22 +0000
draft: false
url: /2014/12/05/compress-files-when-embedding-in-pdf-in-csharp/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


We are very much excited to announce the release of [Aspose.Pdf for .NET 9.8.0][1] which provides some new and exciting features. This new release has an optimized API with great new features. Among these new features, the API has also been optimized from a performance perspective and now you get faster, more reliable PDF creation and manipulation features and an output with great fidelity.

## HTML to PDF Supports CSS3

HTML to PDF conversion is one of our most popular features and has been a key improvement area in recent releases. As there are lots of open standards for HTML, we try to support as many new HTML/CSS tags as we can with each new release. Starting with this release, Aspose.Pdf for .NET now also provides support for CSS3.

## Control File Compression when Adding as Embedded Resources

The FileSpecification class provides makes it possible to add attachments to PDF documents. By default, added files are compressed. However, we have introduced changes to the API to allow developers to control files compression (by enabling or disabling it) when adding files as an embedded resource.

## Custom Footnote

A footnote is an ancillary piece of information printed at the bottom of a page. It can also be a note placed at the bottom of a page of a book or manuscript that comments on or cites a reference. Aspose.Pdf for .NET has the capability to render text information inside a PDF document with various formatting options. You might want to to add footnotes. Using this new release, you can use a custom text label for the FootNote instance and even control the formatting of the footnote line. To define style for the footnote line, create a Graph object, define the line style and pass the object to the NoteLineStyle property of the page instance.

To set a custom label for a footnote, please pass any value to the FootNote.Text property of the TextFragment instance. Similarly, Aspose.Pdf for .NET makes it possible to add end notes to PDF files. An end note is a source citation that refers the readers to a specific place at the end of the document where they can find out the source of the information or words quoted.

## Multi-layered PDF File

Layers can be used in PDF documents in many ways. You might have a multilingual file that you want to distribute and have text in each language appear on different layers, with the background design appearing on a separate layer. Or you might create documents with animation that appears on a separate layer. One example could be to add a license agreement to your file, and you don’t want a user to view the content until they agree to the terms of the agreement.

## Replace Text with Hyperlink

Text manipulation is one of the the features that makes Aspose.Pdf for .NET so flexible. It allows developers to add, update, and remove text from PDF file. It also lets you search text inside a PDF file and replace it. During text replacement, you may also specify text formatting (change the text color, font face, size etc). Furthermore, it also provides the capabilities to create links to applications, external documents or pages within the PDF file. So, using both features, you can search for text in a PDF file and replace it with a hyperlink. For further information, please visit Search Text Based on Regex and Replace with Hyperlink.

## Printing pages to Different Paper Trays

Aspose.Pdf for .NET offers the feature to print PDF files using the PdfViewer class that lets you can print to any printer attached to your system as well as a network printer. When printing, you can adjust margin, paper size, page rotation, display the Print dialog, printing to file, set the number of copies, and much more. Recently, we were asked to support the capability to print different pages to different page trays within a printing job. The user must be able to send a document to a printer and be sure that there are no other print jobs in between or pages. The document must be printed as one.

## Create Filled Rectangle

A PDF document may contain graphics elements such as circle, rectangle, line, ellipse etc. When adding a rectangle to a PDF file, you may want to fill it with color. To do so, pass a value from the Aspose.Pdf.Color enumeration to the Rectangle object's GraphInfo.FillColor property. Please take a look at the following code snippet.

```
// Create Document instance
Document doc = new Document();
// Add page to pages collection of PDF file
Page page = doc.Pages.Add();
// Create Graph instance
Aspose.Pdf.Drawing.Graph graph = new Aspose.Pdf.Drawing.Graph(100, 400);
// Add graph object to paragraphs collection of page instance
page.Paragraphs.Add(graph);
// Create Rectangle instance
Aspose.Pdf.Drawing.Rectangle rect = new Aspose.Pdf.Drawing.Rectangle(100, 100, 200, 120);
// Specify fill color for Graph object
rect.GraphInfo.FillColor = Aspose.Pdf.Color.Red;
// Add rectangle object to shapes collection of Graph object
graph.Shapes.Add(rect);
// Save PDF file
doc.Save("c:/pdftest/FilledRectangle.pdf");
```

For more information, please visit Create Filled Rectangle Object.

## Miscellaneous Fixes

As well as the enhancements and features discussed above, there have been numerous fixes related to HTML to PDF conversion, PDF to Excel conversion, XPS to PDF conversion, PDF to TIFF conversion, conversion of PDF to PDF/A compliant documents, text replacement, rendering PDF files to XPS, creating TOCs in PDF files, and printing PDFs with embedded fonts. Please download and try the latest release of [Aspose.Pdf for .NET 9.8.0][2].




[1]: https://products.aspose.com/pdf/net
[2]: https://downloads.aspose.com/pdf/net




