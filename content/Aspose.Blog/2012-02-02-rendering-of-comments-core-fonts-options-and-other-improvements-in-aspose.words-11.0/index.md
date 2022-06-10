---
title: 'Rendering of Comments, Core Fonts Options, and Other Improvements in Aspose.Words 11.0'
date: Thu, 02 Feb 2012 04:34:55 +0000
draft: false
url: /2012/02/02/rendering-of-comments-core-fonts-options-and-other-improvements-in-aspose.words-11.0/
author: Adam Skelton
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

We have our monthly release of Aspose.Words ready and you can download it from:

*   [Aspose.Words for .NET 11.0][1]
*   [Aspose.Words for Java 11.0][2]

This release contains 74 great new improvements and fixes to Aspose.Words. Here is a look at some of the most notable improvements:

## Comments are now Rendered to Fixed-Page Formats

The new version of Aspose.Words introduces support for rendering of comments in Microsoft Word to fixed-page formats such as PDF. The output is similar to how Microsoft Word renders comments to formats like PDF.

This is only the first version of comment rendering, so there are some limitations which we have detailed below:

*   There’s no automatic coloring and numbering  - all the comments are rendered in red for the time being.
*   Comments are rendered one by one from top to bottom without any special distribution rule applied.
*   Long comments which are too large for the comment bubble are not clipped.

We will be constantly improving this feature with each release so these limitations will eventually be removed.

Here’s an example of the output produced by Aspose.Words. The comments are now properly rendered to PDF. Also, note how the page size is preserved by scaling the document content and comments pane to fit the page size.



{{< figure align=center src="images/PDF-Output-with-Comments.jpg" alt="">}}


## Options to Export PDF using Core Fonts or System Installed Fonts

There were a large number of requests from our customers to find a way to decrease the size of rendered PDF documents. The number one reason for a larger PDF size compared to the PDFs produced by Microsoft was because of Aspose.Words always embedded fonts in the PDF. Microsoft Word by default does not embed core fonts, such as Arial.

The latest version of Aspose.Words introduces new options which allow you to choose how fonts are exported to PDF, either by using standard core PDF fonts or system installed fonts instead of embedding them into the document.

Using either one of these options results in a significant reduction in the file size of PDFs generated using Aspose.Words. Note that these options are mutually exclusive so you should choose only one at a time to use for your particular needs.

### Core Fonts Mode

This option can be set by using **PdfSaveOptions.UseCoreFonts** property. In this mode four of the most popular “True Type” fonts are replaced in the output PDF document with corresponding core “Type 1” fonts. These fonts are:

*   Arial
*   Times New Roman
*   Courier New
*   Symbol

This setting works only for the text in ANSI (Windows-1252) encoding. Writing non-ANSI text to PDF will always require the corresponding font to be embedded.

This option is also useful if you want a greater document portability since PDF viewer provides core fonts on any supported platform. One drawback is that the appearance of core fonts may be different from system fonts.

### System Fonts Mode

This option can be set by using the **PdfSaveOptions.EmbedStandardWindowsFonts** property. When this property is set to false, true type “Arial” and “Times New Roman” fonts are not embedded into PDF so the client viewer is forced to rely upon the fonts which are installed on client operating system. This setting works only for the text in ANSI (Windows-1252) encoding. Writing non-ANSI text to PDF requires the corresponding font to be embedded.

This mode is most useful if you’re looking to view documents on the same platform and you also want to preserve the exact appearance of fonts in the output PDF.

## Compound Lines Rendering

Previous versions of Aspose.Words use standard GDI+ objects for rendering compound (multiline) lines. This worked well when rendering directly to image, but such document formats as PDF and XPS have no explicit support for compound lines. The only way to render such lines types to these formats is to draw them as a set of normal lines.

This technique has been implemented and is now available in the latest version of Aspose.Words.

In Aspose.Words,  line styles of shapes are specified using Shape.Stroke.LineStyle property. Take a look below at how Aspose.Words now properly renders compound lines to PDF.



{{< figure align=center src="images/Compound-Lines-1.jpg" alt="">}}




{{< figure align=center src="images/Compound-Lines-2.jpg" alt="">}}





[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/net




