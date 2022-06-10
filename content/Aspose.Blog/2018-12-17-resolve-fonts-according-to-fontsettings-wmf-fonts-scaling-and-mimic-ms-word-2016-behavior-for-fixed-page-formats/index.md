---
title: 'Resolve Fonts According to FontSettings, WMF Fonts Scaling, and Mimic MS Word 2016 Behavior for Fixed-Page Formats'
date: Mon, 17 Dec 2018 10:13:00 +0000
draft: false
url: /2018/12/17/resolve-fonts-according-to-fontsettings-wmf-fonts-scaling-and-mimic-ms-word-2016-behavior-for-fixed-page-formats/
author: Tahir Manzoor
summary: ''
tags: ['Mimic MS Word 2016 behavior for fixed-page', 'Resolve Fonts in Word Document', 'Scale WMF Fonts in Word']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-net.png" alt="Aspose.Words for .NET logo">}}


We are pleased to announce our next version [Aspose.Words for .NET 18.12][1]. This month’s release contains over 96 useful new features, enhancements and bug fixes. Please check the [**release notes**][2] to get an idea about all new features, enhancements and fixes made in this release. If you are planning to upgrade from older version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][3] section to know what APIs are changed so far.

## Mimic MS Word 2016 Behavior for Handling Hide Mark Element in Table Cell

In old versions of Aspose.Words, handling of hide mark element in a table cell for rendering document to fixed page format is according to MS Word 2013 behavior. Starting from Aspose.Words 18.12, we have changed this behaviour to mimic MS Word 2016 behavior. For more detail, please check Aspose.Words 18.12 [release notes][4].

## Mimic MS Word 2016 Behavior for Special Cases With Continuous and New Column Section Breaks

In some situations, for continuous and "new column" section breaks, the behavior of MS Word 2016 is different from MS Word 2013 or an earlier version when document is converted to fixed file formats e.g. PDF, XPS. We have changed the behavior of Aspose.Words to mimic MS Word 2016. The behavior has changed for computing page numbers and for providing an empty facing page when adjacent pages have the same oddity. For more detail, please check Aspose.Words 18.12 [release notes][5].

## Added Feature to Scale WMF Fonts According to Metafile Size on the Page

In this version of Aspose.Words, we have added new property [ScaleWmfFontsToMetafileSize][6] in MetafileRenderingOptions class to control the scaling of fonts in WMF meta-file according to meta-file size on the page when redering document to fixed file format. This property is used only when meta-file is rendered as vector graphics. Please read following article for more detail.

[WMF Fonts Scaling According to Metafile Size on the Page][7]

## Added Feature to Resolve and Substitute Fonts According to FontSettings

By default, Aspose.Words uses font family names from source document and writes to HTML. Starting from Aspose.Words 18.12, you can resolve and substitute fonts according to FontSettings. We have added new property HtmlSaveOptions.ResolveFontNames to achieve this. For more detail, please read following article.

[Resolve and Substitute Fonts According to FontSettings][8]

## Obsolete Property AllowTrailingWhitespaceForListItems was Removed from LoadOptions Class

Obsolete property AllowTrailingWhitespaceForListItems was removed from LoadOptions class. Please use TxtLoadOptions.DetectNumberingWithWhitespaces instead.

## Removed Obsolete Public API Method 'SetAsDefault' from LoadOptions.LanguagePreferences

We have removed obsolete public API method 'SetAsDefault' from LoadOptions.LanguagePreferences in this version of Aspose.Words. Please use LanguagePreferences.DefaultEditingLanguage property instead. It was introduced in [Aspose.Words for .NET 18.6][9].

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Implemented WMF fonts scaling, according to metafile size on the page, and public option to control it (MetafileRenderingOptions.ScaleWmfFontsToMetafileSize).
*   Improved the default font fallback mechanism to better fit the MW behavior.
*   Optimized metafile from SVG rendering to skip redundant line segments.
*   Fixed a bug that caused an exception when rendering metafiles filled with gradient.
*   Fixed a bug with the order of legend items of the stacked DrawingML chart when rendering.
*   Fixed a bug with text clipping when rendering the DrawingML charts.
*   Fixed a bug with rendering of minor tick marks and clipping the rightmost bar of DrawingML charts.
*   Fixed a bug with rendering data labels for points, located on the border of the DrawingML chart plot area.
*   Implemented support for RTL comments rendering, e.g. Arabic.
*   Improved hyphenation logic for multiple cases.
*   Improved page numbering for sections starting in new columns.
*   Improved table row alignment.
*   Improved tab stop calculations with paragraph indents.
*   Improved table breaking logic for numerous complex cases.
*   Improved handling of character compression within mixed ltr/rtl text.
*   Fixed exception in rare case when field update causes line to contain only zero length spans.
*   Fixed exception in rare case when floating object is pushed beyond empty column.
*   Fixed layout when tables merge over the hidden paragraph.

## Aspose.Words for .NET Resources

The following resources will help you work with Aspose.Words for .NET:

1.  [Home page of .NET API][10].
2.  [Install using NuGet Package][11]
3.  [Documentation][12] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
4.  [API Reference Guide][13] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
5.  Aspose.Words Product Family Forum – post your technical questions and queries, or any other problem you are facing while working with Aspose.Words APIs.
    *   [Free Support Forum][14]
    *   [Paid Support Forum][15]
6.  [Enable Blog Subscription][16] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
7.  [Examples][17] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Words/
[2]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+18.12+Release+Notes
[3]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET
[4]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+18.12+Release+Notes
[5]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+18.12+Release+Notes
[6]: https://apireference.aspose.com/net/words/aspose.words.saving/metafilerenderingoptions/properties/scalewmffontstometafilesize
[7]: https://docs.aspose.com/display/wordsnet/Rendering#Rendering-WMFFontsScalingAccordingtoMetafileSizeonthePage
[8]: https://docs.aspose.com/display/wordsnet/Saving+a+Document#SavingaDocument-ResolveandSubstituteFontsAccordingtoFontSettings
[9]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+18.6+Release+Notes
[10]: https://products.aspose.com/words/net
[11]: https://www.nuget.org/packages/Aspose.Words/
[12]: https://docs.aspose.com/display/wordsnet
[13]: https://apireference.aspose.com/net/words
[14]: https://forum.aspose.com/c/words
[15]: https://helpdesk.aspose.com/
[16]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[17]: https://github.com/aspose-words/Aspose.Words-for-.NET




