---
title: 'Aspose.Words OOXML import is coming out of Beta soon! Part 1'
date: Mon, 31 Dec 2007 00:46:00 +0000
draft: false
url: /2007/12/31/aspose-words-ooxml-import-is-coming-out-of-beta-soon-part-1/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

As you might already know we are working hard to provide great support for Office Open XML in Aspose.Words.

Here is a bit of timeline:

*   2007-08-22 Aspose.Words for .NET 4.4 with **export** to Microsoft Office 2007 Open XML (DOCX) released.
*   2007-10-13 Aspose.Words for .NET 4.4.1 with **import** of DOCX files **Beta** released.
*   2007-12-27 Aspose.Words for **Java** 2.4 with **export** to DOCX released.

Since the release in October 2007, import of DOCX files is still in Beta, but we are successfully finalizing it. A production release is planned for January 2008.

We have created a detailed [Aspose.Words to OOXML conformance specification][1] and I'm working on an overview document. Here is a sneak peek for you. More to come.

Office Open XML in Aspose.Words

Aspose.Words allows to import and export Office Open XML (OOXML) documents.

_Importing_ a document means loading it into an Aspose.Words Document object. _Exporting_ means saving an Aspose.Words Document object to a file or stream. Aspose.Words supports import and export in a variety of formats. Importing a document in one format, followed by export into another format is a _conversion_.

Aspose.Words can convert a document from any of its import formats to any of its export formats. The supported import formats are DOCX, DOC, RTF, WordprocessingML and HTML. The supported export formats are DOCX, DOC, RTF, WordprocessingML, HTML, PDF and TXT. The total number of possible conversions is 30.

Regarding the OOXML files, you can convert:

*   DOCX to DOC, RTF, WordprocessingML, HTML, PDF and TXT
*   DOC, RTF, WordprocessingML and HTML to DOCX

# OOXML Conformance

In general, you can expect _high quality_ conversions from Aspose.Words, meaning that document content or formatting loss during a conversion will be minimal. However, at times, some content or formatting loss is unavoidable due to a big difference in the import and export formats. For example, it is not possible to precisely convert tabs from DOC to HTML because HTML does not have tab elements.

When the import and export formats are both Microsoft Word formats (e.g DOC, RTF, WordprocessingML or DOCX) formatting loss is minimal because of the high degree of Aspose.Words’ conformance to those formats. Although the degree of Aspose.Words conformance to OOXML is high, not all OOXML features are yet supported. A detailed conformance specification is provided in a separate spreadsheet. The rest of this section provides a brief overview of the level of OOXML support in Aspose.Words.

# Main Document Story

Aspose.Words supports the main document part in OOXML which contains the document body and a background shape. The document body contains block-level elements such as paragraphs and tables.

# Paragraphs and Rich Formatting

The most basic unit of block-level content within an OOXML document is a paragraph. A paragraph can contain inline elements such as runs of text, fields, hyperlinks, shapes etc. All elements have their formatting properties.

Aspose.Words supports the following inline elements:

*   Bookmarks
*   Fields
*   Hyperlinks
*   Runs of text
*   Breaks
*   Comments
*   Endnotes and Footnotes
*   Symbols
*   Shapes

Aspose.Words supports most of the paragraph properties. Some of the important properties are:

*   Absolute positioning
*   Alignment
*   Asian properties
*   Borders
*   Bullets and numbers
*   Indents
*   Outline
*   Page breaks and keeps
*   Paragraph style
*   Right-To-Left text
*   Shading
*   Tabs
*   Text direction

Aspose.Words supports most of the run properties. Some of the important properties are:

*   Borders
*   Character style
*   Complex script properties
*   Font name, size, style
*   Language
*   Right-To-Left text
*   Shading
*   Strike, emboss, etc effects
*   Underline color and type
*   Vertical position and alignment

# Tables

Another type of block-level content in OOXML, a table is a set of paragraphs (and other block-level content) arranged in rows and columns.

A table defines a set of table-wide properties, a grid layout of the table and contains non-zero number of rows. Each row contains non-zero number of cells. A cell can contain block-level content such as paragraphs and nested tables.

Some of the table, row and cell features supported by Aspose.Words are as follows:

*   Absolute positioning
*   Borders
*   Can’t split
*   Cell margins and spacing
*   Fit text
*   Horizontal merge
*   Nested tables
*   No wrapping
*   Preferred width
*   Right-to-left
*   Row height
*   Shading
*   Table grid
*   Text direction
*   Vertical alignment
*   Vertical merge

# Sections

In OOXML, sections group paragraphs and define the pages on which the text will appear. Section properties include page size, orientation, margins, number of text columns and so on.

Aspose.Words supports multiple sections in a document and all section properties defined in OOXML. Some of the notable section properties are:

*   Document grid
*   Gutter
*   Headers and footers linked to previous section
*   Headers and footers of all types
*   Line numbering
*   Page borders, including Border Art
*   Page margins, distance to header and footer
*   Page size and orientation
*   Right-to-left
*   Section break type
*   Text columns equal and custom width
*   Text direction
*   Vertical alignment

# Styles

Within an OOXML file, styles are predefined sets of paragraph, character, list and/or table formatting properties which can be applied to text within the document.

Aspose.Words supports the following style features:

*   Built-in and custom styles
*   Character styles
*   List styles
*   Name and aliases
*   Next paragraph style
*   Paragraph styles
*   Style hierarchy

# Bullets and Numbering

Numbering are Arabic numerals, Roman numerals, bullets, text strings, etc that are used to label paragraphs of text. A numbered paragraph refers to a list instance. A list instance refers to a list definition, which in turn defines the appearance and behavior of a set of numbered paragraphs.

Aspose.Words supports all list features defined in OOXML. Some of the notable features are:

*   Custom label text
*   Indents
*   Label font properties
*   Link between a list and a style
*   List definitions
*   List instances
*   List level overrides
*   Number format
*   Picture bullets
*   Single and multi-level lists




[1]: http://www.aspose.com/Community/Files/51/aspose.words/entry107522.aspx




