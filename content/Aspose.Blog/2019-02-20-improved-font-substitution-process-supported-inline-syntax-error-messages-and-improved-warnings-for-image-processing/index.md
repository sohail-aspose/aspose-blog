---
title: 'Font Substitution in Word Documents and Inline Syntax Error Messages for LINQ Reporting Engine in C#'
date: Wed, 20 Feb 2019 09:47:51 +0000
draft: false
url: /2019/02/20/improved-font-substitution-process-supported-inline-syntax-error-messages-and-improved-warnings-for-image-processing/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-net.png" alt="Aspose.Words for .NET logo">}}


We are pleased to announce our next version [Aspose.Words for .NET 19.2][1]. This month’s release contains over 69 useful new features, enhancements and bug fixes. Please check the [release notes][2] to get an idea about all new features, enhancements and fixes made in this release. If you are planning to upgrade from older version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][3] section to know what APIs are changed so far.

## Improved Font Substitution Process When Rendering Documents

Aspose.Words requires TrueType fonts when rendering documents to fixed-page formats (PDF, XPS or TIFF). However, there are situations when the exact font cannot be found and Aspose.Words must substitute a similar font instead. We have improved the font substitution process in this release of Aspose.Words. Please read the complete detail from following article.

*   [Font Availability and Substitution][4]

## Supported Inline Syntax Error Messages into Template for LINQ Reporting Engine

By default, LINQ Reporting Engine throws an exception when encounters a template syntax error. To make things easier, the engine supports ReportBuildOptions.InlineErrorMessages option that enables inline syntax error message into a template document at an exact position where the error occurs during runtime. For more detail, please read the following article.

*   [Inline Syntax Error Messages into Templates][5]

## Improved Warnings for Image Processing Issues When Saving to PDF

Previously there was one generic warning with text "Unsupported image format.". Now there is a specific warning for OutOfMemoryException with the text "Not enough memory to load the image." and a generic warning with the text "Image cannot be processed. Possibly unsupported image format.".

## Removed Deprecated Public Property TxtSaveOptions.ExportHeadersFooters

We have removed deprecated public property TxtSaveOptions.ExportHeadersFooters from Aspose.Words API. Please use TxtSaveOptions.ExportHeadersFootersMode property instead. Please read the following article.

*   [Export Header and Footer in Output TXT][6]

## Other Improvements

There are 69 improvements and fixes in this regular monthly release. The most notable are:

*   Supported inline syntax error messages into templates instead of exception throwing for LINQ Reporting Engine.
*   Improved font fetching and substitution mechanism with corresponding API changes.
*   Improved warnings for image processing issues when rendering to PDF.
*   Improved font fallback rendering for full-width character Unicode ranges.
*   Metafiles with "HeaderPlaceable" structure is now rendering regardless of structure checksum. (MS Word behavior).
*   The width of the DrawingML outline is now normalized if it is below the minimum value while rendering. (MS Word behavior).
*   Fixed a bug with incorrect calculation of DrawingML TextBox shape bounds.
*   Fixed a bug with the calculation of the shape boundaries if the document contains the attribute.ShapeLayoutLikeWW8 (the behavior of MS WORD 97 should be emulated).
*   Fixed a bug that caused an exception when rendering ultra-small text boxes in GDI+.
*   Fixed a bug with the distorted filling of the DrawingML shape outline when rendering grouped shapes.
*   Fixed a bug causing creation of blank images with zero size while rendering into HTML.
*   Improved ordering of number in RTL list labels.
*   Improved check box size calculation when active form fields are exported to PDF.
*   Fixed issue when document has “printer metrics” enabled and Windows has no printer driver installed.
*   Fixed hang when table cell is broken across pages when there is a floating shape anchor in it.
*   Fixed issue when text which has borders is wrapped around a shape and does not fit.

## Aspose.Words for .NET Resources

The following resources will help you work with Aspose.Words for .NET:

1.  [Home page of .NET API][7].
2.  [Install using NuGet Package][8]
3.  [Documentation][9] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
4.  [API Reference Guide][10] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
5.  Aspose.Words Product Family Forum – post your technical questions and queries, or any other problem you are facing while working with Aspose.Words APIs.
    *   [Free Support Forum][11]
    *   [Paid Support Forum][12]
6.  [Enable Blog Subscription][13] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
7.  [Examples][14] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Words/
[2]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+19.2+Release+Notes
[3]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET
[4]: https://docs.aspose.com/display/wordsnet/True+Type+Fonts#TrueTypeFonts-FontAvailabilityandSubstitution
[5]: https://docs.aspose.com/display/wordsnet/LINQ+Reporting+Engine+API#LINQReportingEngineAPI-InliningSyntaxErrorMessagesintoTemplates
[6]: https://docs.aspose.com/display/wordsnet/Working+with+Text+Document#WorkingwithTextDocument-ExportHeaderandFooterinOutputTXT
[7]: https://products.aspose.com/words/net
[8]: https://www.nuget.org/packages/Aspose.Words/
[9]: https://docs.aspose.com/display/wordsnet
[10]: https://apireference.aspose.com/net/words
[11]: https://forum.aspose.com/c/words
[12]: https://helpdesk.aspose.com/
[13]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[14]: https://github.com/aspose-words/Aspose.Words-for-.NET




