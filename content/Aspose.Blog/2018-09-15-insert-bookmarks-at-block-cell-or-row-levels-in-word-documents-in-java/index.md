---
title: 'Bookmarks at Block, Cell or Row Levels in Word Documents in Java'
date: Sat, 15 Sep 2018 09:03:37 +0000
draft: false
url: /2018/09/15/insert-bookmarks-at-block-cell-or-row-levels-in-word-documents-in-java/
author: Awais Hafeez
summary: ''
tags: ['Insert bookmarks in Word documents in Java']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose_words-for-java.png" alt="">}}


We are pleased to announce the new monthly release of [**Aspose.Words for Java 18.9**][1]. The release of this month contains a number of new features, enhancements, and bug fixes. Please check the detailed [release notes of Aspose.Words for Java 18.9][2] to get an idea about all the new features/enhancements and fixes made in this release. Furthermore, if you are planning to upgrade the API from any previous version, we strongly recommend you to check the Public API Changes section of current release and other intermediate releases from release notes folder, to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## Work with Bookmarks on Block, Cell, Row Levels

Starting from Aspose.Words 18.9, the bookmarks are allowed on the block, cell, and row levels. We have added AnnotationsAtBlockLevel and AnnotationsAtBlockLevelAsDefault properties in LoadOptions class to work with block-level bookmarks. Please read the following article for more details.

*   [Working with Bookmark on Block, Cell, Row Levels][3]

## Convert EquationXML to Office Math

A new property LoadOptions.ConvertShapeToOfficeMath has been added in this version of Aspose.Words to convert shapes with EquationXML to Office Math objects. Please refer to the following article for more details:

*   [Import Shapes with Math XML as Shapes into DOM][4]

## Switch Between Old and New Mail Merge Behaviors

We have added new property UnconditionalMergeFieldsAndRegions in MailMerge class to merge fields and merge regions regardless of the parent IF field’s condition. Please refer to the following article for more details.

*   [Switch Between Old and New Mail Merge Behaviors][5]

## Improved PDF Encryption when Owner Password is not Specified

Previously Aspose.Words used to create random owner password in the produced PDF document when PdfEncryptionDetails.OwnerPassword was not set by the user. Starting from this release i.e. 18.9, Aspose.Words properly sets the empty owner password when saving to PDF.

## Other Improvements

There are 85 improvements and fixes in this regular monthly release. The most notable are:

*   **Animated GIF** is fully supported now
*   **MANIFEST.MF** updated to support new OSGI versions
*   TIFF colors accuracy improved
*   **Java 10** and **Java 11** compatibility improved: reflection for safe using of optional external libraries is removed
*   Bookmarks are allowed on the block, cell, row-level 
*   Added load option to treat Shapes with math XML as Shapes in the model 
*   Provided option to choose between Old and New Mail Merge behaviors 
*   Improved PDF encryption in the case when the owner password is not specified 
*   Metafile rendering improved: fixed drawing records processing when path bracket is opened, fixed processing of EMR\_SETBKMODE record when incorrect values specified
*   Improved output image quality when rendering metafiles with raster operations set
*   Fixed handling of glyphs without outlines when parsing glyph data while rendering
*   Fixed a bug with a glow effect, if the specified glow size is less than 10
*   Fixed several problems in DrawingML Charts rendering: incorrect default axis color, bug with the date format for axis values, bug with rendering of the trend line with unsorted x-values
*   Improved rendering of the mathematical element "Apostrophe" of the MathML object 
*   Improved justification of Asian texts
*   Improved rendering of revisions in balloons
*   Improved text placement around floating shapes
*   Fixed issue with paragraph spacing in footnotes
*   Fixed issue with line wrapping when it has single glyph wider than the line followed by the page break
*   Fixed issue with table row height calculation when cells in vertical merge have horizontal borders

The following resources will help you work with Aspose.Words for Java:

*   [Home page for Aspose.Words for Java][6]
*   [Install Aspose.Words for Java from Maven][7]
*   Words product family forum – Post your technical questions and queries, or any other problem you faced while running Aspose.Words APIs.
    *   [Free Support Forum][8]
    *   [Paid Support Forum][9]
*   [Aspose.Words for Java online documentation][10]– Help documentation.
*   [Aspose.Words for Java online API reference][11]– API reference documents.
*   [Enable Blog Subscription][12]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words, APIs, new features, fixes, and other API related topics by subscribing to Aspose.Words blog.
*   [Aspose.Words for Java Examples][13] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[2]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+18.9+Release+Notes
[3]: https://docs.aspose.com/display/wordsjava/Working+with+Bookmarks#WorkingwithBookmarks-WorkingwithBookmarkonBlock,Cell,RowLevels
[4]: https://docs.aspose.com/display/wordsjava/Use+DocumentBuilder+to+Insert+Document+Elements#UseDocumentBuildertoInsertDocumentElements-ImportShapeswithMathXMLasShapesintoDOM
[5]: https://docs.aspose.com/display/wordsjava/How+to+Execute+Mail+Merge#HowtoExecuteMailMerge-SwitchBetweenOldandNewMailMergeBehaviors
[6]: https://products.aspose.com/words/java
[7]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[8]: https://forum.aspose.com/c/words
[9]: https://helpdesk.aspose.com/
[10]: https://docs.aspose.com/display/wordsjava/Home
[11]: https://apireference.aspose.com/java/words
[12]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[13]: https://github.com/aspose-words/Aspose.Words-for-Java




