---
title: 'Convert PDF to PDF/A_3 (3a and 3b) using C# with Aspose.PDF for .NET 10.6.0'
date: Thu, 06 Aug 2015 14:07:23 +0000
draft: false
url: /2015/08/06/convert-pdf-to-pdfa_3-and-convert-pdf-from-rgb-to-grayscale-using-csharp-asp.net/
author: Codewarior
summary: ''
tags: ['Convert PDF from RGB to Grayscale', 'Convert PDF to PDF/A_3']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


Empowering the API with new rich features and enhancements, a new release of [Aspose.PDF for .NET 10.6.0][1] has been published. This version contains some amazing new features which enrich the API to create stunning applications with a vast variety of PDF creation as well as manipulation features. Astonish your customers through your applications by providing stunningly amazing features for PDF file creation/manipulation and surprise them with resultant files with great fidelity.

## Convert PDF to PDF/A-3 with Compliance-Level (3a, 3b)

[PDF to PDF/A conversion][2] and [PDF/A compliance validation][3] features have been supported by our API for quite some time and from time to time, we introduce modifications so that new enhancements are provided in these functionalities. The following code sample shows how to convert PDF files to PDF/A\_3b compliant format using C#.

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-DocumentConversion-PDFToPDFA3b-PDFToPDFA3b.cs" >}}

## Convert a PDF from RGB Colorspace to Grayscale

We received a requirement to convert a PDF from RGB colorspace to Grayscale so that it would be faster while printing those PDF files. Also when the file is converted to GrayScale, the size of the document is also reduced but with this change, the quality of the document may drop. Currently, this feature is supported by the Pre-Flight feature of Adobe Acrobat, but when talking about Office automation, Aspose.PDF is the ultimate solution to provide such leverages for document manipulation. In order to accomplish this requirement, the following code snippet can be used.

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-Working-Document-ConvertFromRGBToGrayscale-ConvertFromRGBToGrayscale.cs" >}}

## Manipulate Tables in Existing PDF Document

One of the earliest features supported by Aspose.PDF for .NET is its capabilities of [Working with Tables][4] and it provides great support for adding tables in PDF files being generated from scratch or any existing PDF files. You also get the capability to [Integrate Table with Database (DOM)][5] to create dynamic tables based on database contents. In this new release, we have implemented a new feature of searching and parsing simple tables that already exist on the page of PDF document. A new class named Aspose.Pdf.Text.TableAbsorber provides these capabilities. The usage of TableAbsorber is very much similar to the existing TextFragmentAbsorber class. The following code snippet shows the steps to update contents in a particular table cell.

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-Tables-ManipulateTable-ManipulateTable.cs" >}}

Features related to this functionality which still need implementation.

*   One of the customers has requested to fetch the data based on the blocks of table or borders (as given in the diagram) and colors as well. Currently, TableAbsorber cannot recognize the table cell background color now. However, we expect to make this improvement in this future and a separate ticket PDFNEWNET-38997 is already created in our issue tracking system.
*   Another customer wants to get the contents of the column in the table. Currently, TableAbsorber cannot recognize tables without borders, but conversion to XLS works well in such cases. However, conversion to XLS is a workaround. However, we created a ticket PDFNEWNET-38998 to improve TableAbsorber for working with such table types.
*   The customer wants to update table in the existing PDF dynamically. Including deleting / insertion of rows. This request is a bit difficult to implement and the current implementation of TableAbsorber cannot fulfill such requirements. However, in order to cater to such requirements, we have created a ticket PDFNEWNET-38999 to investigate the request.
*   If you have a requirement of looking for text property in Aspose.Pdf.Cells or BaseParagraph types, (such types are designed for adding new contents on the page), you must cast BaseParagraph to one of the inherited types. For example, next code must help: `foreach (Row r in table.Rows) { TextFragment fragment = r.Cells[1].Paragraphs[1] as TextFragment; string text; if (fragment != null) text = fragment.Text; }`

## XML to PDF: Working with individual objects in a new generator

The XmlLoadOptions class provides the feature to load the XML document and parse it to PDF format. However recently we received a requirement to work with individual objects (as supported in legacy Aspose.Pdf.Generator) when using this approach.

```
Document doc = new Document();
doc.BindXml(inXml);
doc.Pages[1].Paragraphs[0].IsInNewPage = true;
```

## Clear() Method in PageCollection

When using legacy Aspsoe.Pdf.Generator approach, we get the option to create a separate list which can be used to save the pages already created. After creating multiple pages, we usually clear the PDF and then again add the pages from own list. Therefore in order to introduce the same capabilities in the new Document Object Model, the following code snippet can be used.

```
string outFile = "38613.pdf";
Document doc = new Document();
Page page = doc.Pages.Add();
page.Paragraphs.Add(new TextFragment("text"));
page.Paragraphs.Add(new TextFragment("text1"));
doc.Pages.Clear();
Assert.IsTrue(doc.Pages.Count == 0);
doc.Pages.Add(page);
Assert.IsTrue(doc.Pages.Count == 1);
doc.Save(outFile);
```

## Miscellaneous Fixes

As well as the enhancements and features discussed above, there has been a specific improvement for PDF to HTML and HTML to PDF conversion features with better support for HTML5. Among these fixes, the PCL to PDF, SVG to PDF, PDF to Excel, PDF to DOC, PDF to TIFF and TIFF to PDF conversion, conversion of PDF to PDF/A compliant documents, text replacement, Filling of the signature field with an image, flattening of PDF and rendering of PDF to XPS format, FloatingBox rendering, FootNote, EndNote and rendering of non-English (specifically Arabic) contents are also improved. Please download and try the latest release of [Aspose.PDF for .NET 10.6.0][6].




[1]: https://downloads.aspose.com/pdf/net
[2]: https://docs.aspose.com/display/pdfnet/Convert+PDF+file+to+other+Formats
[3]: https://docs.aspose.com/display/pdfnet/Manipulate+PDF+Document#ManipulatePDFDocument-ValidatePDFDocumentforPDFAStandard(A1AandA1B)
[4]: https://docs.aspose.com/display/pdfnet/Working+with+Tables
[5]: https://docs.aspose.com/display/pdfnet/Manipulate+and+Integrate+Table
[6]: https://downloads.aspose.com/pdf/net




