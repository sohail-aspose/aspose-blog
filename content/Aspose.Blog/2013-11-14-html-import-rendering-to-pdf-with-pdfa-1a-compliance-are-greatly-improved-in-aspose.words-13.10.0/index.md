---
title: 'HTML Import and Rendering to PDF with PDF/A-1a Compliance using Aspose.Words 13.10.0'
date: Thu, 14 Nov 2013 10:37:28 +0000
draft: false
url: /2013/11/14/html-import-rendering-to-pdf-with-pdfa-1a-compliance-are-greatly-improved-in-aspose.words-13.10.0/
author: Adam Skelton
summary: ''
tags: ['CSS Cascade', 'CSS margins support', 'HTML engine', 'HTML export', 'HTML import', 'PDF/A-1a', 'PDF/A-1b', 'Support for table styles', 'conversion to PDF', 'convert document to PDF', 'import of HTML based formats', 'improved CSS Cascading', 'render documents to PDF', 'rendering to PDF with PDF/A-1a compliance', 'working with HTML based documents']
categories: ['Aspose.Words Product Family']
---

Aspose.Words 13.10.0 has been released and we are very pleased to announce that this month’s release contains nearly 200 useful improvements and features including the long-awaited rework of the HTML import/export engine.

You can download the latest release of Aspose.Words from the following links:

*   [Aspose.Words for .NET 13.10.0][1]
*   [Aspose.Words for Java 13.10.0][2]
*   [Aspose.Words for Android 1.3][3] (this version matches the Aspose.Words for Java 13.10.0 codebase)

Here is a look at just a few of the biggest features in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

## Reworked HTML Engine - Richer Support for CSS Cascading and Inheritance during HTML Import

We have just integrated an overhaul of our existing HTML engine which adds better support for CSS features and improves overall performance when working with HTML based documents. As you may know, HTML documents differs greatly from traditional Word documents so it takes a detailed underlying engine to convert between the two formats with high fidelity, and while our old engine dealt well with many HTML documents there was room for improvement.

This new engine is the result of many months of work by our developers and we know you will enjoy the results that it brings.  This is also good news to many customers as this rework closes many open issues that customers have faced with the old HTML engine.

This new engine not only brings great efficiency but also supports many new HTML features during import, such as:

*   **Proper inheritance of attributes from parent nodes**, for example, a style applied to a row or cell tag in an HTML document is correctly applied to the text within the cell when imported into the Aspose.Words Document Object Model. In previous versions, this feature was missing and therefore the formatting of the imported text was incorrect.
*   **Support for table styles** (style attribute of table element) during import of HTML based formats.
*   **Quirks and Standards modes** which support leads to greater fidelity when working with HTML documents without a document type declared.
*   **Improved support for CSS margins** for improved document layout when working with the spacing of content.
*   Many other new features and improvements.

For further details on the HTML features supported during import and export for all formats including HTML, take a look at our Supported Features section in the documentation.

## Render to PDF with PDF/A-1a Compliance

Aspose.Words now support rendering documents to PDF with PDF/A-1a compliance level. This compliance encompasses all of the requirements of PDF/A-1b which Aspose.Words already support and ensures the document can be searched and repurposed.

With this compliance document features are also exported to the logical structure contained in the document. Aspose.Words includes the following features from the source document in the logical structure:

*   Paragraphs, including paragraphs spanned over several pages.
*   Lists, including lists spanned over several pages.
*   Tables. Spanned tables are not supported.
*   Header/footer.
*   DML/VML shapes and OfficeMath.
*   Footnotes/endnotes.
*   Comments.
*   Text language

Check out our documentation which demonstrates [How to Convert any supported document to PDF][4] with just two lines of code. To define the compliance type and many other options when converting to PDF check out the PdfSaveOptions class.




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java
[3]: https://downloads.aspose.com/words/androidjava
[4]: https://docs.aspose.com/display/wordsnet/Converting+a+Document




