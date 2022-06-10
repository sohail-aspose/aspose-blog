---
title: 'Set Fallback Font and Remove Empty Paragraphs in Word Document using C#'
date: Wed, 17 Oct 2018 11:01:57 +0000
draft: false
url: /2018/10/17/set-fallback-font-and-remove-empty-paragraphs-in-word-document/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-net.png" alt="Aspose.Words for .NET logo">}}


We are pleased to announce our next version [Aspose.Words for .NET 18.10][1]. This month’s release contains over 64 useful new features, enhancements and bug fixes. Please check the [release notes][2] to get an idea about all new features, enhancements and fixes made in this release. If you are planning to upgrade from older version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][3] section to know what APIs are changed so far.

## Set Font Fallback Settings for Rendering in Word Document

A new feature has been added in Aspose.Words 18.10 to set font fallback settings. Font fallback is used when font is resolved but it doesn't contain a specific character. We have added new property FontSettings.FallbackSettings to set the settings related to font fallback mechanism. A new class FontFallbackSettings is also added for fallback mechanism settings. Please read the following article for more detail.

[Font substitution and Font fallback in Aspose.Words][4]

## Remove Empty Paragraphs by LINQ Reporting Engine

We have added new feature in Aspose.Words 18.10 to remove empty paragraphs while generating report by LINQ Reporting engine. The paragraphs are generated after the removal of template syntax tags and replaced tags with empty value. We have added new member RemoveEmptyParagraphs to ReportBuildOptions enumeration to remove empty paragraphs. Please read the following article for more detail.

[How to Remove Empty Paragraphs][5]

## Get Actual Bounding Box of Shape

We have added new property [NodeRendererBase.BoundsInPoints][6] in Aspose.Words 18.10 to get the actual bounding box of the shape as rendered on the page. For more detail, please read the following article.

[How to Get Actual Bounds of Shape in Points][7]

## Set the Style of Content Control to Format Text Typed

We have added two new properties named Style and StyleName in [StructuredDocumentTag][8] class to set or get the style applied to content control. Please read the following article for more detail.

[How to Set Style to Format Text Typed into the Content Control][9]

## Copy All Styles from Template

A new feature has been added in this version of Aspose.Words to copy all styles of the document into another document. For this purpose, we have added the following two methods in Document class. Please read the following article for more detail.

[Copy All Styles from Template][10]

## Insert Untyped/Empty Field into Document

MS Word allows to insert an empty field into document. We have added this feature in Aspose.Words 18.10 to insert an empty field into document. Please read the following article for more detail.

[How to Insert Untyped/Empty Field][11]

## Allow Spacing Between Cells of Table

A new property Table.AllowCellSpacing has been added in this version of Aspose.Words to set or get the option "Allow spacing between cells" of table. Please read following article for more detail.

[Allow Spacing Between Cells][12]

## Insert Horizontal Rule into Document

We have added new feature in Aspose.Words 18.10 to insert horizontal rule into document. A new method InsertHorizontalRule() has been added to DocumentBuilder class. Please read following article for more detail.

[Insert Horizontal Rule into Document][13]

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Implemented new API to set up font fallback mechanism through XML configuration
*   Provide option to Use a style to format text typed into the SDT control
*   Add feature to insert Horizontal Rule into document
*   PNG images with a corrupted file structure are not skipped now from the rendering if it is possible to read information about their size
*   Improved rendering of abscissa labels of a DrawingML Chart if the axis contains a large number of dummy values
*   Improved scaling of the vertical axis of DrawingML Charts if a small range is used
*   Fixed an error causing an exception while rendering pattern-filled DrawingML shapes when pattern is not specified
*   Fixed a rendering glitch caused by negative arcsize of rounded rectangle VML shapes
*   Fixed a bug with rendering of the gridlines in a DrawingML Chart if the interval between tick marks is specified
*   Fixed a bug with rendering of the second axis title in a DrawingML Chart if manual layout is set
*   Fixed issue with paragraph above spacing for page break lines in compatibility mode
*   Fixed rendering of hidden paragraph in TOC fields
*   Fixed line wrapping in compatibility mode when line break follows inline shape wider that column
*   Improved rendering of underlines, it is now based on fields of the POST table in OTF fonts
*   Improved alignment of page relative shapes for documents created in Word 2013 and later
*   LINQ Reporting Engine supports removal of paragraphs becoming empty after template syntax tags are removed or replaced with empty values

## Aspose.Words for .NET Resources

The following resources will help you work with Aspose.Words for .NET:

1.  [Home page of .NET API][14].
2.  [Install using NuGet Package][15]
3.  [Documentation][16] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
4.  [API Reference Guide][17] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
5.  Aspose.Words Product Family Forum – post your technical questions and queries, or any other problem you are facing while working with Aspose.Words APIs.
    *   [Free Support Forum][18]
    *   [Paid Support Forum][19]
6.  [Enable Blog Subscription][20] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
7.  [Examples][21] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Words/
[2]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+18.10+Release+Notes
[3]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET
[4]: https://docs.aspose.com/display/wordsnet/True+Type+Fonts#TrueTypeFonts-FontsubstitutionandFontfallbackinAspose.Words
[5]: https://docs.aspose.com/display/wordsnet/Template+Syntax#TemplateSyntax-HowtoRemoveEmptyParagraphs
[6]: https://apireference.aspose.com/net/words/aspose.words.rendering/noderendererbase/properties/boundsinpoints
[7]: https://docs.aspose.com/display/wordsnet/Working+with+Images#WorkingwithImages-HowtoGetActualBoundsofShapeinPoints
[8]: https://apireference.aspose.com/net/words/aspose.words.markup/structureddocumenttag/
[9]: https://docs.aspose.com/display/wordsnet/Working+with+Content+Control+SDT#WorkingwithContentControlSDT-HowtoSetStyletoFormatTextTypedintotheContentControl
[10]: https://docs.aspose.com/display/wordsnet/Working+with+Styles#WorkingwithStyles-CopyAllStylesfromTemplate
[11]: https://docs.aspose.com/display/wordsnet/Inserting+Fields#InsertingFields-HowtoInsertUntyped/EmptyField
[12]: https://docs.aspose.com/display/wordsnet/Applying+Formatting#ApplyingFormatting-AllowSpacingBetweenCells
[13]: https://docs.aspose.com/display/wordsnet/Use+DocumentBuilder+to+Insert+Document+Elements#UseDocumentBuildertoInsertDocumentElements-InsertHorizontalRuleintoDocument
[14]: https://products.aspose.com/words/net
[15]: https://www.nuget.org/packages/Aspose.Words/
[16]: https://docs.aspose.com/display/wordsnet
[17]: https://apireference.aspose.com/net/words
[18]: https://forum.aspose.com/c/words
[19]: https://helpdesk.aspose.com/
[20]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[21]: https://github.com/aspose-words/Aspose.Words-for-.NET




