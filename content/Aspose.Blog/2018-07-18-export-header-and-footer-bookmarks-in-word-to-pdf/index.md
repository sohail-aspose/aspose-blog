---
title: 'Export Header and Footer Bookmarks in Word Document to PDF using C#'
date: Wed, 18 Jul 2018 12:50:27 +0000
draft: false
url: /2018/07/18/export-header-and-footer-bookmarks-in-word-to-pdf/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-net.png" alt="Aspose.Words for .NET logo">}}


We are pleased to announce our next version [Aspose.Words for .NET 18.7][1]. This month’s release contains over 77 useful new features, enhancements and bug fixes. Please check the [**release notes**][2] to get an idea about all new features, enhancements and fixes made in this release. If you are planning to upgrade from older version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][3] section to know what APIs are changed so far.

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   New typed (generic) collections and enumerators were introduced in Aspose.Words.Net public API
*   Added public property HeaderFooterBookmarksExportMode in PdfSaveOptions

Added FontSourceBase.GetAvailableFonts method

*   Added public API for revision groups
*   Introduced new comparison settings
*   A new limo stretch algorithm for VML shapes rendering was developed, which most accurately repeats the output of MS Word (limo-stretched shapes)
*   Public property OutlineOptions.CreateOutlinesForHeadingsInTables added allowing to specify whether or not to create outlines for headings inside tables
*   Public method FontSourceBase.GetAvailableFonts added. It returns the list of fonts available via specific font source
*   Improved rendering of DrawingML shapes with specified parent object extents
*   EffectExtent attributes are now taken into account when calculating the bounding box for DrawingML shapes
*   Improved EMR\_ALPHABLEND record handling while rendering metafiles
*   Now hidden shapes inside the group are not visible during rendering
*   Fixed the leading spaces handling while processing EMF+ DrawString records
*   Fixed a bug when grayscale effect was incorrectly applied to metafile
*   Fixed a bug with the graphic frame rendering (invalid frame layout on the page)
*   Fixed rendering of shadow effect for transparent shapes
*   Fixed a bug with rendering of the MathML object if balanceSingleByteDoubleByteWidth property and UseFELayout property are specified
*   Improved rendering of \\0 characters
*   Improved column balancing when column has footnotes
*   Improved handling of table grid when layout is changed programmatically
*   Improved table breaking in 2013 mode when it overlaps footer
*   Improved handling of "don't add space between paragraphs of the same style" option when only one of the paragraphs have this option set
*   Fixed issue when hanging punctuation precedes inline shape
*   Fixed issue when Kinsoku rule is analyzed for shapes

## Export Header and Footer Bookmarks in Output PDF

In some cases, Word document has more than one section that contain bookmarks in the header/footer. We have added new feature in this version of Aspose.Words to control how header/footer bookmarks are exported in PDF. Please read the following article for more detail.

[Export Bookmarks in Output PDF][4]

## Support of Revision Groups

If a document has revisions, MS Word shows the similar revisions in a group in "Reviewing Pane". We have added support of revision group in this version of Aspose.Words to get the similar revisions e.g. insert, delete etc. We have added RevisionCollection.Groups property, RevisionGroupCollection and RevisionGroup classes in this version to work with revision groups. Please read the following article for more detail.

[Access Revision Group][5]

## Get the List of Available Fonts

A new feature has been added to get the list of fonts available in Aspose.Words font engine. We have added FontSourceBase.GetAvailableFonts method in Aspose.Words 18.7 that returns the collection of PhysicalFontInfo class. This class specifies information about physical font available. For more detail, please read the following article.

[How to Get Available Fonts for Rendering][6]

## Introduced new Comparison Settings

MS Word allows to compare documents with comparison settings. You can ignore document formatting, headers footers, fields, footnotes, tables, textboxes, comments and case changes when documents are compared. We have added the "comparison settings" feature in this version of Aspose.Words. Please read the following article for more detail.

[Compare Word Documents and Ignore Document Formatting][7]

## Enhanced the Load Options for Text File

We have added new TxtLoadOptions class to work with load options of text files in this version of Aspose.Words. New public properties LeadingSpacesOptions and TrailingSpacesOptions have been added in this class to control the way of handling leading and trailing spaces during loading TXT file. Please read the following article for more detail.

[How to Handle Leading and Trailing spaces During Loading TXT][8]

We have added new public property TxtLoadOptions.DetectNumberingWithWhitespaces in Aspose.Words 18.7. The LoadOptions.AllowTrailingWhitespaceForListItems is obsolete property now. Use TxtLoadOptions.DetectNumberingWithWhitespaces property instead of it. Please refer to the following article for more detail.

[How List Items are Recognized During Loading TXT  
](https://docs.aspose.com/display/wordsnet/Working+with+Text+Document#WorkingwithTextDocument-HowListItemsareRecognizedDuringLoadingTXT)

## Support of Removing Personal Information Setting from Document

We have added new feature to remove personal information from the document. Please read the following article for more detail.

[Remove Personal Information from Document][9]

## Obsolete Method Document.RemoveUnusedResources() was Removed

Obsolete method RemoveUnusedResources() was removed from Document class. Please use Document.Cleanup() method instead.

## Obsolete Method ImageData.SetImage() was Removed

Obsolete method SetImage() was removed from ImageData class. Please use the ImageBytes property to set an image.

## Obsolete Property PageSetup.MirrorMargins was Removed

Obsolete property MirrorMargins was removed from PageSetup class. Please use the PageSetup.MultiplePages property to set MultiplePagesType.

## Generics

Starting from Aspose.Words 18.7, untyped containers like **ArrayList** have been replaced with typed containers like **List<T>**. Please read the detail from here:  
[Public API and Backward Incompatible Changes][10]

## Aspose.Words for .NET Resources

The following resources will help you work with Aspose.Words for .NET:

1.  [Home page of .NET API][11].
2.  [Install using NuGet Package][12]
3.  [Documentation][13] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
4.  [API Reference Guide][14] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
5.  Aspose.Words Product Family Forum – post your technical questions and queries, or any other problem you are facing while working with Aspose.Words APIs.
    *   [Free Support Forum][15]
    *   [Paid Support Forum][16]
6.  [Enable Blog Subscription][17] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
7.  [Examples][18] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Words/
[2]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+18.7+Release+Notes
[3]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET
[4]: https://docs.aspose.com/display/wordsnet/Rendering#Rendering-ExportBookmarksinOutputPDF
[5]: https://docs.aspose.com/display/wordsnet/Working+with+Document#WorkingwithDocument-AccessRevisionGroup
[6]: https://docs.aspose.com/display/wordsnet/True+Type+Fonts#TrueTypeFonts-HowtoGetAvailableFontsforRendering
[7]: https://docs.aspose.com/display/wordsnet/Working+with+Document#WorkingwithDocument-CompareWordDocumentsandIgnoreDocumentFormatting
[8]: https://docs.aspose.com/display/wordsnet/Working+with+Text+Document#WorkingwithTextDocument-HowtoHandleLeadingandTrailingspacesDuringLoadingTXT
[9]: https://docs.aspose.com/display/wordsnet/Working+with+Document#WorkingwithDocument-RemovePersonalInformationfromDocument
[10]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+18.7+Release+Notes
[11]: https://products.aspose.com/words/net
[12]: https://www.nuget.org/packages/Aspose.Words/
[13]: https://docs.aspose.com/display/wordsnet
[14]: https://apireference.aspose.com/net/words
[15]: https://forum.aspose.com/c/words
[16]: https://helpdesk.aspose.com/
[17]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[18]: https://github.com/aspose-words/Aspose.Words-for-.NET




