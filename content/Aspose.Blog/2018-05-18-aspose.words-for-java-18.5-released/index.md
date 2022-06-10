---
title: 'LINQ Reporting Engine Supports Null-Conditional Operators in Template Expressions in Aspose.Words for Java 18.5'
date: Fri, 18 May 2018 08:49:41 +0000
draft: false
url: /2018/05/18/aspose.words-for-java-18.5-released/
author: Awais Hafeez
summary: ''
tags: ['LINQ Reporting Engine', 'Use NULL conditional operator in template expression']
categories: ['Aspose.Words Product Family']
---

We are pleased to announce the new monthly release of [**Aspose.Words for Java 18.5**][1]. The release of this month contains a number of new features, enhancements and bug fixes of the issues reported by our users in previous versions. Please check the detailed [release notes of Aspose.Words for Java 18.5][2] to get an idea about all the new features/enhancements and fixes made in this release. Furthermore, if you are planning to upgrade the API from any previous version, we strongly recommend you to check the Public API Changes section of current release and other intermediate releases from release notes folder, to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## Supported Null-Conditional Operators in Template Expressions for LINQ Reporting Engine

We have added new feature in LINQ Reporting Engine to support null-conditional (A?.B) and null-coalescing (A ?? B) operators. Please read the following article for more detail.

[Using Operators][3]

## Change Content Control Background and Border Colors

We have added StructuredDocumentTag.Color property in this version of Aspose.Words for Java. This property gets or sets the color of the structured document tag. Please read the following article for more detail.  
Change Content Control Background and Border Colors  

## Obsolete Property HtmlSaveOptions.ExportMetafileAsRaster Removed

We have removed obsolete property ExportMetafileAsRaster from the HtmlSaveOptions class in Aspose.Words 18.5. Please use the HtmlSaveOptions.MetafileFormat property instead.

## Other Improvements

There are 75 improvements and fixes in this regular monthly release. The most notable are:

*   Added public property StructuredDocumentTag.Color 
*   Improved logic to detect the encoding of a short TXT file.
*   Fixed line wrapping with trailing spaces at the end
*   Fixed issue with paragraph after spacing in headers/footers
*   Fixed issue with table width when widthAfter is specified for a jagged table
*   Fixed issue with table width with complex column layout and default widths
*   Fixed breaking of floating table row in compatibility mode
*   Fixed issue with floating frame pushed from the page because of invalid wrap point
*   Implemented support for "distribute space" and "distribute letter" types of alignment when rendering Ruby objects
*   Improved rendering of a Doughnut DrawingML Chart with multiple series
*   Improved rendering of DrawingML Charts data labels with the direct layout and a layout specified in the extension properties
*   Fixed a problem with metafile rendering when glyph offsets were wrongly read for EMF\_EXTTEXTOUT record with glyph indices
*   Fixed a problem with the processing of control character (U+0019) in the text when rendering
*   Fixed a problem with Adobe “Fast Find” function (words searching) in rendered PDF documents
*   Fixed a bug with inaccurate processing of EMR\_ALPHABLEND record while rendering metafiles. This bug caused a loss of fill in some figures
*   Fixed a bug with rendering of PieChart data label separator when it is set directly
*   Fixed rendering of dashed line shapes with a shadow
*   LINQ Reporting Engine supports **?.** and **?\[\]** null-conditional operators in template expressions

## Aspose.Words for Java Resources

The following resources will help you work with Aspose.Words for Java:

*   [Home page for Aspose.Words for Java][4]
*   [Install Aspose.Words for Java from Maven][5]
*   Words product family forum – Post your technical questions and queries, or any other problem you faced while running Aspose.Words APIs.
    *   [Free Support Forum][6]
    *   [Paid Support Forum][7]
*   [Aspose.Words for Java online documentation][8]– Help documentation.
*   [Aspose.Words for Java online API reference][9]– API reference documents.
*   [Enable Blog Subscription][10]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words, APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
*   [Aspose.Words for Java Examples][11] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[2]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+18.5+Release+Notes
[3]: https://docs.aspose.com/display/wordsjava/Using+Operators
[4]: https://products.aspose.com/words/java
[5]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[6]: https://forum.aspose.com/c/words
[7]: https://helpdesk.aspose.com/
[8]: https://docs.aspose.com/display/wordsjava/Home
[9]: https://apireference.aspose.com/java/words
[10]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[11]: https://github.com/aspose-words/Aspose.Words-for-Java




