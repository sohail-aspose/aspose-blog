---
title: 'Export Word Document (DOC/DOCX) Headers Footers to Plain TXT File'
date: Mon, 12 Nov 2018 08:03:47 +0000
draft: false
url: /2018/11/12/convert-header-footer-txt/
author: Awais Hafeez
summary: ''
tags: ['Export headers and footers in Word to TXT', 'headers and footers']
categories: ['Aspose.Words Product Family']
---

## 



{{< figure align=center src="images/aspose-Words-for-Java.png" alt="Aspose.Words for Java">}}


We are pleased to announce the new monthly release of [**Aspose.Words for Java 18.11**][1]. The release of this month contains number of new features, enhancements and bug fixes of the issues reported by our users in previous versions. Please check the detailed [release notes of Aspose.Words for Java 18.11][2] to get an idea about all the new features/enhancements and fixes made in this release. Furthermore, if you are planning to upgrade the API from any previous version, we strongly recommend you to check the Public API Changes section of current release and other intermediate releases from release notes folder, to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## Export Headers Footers to Plain Text TXT File

A new feature has been added in Aspose.Words 18.11 to export all headers and footers at the end of document. We have added new property TxtSaveOptions.ExportHeadersFootersMode in this version of Aspose.Words. The main advantage of a new property over the old TxtSaveOptions.ExportHeadersFooters property is that it has new headers and footers export mode: 'AllAtEnd'. In this mode Aspose.Words act the way similar to MS Word; all headers and footers are placed after all section bodies at the very end of a document. Please read the following article:

[Export Header and Footer in Output TXT Format][3]

## Other Improvements

There are 81 improvements and fixes in this regular monthly release. The most notable are:

*   **Aspose.Words for Java release jar is tested on Java 11**.
*   Compatibility with GroupDocs Total License is improved.
*   GraphicsQualityOptions is better mapped to Java.
*   We did yet another step to shrink (already small) pixel difference between .Net and Java generated images, borders, etc.
*   **JavaDoc for obsolete members become more clear**.
*   Fixed hang with autosized tables when cell has right aligned floaters.
*   Fixed wrong visual order of text in specific cases.
*   Fixed non-breaking space widths calculation.
*   Implemented support for floating table metrics when calculating grid.
*   ROP (raster operations) emulation code was improved, resulting in a significant performance boost (up to 5 times) when rendering the corresponding metafiles.
*   Improved legacy vertical writing support in EMF rendering. Fonts with the '@' prefix additionally rotate the Japanese glyphs.
*   Improved calculation of the shape boundaries, more accurately mimicking the MS Word output.
*   Improved the rendering of DrawingML charts canvases overlay. Markers of the “nofill” series are rendered on the foreground.
*   Improved rendering of DrawingML chart axes for documents created using MS Word 2007.
*   Fixed a bug with incorrect resolution of the system “window” color when rendering of VML shapes.
*   Fixed an issue with underline/strikeout text effects in EMF/WMF rendering.
*   Fixed a document rendering issue when font with English name could not be found in the system with a different locale.
*   Fixed bug with rendering of DrawingML chart markers, if series data are not sorted in ascending order.
*   Fixed a bug causing shifts of rotated shapes in DrawingML chart while rendering.
*   Provided TxtSaveOptions.ExportHeadersFootersMode property.

The following resources will help you work with Aspose.Words for Java:

*   [Home page for Aspose.Words for Java][4][](https://downloads.aspose.com/words/java)
*   [Install Aspose.Words for Java from Maven][5]
*   Words product family forum – Post your technical questions and queries, or any other problem you faced while running Aspose.Words APIs.
    *   [Free Support Forum][6]
    *   [Paid Support Forum][7]
*   [Aspose.Words for Java online documentation][8]– Help documentation.
*   [Aspose.Words for Java online API reference][9]– API reference documents.
*   [Enable Blog Subscription][10]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words, APIs, new features, fixes, and other API related topics by subscribing to Aspose.Words blog.
*   [Aspose.Words for Java Examples][11] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[2]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+18.11+Release+Notes
[3]: https://docs.aspose.com/display/wordsjava/Working+with+Text+Document#WorkingwithTextDocument-ExportHeaderandFooterinOutputTXTFile
[4]: https://products.aspose.com/words/java
[5]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[6]: https://forum.aspose.com/c/words
[7]: https://helpdesk.aspose.com/
[8]: https://docs.aspose.com/display/wordsjava/Home
[9]: https://apireference.aspose.com/java/words
[10]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[11]: https://github.com/aspose-words/Aspose.Words-for-Java




