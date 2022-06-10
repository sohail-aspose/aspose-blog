---
title: 'Save Word as Fixed HTML, Detect Shapes with 3D or Shadow Effects using Aspose.Words 13.3.0'
date: Wed, 24 Apr 2013 12:44:41 +0000
draft: false
url: /2013/04/24/new-fixed-html-save-format-detect-shapes-with-3d-or-shadow-effects-plus-many-other-improvements-in-aspose.words-13.3.0/
author: Adam Skelton
summary: ''
tags: ['Convert DOC DOCX to fixed HTML', 'Convert Word to fixed HTML', 'Fixed html format', 'Html high fidelity']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose.words-logo2.jpg" alt="Aspose.Words Logo">}}


This month’s release of Aspose.Words for .NET and Java contains 97 improvements to Aspose.Words, including a new save format for greater fidelity when saving a document as HTML, improvements to the API and more.

You can immediately download our latest Aspose.Words release from the following links:

*   [Aspose.Words for .NET 13.3.0][1]
*   [Aspose.Words for Java 13.3.0][2]

## Introducing the Fixed HTML Save Format

This month’s release contains a brand new save format: **HtmlFixed**. The **HtmlFixed** format provides the ability to render a document to HTML while preserving almost all formatting and structure found in the original input document. This is a great development as traditionally Word to HTML conversion does not yield a result that looks exactly like the original document, this is not caused by any issue with the way Aspose.Words converts Word documents to HTML but is to be expected due to the differences between the two formats. Not all elements in Word documents can be directly represented in an HTML document and thus these elements may be distorted or removed.

This new format improves the output by first rendering the document in memory using the same layout engine which is used to render documents to PDF or image, and then exports absolutely positioned elements to HTML using this information. The result is an HTML document that looks almost identical to the original, with many elements present that cannot normally be exported when saving as regular HTML.

The main difference, as the name implies, is when the container window is resized the text will not reflow and wrap like as with normal flow HTML documents instead the text stays in a fixed position. What is displayed is still regular HTML content so the text can be copied and pasted, and it will also display correctly on mobile devices.

_The input document_



{{< figure align=center src="images/SampleInputDocument.jpg" alt="Sample Input Document">}}


_The same document converted using the regular HTML save format (this can be referred to as_ **HtmlFlow** _to differentiate it from_ **HtmlFixed** _format).  Note if the window is resized then the text is reflowed._

_The output document rendered using the new **HtmlFixed** format. The output looks more accurate. The text in this output is fixed and does not reflow if the window is resized._



{{< figure align=center src="images/HtmlFixedOutput.jpg" alt="The output produced by Aspose.Words using Html Fixed format">}}


## Detect 3D and Shadow on Drawing Objects

Use the newly added **ExtrusionEnabled** and **ShadowEnabled** properties on **Shape** class to detect whether a shape is formatted as 3D (extrusion) or with a shadow.

## Improved Outline Options when Rendering to Fixed Page Documents

Several fixed paged formats display headings and bookmarks in a tree-based display for easy access, for example, the navigation panel found with most PDF viewers.

In this release the API to work with outline levels has been improved, an introduction of the standard **OutlineOptions** class replaces the individual members which were previously used to set outline levels for each **SaveOptions** class. In addition to this, through the use of the new **BookmarksOutlineLevelCollection** class, you can now set the outline level of individual bookmarks.




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java




