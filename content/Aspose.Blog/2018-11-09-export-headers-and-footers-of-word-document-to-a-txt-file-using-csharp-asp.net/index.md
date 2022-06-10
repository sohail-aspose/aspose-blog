---
title: 'Export Headers and Footers of Word Document to a TXT File using C#'
date: Fri, 09 Nov 2018 14:29:32 +0000
draft: false
url: /2018/11/09/export-headers-and-footers-of-word-document-to-a-txt-file-using-csharp-asp.net/
author: Tahir Manzoor
summary: ''
tags: ['Export Word to TXT in Csharp', 'Export headers and footers in Word to TXT']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-net.png" alt="Aspose.Words for .NET logo">}}


We are pleased to announce our next version [Aspose.Words for .NET 18.11][1]. This month’s release contains over 69 useful new features, enhancements, and bug fixes. Please check the [**release notes**][2] to get an idea about all new features, enhancements, and fixes made in this release. If you are planning to upgrade from an older version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][3] section to know what APIs are changed so far.

## Export Header and Footer in Word Document to TXT File

A new feature has been added in Aspose.Words 18.11 to export all headers and footers at the end of the document. We have added new property TxtSaveOptions.ExportHeadersFootersMode in this version of Aspose.Words. The main advantage of a new property over the old TxtSaveOptions.ExportHeadersFooters property is that it has new headers and footers export mode: 'AllAtEnd'. In this mode Aspose.Words acts the way similar to MS Word; all headers and footers are placed after all section bodies at the very end of a document.

The following code sample shows how to export header and footer in a Word document to a TXT file using C#.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Loading-and-Saving-WorkingwithTxt-ExportHeadersFootersMode.cs" >}}

Please read the following article for more details.

*   [Export Header and Footer in Output TXT][4]

## Other API Changes

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Fixed hang with auto-sized tables when the cell has right-aligned floaters.
*   Fixed wrong visual order of text in specific cases.
*   Fixed non-breaking space widths calculation.
*   Implemented support for floating table metrics when calculating grid.
*   ROP (raster operations) emulation code was improved, resulting in a significant performance boost (up to 5 times) when rendering the corresponding metafiles.
*   Improved legacy vertical writing support in EMF rendering.

Fonts with the '@' prefix additionally rotate the Japanese glyphs.

*   Improved calculation of the shape boundaries, more accurately mimicking the MS Word output.
*   Improved the rendering of DrawingML charts canvases overlay.

Markers of the “nofill” series are rendered on the foreground.

*   Improved rendering of DrawingML chart axes for documents created using MS Word 2007.
*   Fixed a bug with an incorrect resolution of the system “window” color when rendering of VML shapes.
*   Fixed an issue with underline/strikeout text effects in EMF/WMF rendering.
*   Fixed a document rendering issue when font with English name could not be found in the system with a different locale.
*   Fixed bug with rendering of DrawingML chart markers, if series data are not sorted in ascending order.
*   Fixed a bug causing shifts of rotated shapes in DrawingML chart while rendering.
*   Provided TxtSaveOptions.

ExportHeadersFootersMode property.

## Aspose.Words for .NET Resources

The following resources will help you work with Aspose.Words for .NET:

1.  [Home page of .NET API][5].
2.  [Install using NuGet Package][6]
3.  [Documentation][7] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
4.  [API Reference Guide][8] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
5.  Aspose.Words Product Family Forum – post your technical questions and queries, or any other problem you are facing while working with Aspose.Words APIs.
    *   [Free Support Forum][9]
    *   [Paid Support Forum][10]
6.  [Enable Blog Subscription][11] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
7.  [Examples][12] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Words/
[2]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+18.11+Release+Notes
[3]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET
[4]: https://docs.aspose.com/display/wordsnet/Working+with+Text+Document#WorkingwithTextDocument-ExportHeaderandFooterinOutputTXT
[5]: https://products.aspose.com/words/net
[6]: https://www.nuget.org/packages/Aspose.Words/
[7]: https://docs.aspose.com/display/wordsnet
[8]: https://apireference.aspose.com/net/words
[9]: https://forum.aspose.com/c/words
[10]: https://helpdesk.aspose.com/
[11]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[12]: https://github.com/aspose-words/Aspose.Words-for-.NET




