---
title: 'Aspose.Words Supports Conditional Blocks in LINQ Reporting Engine'
date: Tue, 09 Jun 2015 11:53:50 +0000
draft: false
url: /2015/06/09/use-conditional-blocks-in-linq-reporting-engine-with-aspose.words-for-.net/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Aspose.Words 15.5.0 has been released. This month’s release contains over 87 useful new features, enhancements and bug fixes to the Aspose.Words products.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 15.5.0][1]
*   [Aspose.Words for Java 15.5.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

*   CustomXML nodes are removed
*   Support for conditional blocks added to the LINQ Reporting Engine
*   Improved rendering of floating shapes in complex tables
*   Implemented Arabic Abjad list numbering style in the layout
*   Improved performance of importing HTML documents with complex CSS selectors
*   Improved positioning of floating shapes in HTML output
*   A document can now be rendered in a grayscale mode
*   Improved Far-Eastern characters rendering for PDF embedded fonts
*   Significantly improved time and size when rendering PDF documents with DrawingML text effects

## PageSetup.TextOrientation Public Property Added

We have added new public property TextOrientation to PageSetup class:

```
/// <summary>
/// Allows to specify <see cref="TextOrientation"/> for the whole page.
/// Default value is <see cref="Aspose.Words.TextOrientation.Horizontal"/>
/// </summary>
public TextOrientation TextOrientation
```

It allows specifying TextOrientation for the whole page. The default value is Horizontal. This property is only supported for MS Word native formats such as DOCX, WML, RTF, and DOC.

## SaveOptions.ColorMode Public Property Added

We have added new public property ColorMode to SaveOptions class. While rendering to fixed page formats such as PDF, XPS, and images, the documents can be rendered in two color modes now

*   ColorMode.Normal - an ordinary way with unmodified colors and
*   ColorMode.Grayscale - with colors in a range of gray shades from white to black.

```
///
/// Gets or sets a value determining how colors are rendered.
/// 
/// The default value is 
/// This property is used when the document is exported to fixed page formats.
/// 
public ColorMode ColorMode { get; set; }
```

Sample code is as follows:

```
Document doc = new Document(MyDir + "in.docx");
PdfSaveOptions options = new PdfSaveOptions();
// Save the document "doc" in grayscale mode PDF.
options.ColorMode = ColorMode.Grayscale;
doc.Save(MyDir + "out.pdf", options);
```

## Conditional Blocks for LINQ Reporting Engine Supported

The new functionality of conditional blocks is described in the following sections of the documentation:

*   Using Conditional Blocks
*   [Working with Table-Row Conditional Blocks][3]
*   [Multicolored Numbered List Template (Appendix C)][4]
*   [In-Table List Template with Highlighted Rows (Appendix C)][5]
*   [In-Table List Template with Alternate Content (Appendix C)][6]




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java
[3]: https://docs.aspose.com/display/wordsnet/Template+Syntax#TemplateSyntax-WorkingwithTable-RowConditionalBlocks
[4]: http://docs.aspose.com/display/wordsnet/Appendix+C.+Typical+Templates#AppendixC.TypicalTemplates-MulticoloredNumberedListTemplate
[5]: http://docs.aspose.com/display/wordsnet/Appendix+C.+Typical+Templates#AppendixC.TypicalTemplates-InTableListTemplatewithHighlightedRows
[6]: http://docs.aspose.com/display/wordsnet/Appendix+C.+Typical+Templates#AppendixC.TypicalTemplates-InTableListTemplatewithAlternateContent




