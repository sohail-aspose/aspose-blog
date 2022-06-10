---
title: 'Hyphenation API Extended, FitText Attribute for Flow Formats, OOXML (Microsoft Word 2010) Text Effects Rendering and More in Aspose.Words 14.5.0'
date: Tue, 03 Jun 2014 14:01:45 +0000
draft: false
url: /2014/06/03/hyphenation-api-extended-support-of-fittext-attribute-in-flow-formats-ooxml-ms-word-2010-text-effects-rendering-performance-and-other-improvements-in-aspose.words-14.5.0/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Total Product Family']
---

Aspose.Words 14.5.0 has been released. This month’s release contains over 95 useful new features, enhancements and bug fixes.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 14.5.0][1]
*   [Aspose.Words for Java 14.5.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

*   Performance improvements.
*   Improved justification around inline paragraph breaks.
*   Hyphenation API updated and extended with a callback mechanism.
*   Table row wrapping around floaters in compatibility mode improved.
*   OOXML (Microsoft Word 2010) text effects rendering implemented.
*   Image export to HTML, MHTML and EPUB improved.
*   FitText attribute supported for all flow formats.

## Hyphenation API Extended

Hyphenation API logic has been changed in the following way:

1.  When a dictionary is registered, it is loaded instantly and if there is an error, an exception is thrown. In the previous version dictionary registration was delayed until its first use which could throw errors when building the page layout.
2.  A callback has been added which allows delayed loading of dictionaries.
3.  The API now supports loading a hyphenation dictionary from a stream.

## SaveOptions.UseAntiAliasing Supported for Raster Images when Exporting Document to HTML

When the document is exported to the HTML, MHTML and EPUB formats, the SaveOptions.UseAntiAliasing option is used for raster images.




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/category1188.aspx
[2]: http://www.aspose.com/community/files/72/java-components/aspose.words-for-java/category1378.aspx




