---
title: 'Support of Getting Available Fonts List and Revision Groups in Aspose.Words for Java 18.7'
date: Sat, 21 Jul 2018 07:38:05 +0000
draft: false
url: /2018/07/21/aspose.words-for-java-18.7-released/
author: Awais Hafeez
summary: ''
tags: ['Export header/footer bookmarks to PDF', 'Extract the revision groups from the Word', 'Get the list of available fonts in Word']
categories: ['Aspose.Words Product Family']
---

We are pleased to announce the new monthly release of [**Aspose.Words for Java 18.7**][1]. The release of this month contains a number of new features, enhancements and bug fixes of the issues reported by our users in previous versions. Please check the detailed [release notes of Aspose.Words for Java 18.7][2] to get an idea about all the new features/enhancements and fixes made in this release. Furthermore, if you are planning to upgrade the API from any previous version, we strongly recommend you to check the Public API Changes section of current release and other intermediate releases from release notes folder, to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## Revision Groups Supported

If a document has revisions, MS Word shows similar revisions in a group in “Reviewing Pane”. We have added support of revision groups in this version of Aspose.Words to get similar revisions e.g. insert, delete, etc. We have added RevisionCollection.Groups property, RevisionGroupCollection and RevisionGroup classes in this version to work with revision groups. Please read the following article for more detail.  
[Access Revision Group][3]

## Export Header and Footer Bookmarks in Output PDF

In some cases, Word document has more than one section that contain bookmarks in the header/footer. We have added a new feature in this version of Aspose.Words to control how header/footer bookmarks are exported in PDF. Please read the following article for more details:  
[Export Bookmarks in Output PDF][4]

## Get the List of Available Fonts

A new feature has been added to get the list of fonts available in Aspose.Words font engine. We have added FontSourceBase.GetAvailableFonts method in Aspose.Words 18.7 that returns the collection of PhysicalFontInfo class. This class specifies information about the physical font available. For more detail, please read the following article.  
[How to Get Available Fonts for Rendering][5]

## Introduced new Comparison Settings

MS Word allows comparing documents with comparison settings. You can ignore document formatting, header footers, fields, footnotes, tables, text boxes, comments, and case changes when documents are compared. We have added the “comparison settings” feature in this version of Aspose.Words. Please read the following article for more details.  
[Compare Word Documents and Ignore Document Formatting][6]

## Enhanced the Load Options for Text File

We have added a new TxtLoadOptions class to work with load options of text files in this version of Aspose.Words. New public properties LeadingSpacesOptions and TrailingSpacesOptions have been added in this class to control the way of handling leading and trailing spaces during loading the TXT file. Please read the following article for more details:  
[How to Handle Leading and Trailing spaces During Loading TXT][7]

We have added new public property TxtLoadOptions.DetectNumberingWithWhitespaces in Aspose.Words 18.7. The LoadOptions.AllowTrailingWhitespaceForListItems is obsolete property now. Use TxtLoadOptions.DetectNumberingWithWhitespaces property instead of it. Please refer to the following article for more details:  
[How List Items are Recognized During Loading TXT][8]

## Support for Removing Personal Information Setting from Document

We have added a new feature to remove personal information from the document. Please read the following article for more details:  
[Remove Personal Information from Document][9]

## Generics

Starting from Aspose.Words 18.7, untyped containers like ArrayList have been replaced with typed containers like List. Please read the details from here:  
[Aspose.Words for Java 18.7 Release Notes][10]

## Obsolete Method Document.RemoveUnusedResources() was Removed

Obsolete method RemoveUnusedResources() was removed from Document class. Please use Document.Cleanup() method instead.

## Obsolete Method ImageData.SetImage() was Removed

Obsolete method SetImage() was removed from ImageData class. Please use the ImageBytes property to set an image.

## Obsolete Property PageSetup.MirrorMargins was Removed

Obsolete property MirrorMargins was removed from PageSetup class. Please use the PageSetup.MultiplePages property to set MultiplePagesType.

## Other Improvements

There are 90 improvements and fixes in this regular monthly release. The most notable are:

*   New typed (generic) collections and enumerators were introduced in Aspose.Words public API
*   Added public property HeaderFooterBookmarksExportMode in PdfSaveOptions 
*   Added FontSourceBase.GetAvailableFonts method 
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
*   Improved column balancing when the column has footnotes
*   Improved handling of table grid when layout is changed programmatically
*   Improved table breaking in 2013 mode when it overlaps footer
*   Improved handling of "don't add space between paragraphs of the same style" option when only one of the paragraphs have this option set
*   Fixed issue when hanging punctuation precedes inline shape
*   Fixed issue when Kinsoku rule is analyzed for shapes

## Aspose.Words for Java Resources

The following resources will help you work with Aspose.Words for Java:

*   [Home page for Aspose.Words for Java][11]
*   [Install Aspose.Words for Java from Maven][12]
*   Words product family forum – Post your technical questions and queries, or any other problem you faced while running Aspose.Words APIs.
    *   [Free Support Forum][13]
    *   [Paid Support Forum][14]
*   [Aspose.Words for Java online documentation][15]– Help documentation.
*   [Aspose.Words for Java online API reference][16]– API reference documents.
*   [Enable Blog Subscription][17]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words, APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
*   [Aspose.Words for Java Examples][18] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[2]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+18.7+Release+Notes
[3]: https://docs.aspose.com/display/wordsjava/Working+with+Document#WorkingwithDocument-AccessRevisionGroup
[4]: https://docs.aspose.com/display/wordsjava/Rendering#Rendering-ExportBookmarksinOutputPDF
[5]: https://docs.aspose.com/display/wordsjava/True+Type+Fonts#TrueTypeFonts-HowtoGetAvailableFontsforRendering
[6]: https://docs.aspose.com/display/wordsjava/How+to+Compare+Two+Word+Documents#HowtoCompareTwoWordDocuments-CompareWordDocumentsandIgnoreDocumentFormatting
[7]: https://docs.aspose.com/display/wordsjava/Working+with+Text+Document#WorkingwithTextDocument-HowtoHandleLeadingandTrailingSpacesduringLoadingTXT
[8]: https://docs.aspose.com/display/wordsjava/Working+with+Text+Document#WorkingwithTextDocument-HowListItemsareRecognizedDuringLoadingTXT
[9]: https://docs.aspose.com/display/wordsjava/Working+with+Document#WorkingwithDocument-RemovePersonalInformationfromDocument
[10]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+18.7+Release+Notes
[11]: https://products.aspose.com/words/java
[12]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[13]: https://forum.aspose.com/c/words
[14]: https://helpdesk.aspose.com/
[15]: https://docs.aspose.com/display/wordsjava/Home
[16]: https://apireference.aspose.com/java/words
[17]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[18]: https://github.com/aspose-words/Aspose.Words-for-Java




