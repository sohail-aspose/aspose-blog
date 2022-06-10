---
title: 'Insert Horizontal Rule and Remove Empty Paragraphs in Word Documents using Java'
date: Wed, 24 Oct 2018 12:20:11 +0000
draft: false
url: /2018/10/24/insert-horizontal-rule-and-remove-empty-paragraphs-in-word-using-java/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

We are pleased to announce the new monthly release of [**Aspose.Words for Java 18.10**][1]. The release of this month contains number of new features, enhancements and bug fixes of the issues reported by our users in previous versions. Please check the detailed [release notes of Aspose.Words for Java 18.10][2] to get an idea about all the new features/enhancements and fixes made in this release. Furthermore, if you are planning to upgrade the API from any previous version, we strongly recommend you to check the Public API Changes section of current release and other intermediate releases from release notes folder, to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## Set Font Fallback Settings for Rendering Word Documents

A new feature has been added in Aspose.Words 18.10 to set font fallback settings. Font fallback is used when the font is resolved but it doesn’t contain a specific character. We have added new property FontSettings.FallbackSettings to set the settings related to font fallback mechanism. A new class FontFallbackSettings is also added for fallback mechanism settings. Please read the following article for more detail.

*   [Font substitution and Font fallback in Aspose.Words][3]

## Get Actual Bounding Box of Shape

We have added a new property NodeRendererBase.BoundsInPoints in Aspose.Words 18.10 to get the actual bounding box of the shape as rendered on the page. For more detail, please read the following article.

*   [How to Get Actual Bounds of Shape in Points][4]

## Set the Style of Content Control to Format Text Typed

We have added two new properties named Style and StyleName in StructuredDocumentTag class to set or get the style applied to content control. Please read following article for more detail.

*   [How to Set Style to Format Text Typed into the Content Control][5]

## Copy All Styles from Template

A new feature has been added in this version of Aspose.Words to copy all styles of the document into another document. For this purpose, we have added the following two methods in Document class.

1.  public void Document.copyStylesFromTemplate(String template)
2.  public void Document.copyStylesFromTemplate(Document template)

Please read the following article for more detail.

*   [Copy All Styles from Template][6]

## Insert Untyped/Empty Field into Document

MS Word allows inserting an empty field into documents. We have added this feature in Aspose.Words 18.10 to insert an empty field into document. Please read the following article for more detail.

*   [How to Insert Untyped/Empty Field][7]

## Allow Spacing Between Cells of Table

A new property Table.AllowCellSpacing has been added in this version of Aspose.Words to set or get the option “Allow spacing between cells” of the table. Please read the following article for more detail.

*   [Allow Spacing Between Cells][8]

## Insert Horizontal Rule into Document

We have added a new feature in Aspose.Words 18.10 to insert the horizontal rule into the document. A new method InsertHorizontalRule() has been added to DocumentBuilder class. Please read the following article for more detail.

*   [Insert Horizontal Rule into Document][9]

## Other Improvements

There are 84 improvements and fixes in this regular monthly release. The most notable are:

*   Aspose.Words for Java is FIPS compliant now. The single sentence 'SecuritySettings.startFipsMode()' switches current Aspose.Words thread to the FIPS mode.
*   Support Conholdate.Total for Java licensing system.
*   Compatibility within GroupDocs Total package is improved.
*   Just another Veracode Security Scan Report is fixed.
*   Java 10/11 compatibility updates caused few bugs on some old Java Runtime Environments. We managed to fix these bugs quickly.
*   Massive JavaDoc fixes.
*   Aspose.BarCode compatibility changed to a new architecture that started from v.18.8. BarCode inside AW documents is more consistent now.
*   Implemented new API to set up font fallback mechanism through XML configuration.
*   Provide option to Use a style to format text typed into the SDT control.
*   Add feature to insert Horizontal Rule into document.
*   PNG images with a corrupted file structure are not skipped now from the rendering if it is possible to read information about their size.
*   Improved rendering of abscissa labels of a DrawingML Chart if the axis contains a large number of dummy values.
*   Improved scaling of the vertical axis of DrawingML Charts if a small range is used.
*   Fixed an error causing an exception while rendering pattern-filled DrawingML shapes when pattern is not specified.
*   Fixed a rendering glitch caused by negative arcsize of rounded rectangle VML shapes.
*   Fixed a bug with rendering of the gridlines in a DrawingML Chart if the interval between tick marks is specified.
*   Fixed a bug with rendering of the second axis title in a DrawingML Chart if manual layout is set.
*   Fixed issue with paragraph above spacing for page break lines in compatibility mode.
*   Fixed rendering of hidden paragraph in TOC fields.
*   Fixed line wrapping in compatibility mode when line break follows inline shape wider that column.
*   Improved rendering of underlines, it is now based on fields of the POST table in OTF fonts.
*   Improved alignment of page relative shapes for documents created in Word 2013 and later.
*   LINQ Reporting Engine supports removal of paragraphs becoming empty after template syntax tags are removed or replaced with empty values.

The following resources will help you work with Aspose.Words for Java:

*   [Home page for Aspose.Words for Java][10]
*   [Install Aspose.Words for Java from Maven][11]
*   Words product family forum – Post your technical questions and queries, or any other problem you faced while running Aspose.Words APIs.
    *   [Free Support Forum][12]
    *   [Paid Support Forum][13]
*   [Aspose.Words for Java online documentation][14]– Help documentation.
*   [Aspose.Words for Java online API reference][15]– API reference documents.
*   [Enable Blog Subscription][16]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words, APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
*   [Aspose.Words for Java Examples][17] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[2]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+18.10+Release+Notes
[3]: https://docs.aspose.com/display/wordsjava/True+Type+Fonts#TrueTypeFonts-FontsubstitutionandFontfallbackinAspose.Words
[4]: https://docs.aspose.com/display/wordsjava/Working+with+Images#WorkingwithImages-HowtoGetActualBoundsofShapeinPoints
[5]: https://docs.aspose.com/display/wordsjava/Working+with+Content+Control+SDT#WorkingwithContentControlSDT-HowtoSetStyletoFormatTextTypedintotheContentControl
[6]: https://docs.aspose.com/display/wordsjava/Working+with+Styles#WorkingwithStyles-CopyAllStylesfromTemplate
[7]: https://docs.aspose.com/display/wordsjava/Insert+and+Remove+Field#InsertandRemoveField-HowtoInsertUntyped/EmptyField
[8]: https://docs.aspose.com/display/wordsjava/Applying+Formatting+to+Table%2C+Row+and+Cell#ApplyingFormattingtoTable,RowandCell-AllowSpacingBetweenCells
[9]: https://docs.aspose.com/display/wordsjava/Use+DocumentBuilder+to+Insert+Document+Elements#UseDocumentBuildertoInsertDocumentElements-InsertHorizontalRuleintoDocument
[10]: https://products.aspose.com/words/java
[11]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[12]: https://forum.aspose.com/c/words
[13]: https://helpdesk.aspose.com/
[14]: https://docs.aspose.com/display/wordsjava/Home
[15]: https://apireference.aspose.com/java/words
[16]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[17]: https://github.com/aspose-words/Aspose.Words-for-Java




