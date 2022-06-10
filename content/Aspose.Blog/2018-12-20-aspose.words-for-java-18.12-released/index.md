---
title: 'Scale WMF Fonts to Match Metafile Size using Aspose.Words for Java 18.12'
date: Thu, 20 Dec 2018 08:09:18 +0000
draft: false
url: /2018/12/20/aspose.words-for-java-18.12-released/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose_words-for-java.png" alt="">}}


We are pleased to announce the new monthly release of [**Aspose.Words for Java 18.12**][1]. The release of this month contains a number of new features, enhancements and bug fixes of the issues reported by our users in previous versions. Please check the detailed [release notes of Aspose.Words for Java 18.12][2] to get an idea about all the new features/enhancements and fixes made in this release. Furthermore, if you are planning to upgrade the API from any previous version, we strongly recommend you to check the Public API Changes section of current release and other intermediate releases from release notes folder, to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## Scale WMF Fonts According to Metafile Size on the Page

In this version of Aspose.Words, we have added new property ScaleWmfFontsToMetafileSize in MetafileRenderingOptions class to control the scaling of fonts in WMF meta-file according to meta-file size on the page when rendering the document to the fixed file format. This property is used only when meta-file is rendered as vector graphics. Please read the following article for more details.

[WMF Fonts Scaling According to Metafile Size on the Page][3]

## Handling Hide Mark Element in Table Cell

In old versions of Aspose.Words, handling of 'hide mark element' in a table cell for rendering document to fixed page format is according to MS Word 2013 behavior. Starting from Aspose.Words 18.12, we have changed this behavior and mimic MS Word 2016 behavior. For more details, please check Aspose.Words 18.12 release notes.

[Aspose.Words for Java 18.12 release notes][4]

## Special Cases with Continuous and New Column Section Breaks

In some situations, for "continuous" and "new column" section breaks, the behavior of MS Word 2016 is different from MS Word 2013 or an earlier version when document is converted to fixed file formats e.g. PDF, XPS. We have changed the behavior of Aspose.Words and now it mimics MS Word 2016. The behavior has changed for computing page numbers and for providing an empty facing page when adjacent pages have the same oddity. For more detail, please check Aspose.Words 18.12 release notes

[Aspose.Words for Java 18.12 release notes][5]

## Resolve and Substitute Fonts According to FontSettings

By default, Aspose.Words uses font family names from source document and writes to HTML. Starting from Aspose.Words 18.12, you can resolve and substitute fonts according to FontSettings. We have added new property HtmlSaveOptions.ResolveFontNames to achieve this. For more details, please read following article.

[Resolve and Substitute Fonts According to FontSettings][6]

## Obsolete Property AllowTrailingWhitespaceForListItems was Removed from LoadOptions Class

Obsolete property AllowTrailingWhitespaceForListItems was removed from LoadOptions class. Please use TxtLoadOptions.DetectNumberingWithWhitespaces instead.

## Removed Obsolete Public API Method ‘SetAsDefault’ from LoadOptions.LanguagePreferences

We have removed obsolete public API method ‘SetAsDefault’ from LoadOptions.LanguagePreferences in this version of Aspose.Words. Please use LanguagePreferences.DefaultEditingLanguage property instead. It was introduced in [Aspose.Words for Java 18.6][7].

## Other Improvements

There are 108 improvements and fixes in this regular monthly release. The most notable are:

*   Java 11 compatibility is checked and updated.
*   ExternalImageLibTest utility class added to check external image libraries on user side.
*   Implemented WMF fonts scaling, according to metafile size on the page, and public option to control it (MetafileRenderingOptions.ScaleWmfFontsToMetafileSize).
*   Improved the default font fallback mechanism to better fit the MW behavior.
*   Optimized metafile from SVG rendering to skip redundant line segments.
*   Fixed a bug that caused an exception when rendering metafiles filled with gradient.
*   Fixed a bug with the order of legend items of the stacked DrawingML chart when rendering.
*   Fixed a bug with text clipping when rendering the DrawingML charts.
*   Fixed a bug with rendering of minor tick marks and clipping the rightmost bar of DrawingML charts.
*   Fixed a bug with rendering data labels for points, located on the border of the DrawingML chart plot area.
*   Implemented support for RTL comments rendering, e.g. Arabic.
*   Improved hyphenation logic for multiple cases.
*   Improved page numbering for sections starting in new columns.
*   Improved table row alignment.
*   Improved tab stop calculations with paragraph indents.
*   Improved table breaking logic for numerous complex cases.
*   Improved handling of character compression within mixed ltr/rtl text.
*   Fixed exception in rare case when field update causes line to contain only zero length spans.
*   Fixed exception in rare case when floating object is pushed beyond empty column.
*   Fixed layout when tables merge over the hidden paragraph.

The following resources will help you work with Aspose.Words for Java:

*   [Home page for Aspose.Words for Java][8]
*   [Install Aspose.Words for Java from Maven][9]
*   Words product family forum – Post your technical questions and queries, or any other problem you faced while running Aspose.Words APIs.
    *   [Free Support Forum][10]
    *   [Paid Support Forum][11]
*   [Aspose.Words for Java online documentation][12]– Help documentation.
*   [Aspose.Words for Java online API reference][13]– API reference documents.
*   [Enable Blog Subscription][14]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words, APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
*   [Aspose.Words for Java Examples][15] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[2]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+18.12+Release+Notes
[3]: https://docs.aspose.com/display/wordsjava/Rendering#Rendering-WMFFontsScalingAccordingtoMetafileSizeonthePage
[4]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+18.12+Release+Notes
[5]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+18.12+Release+Notes
[6]: https://docs.aspose.com/display/wordsjava/Saving+a+Document#SavingaDocument-ResolveandSubstituteFontsAccordingtoFontSettings
[7]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+18.6+Release+Notes
[8]: https://products.aspose.com/words/java
[9]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[10]: https://forum.aspose.com/c/words
[11]: https://helpdesk.aspose.com/
[12]: https://docs.aspose.com/display/wordsjava/Home
[13]: https://apireference.aspose.com/java/words
[14]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[15]: https://github.com/aspose-words/Aspose.Words-for-Java




