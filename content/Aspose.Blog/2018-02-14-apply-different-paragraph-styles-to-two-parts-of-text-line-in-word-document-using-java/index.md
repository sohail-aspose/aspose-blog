---
title: 'Apply Different Paragraph Styles to Two Parts of Text Line in Word Document using Java'
date: Wed, 14 Feb 2018 11:41:57 +0000
draft: false
url: /2018/02/14/apply-different-paragraph-styles-to-two-parts-of-text-line-in-word-document-using-java/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

We are pleased to announce the new monthly release of [**Aspose.Words for Java 18.2**][1]. The release of this month contains number of new features, enhancements and bug fixes of the issues reported by our users in previous versions. Please check the detailed [release notes of Aspose.Words for Java 18.2][2] to get an idea about all the new features/enhancements and fixes made in this release. Furthermore, if you are planning to upgrade the API from any previous version, we strongly recommend you to check the Public API Changes section of current release and other intermediate releases from release notes folder, to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## Insert Style Separator to Put Different Paragraph Styles

In this version of Aspose.Words, we have added the support of style separator to put different paragraph styles in the same printed paragraph. Style Separator can be added to the end of a paragraph using the Ctrl+Alt+Enter Keyboard Shortcut into MS Word. This feature allows for two different paragraph styles used in one logical printed paragraph. Please read following article for more detail.

*   [Insert Style Separator to Put Different Paragraph Styles][3]

## Specify Metafile format When Exporting Document to HTML

In this version, we have added HtmlSaveOptions.MetafileFormat property to specify in what format metafiles are saved when exporting to HTML, MHTML, or EPUB. By default, metafiles are rendered to raster PNG images. HtmlMetafileFormat enumeration has added to indicate the format in which metafiles are saved to HTML document. This new property replaces HtmlSaveOptions.ExportMetafileAsRaster which is now marked obsolete. For more detail, please read the following article.

*   [Specify Metafile format When Exporting Document to HTML][4]

## Enable/Disable Font Substitution

We have added new property FontSettings.EnableFontSubstitution in this version of Aspose.Words to specify whether to enable or disable font substitution. Please read the following article for more detail.

*   [Enable or Disable Font Substitution][5]

## Changed Importing Logic with KeepSourceFormatting Mode

In old versions of Aspose.Words, our import algorithm was different from what MS Word does. We imported style with expanded attributes. If a style already exists in the document, we applied a new name to it. MS Word does not import style if it already exists. It just expands attributes into the direct paragraph/run properties. We have improved the importing document logic with KeepSourceFormatting mode that is closer to MS Word’s behavior. Now we are expanding source formatting into the direct attributes of imported nodes.

## Obsolete Properties were Removed from Aspose.Words API

*   The **HtmlSaveOptions.AllowNegativeLeftIndent** was removed. Please use HtmlSaveOptions.AllowNegativeIndent property.
*   The **HtmlSaveOptions.ExportHeadersFooters** was removed. Please use HtmlSaveOptions.ExportHeadersFootersMode property.
*   The **HtmlFixedSaveOptions.MetafileRenderingMode** was removed. Please use the HtmlFixedSaveOptions.MetafileRenderingOptions.RenderingMode property.
*   The **SvgSaveOptions.MetafileRenderingMode** was removed. Please use the SvgSaveOptions.MetafileRenderingOptions.RenderingMode property.
*   The **XpsSaveOptions.HeadingsOutlineLevels** was removed. Please use OutlineOptions.HeadingsOutlineLevels property.
*   The **XpsSaveOptions.BookmarksOutlineLevel** was removed. Please use OutlineOptions.DefaultBookmarksOutlineLevel property.
*   The **XpsSaveOptions.MetafileRenderingMode** was removed. Please use MetafileRenderingOptions.RenderingMode property.

## Other Improvements

There are 102 improvements and fixes in this regular monthly release. The most notable are:

*   FontSettings.EnableFontSubstitution option added
*   Support to insert Style Separator to put different Paragraph styles
*   HtmlSaveOptions.MetafileFormat property added 
*   KeepSourceFormatting logic improved
*   Rendering of SVG graphics elements embedded into DrawingML objects (svgBlip) implemented
*   Added option to disable the internal font substitution mechanism and use the default font instead while rendering to PDF. (FontSettings.EnableFontSubstitution)
*   Fixed "Compound lines are not supported" warning generation
*   Fixed problem with path gradient brush scaling while rendering metafiles
*   Spacing  between legend items in DrawingML Charts rendering fixed
*   The data series line with "Round" cap type is rendered properly when exporting DrawingML Charts into PDF now
*   Rotated VML text boxes with non-default alignment rendering fixed
*   Auto-size calculation of rotated VML text boxes with vertical layout fixed
*   Implemented none wrapping for text frames
*   Improved paragraph spacing computation with hidden paragraphs
*   Improved custom tab stops handling around hidden paragraphs
*   Improved line wrapping around dashes
*   Improved character spacing control for complex code point sequences
*   Improved processing of out-of-order footnotes
*   Implemented mirror margins and gutter position handling when page orientation changes
*   Improved performance of reflow when document is large and has fields in headers/footers
*   Fixed text box width issue with left-aligned RTL text

## Aspose.Words for Java Resources

The following resources will help you work with Aspose.Words for Java:

*   [Home page for Aspose.Words for Java][6]
*   [Install Aspose.Words for Java from Maven][7]
*   Words product family forum – Post your technical questions and queries, or any other problem you faced while running Aspose.Words APIs.
    *   [Free Support Forum][8]
    *   [Paid Support Forum][9]
*   [Aspose.Words for Java online documentation][10]– Help documentation.
*   [Aspose.Words for Java online API reference][11]– API reference documents.
*   [Enable Blog Subscription][12]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words, APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
*   [Aspose.Words for Java Examples][13] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-words/
[2]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+18.2+Release+Notes
[3]: https://docs.aspose.com/display/wordsjava/Working+with+Styles#WorkingwithStyles-InsertStyleSeparatortoPutDifferentParagraphStyles
[4]: https://docs.aspose.com/display/wordsjava/Saving+a+Document#SavingaDocument-SpecifyMetafileformatWhenExportingDocumenttoHTML
[5]: https://docs.aspose.com/display/wordsjava/Rendering#Rendering-EnableorDisableFontSubstitution
[6]: https://products.aspose.com/words/java
[7]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-words/
[8]: https://forum.aspose.com/c/words
[9]: https://helpdesk.aspose.com/
[10]: https://docs.aspose.com/display/wordsjava/Home
[11]: https://apireference.aspose.com/java/words
[12]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[13]: https://github.com/aspose-words/Aspose.Words-for-Java




