---
title: 'Get Available Fonts List in Aspose.Words for Android via Java 18.7'
date: Tue, 31 Jul 2018 08:01:34 +0000
draft: false
url: /2018/07/31/aspose.words-for-android-via-java-18.7-released/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose_words-for-android-128x128.png" alt="Aspose.Words for Android via Java">}}


We are pleased to announce the new monthly release of **Aspose.Words for Android via Java 18.7**. Aspose.Words for Android via Java has full functionality of Aspose.Words for Java with [few limitations, minor API changes, and additional requirements][1]. This version also includes all bug fixes and public API changes made in Aspose.Words for Java 18.7, see the following release notes for more information.

*   [Aspose.Words for Java 18.7 release notes][2]
*   [Aspose.Words for Android via Java 18.7 release notes][3]

[Aspose.Words for Android via Java 18.7][4] now allows you to perform the following tasks:

*   [Revision Groups Supported][5]
*   [Export Header and Footer Bookmarks in Output PDF][6]
*   [Get the List of Available Fonts][7]
*   [Introduced new Comparison Settings][8]
*   [Enhanced the Load Options for Text File][9]
*   [How List Items are Recognized During Loading TXT][10]
*   [Support of Removing Personal Information Setting from Document][11]
*   [Generics Supported][12]
*   Obsolete Method Document.RemoveUnusedResources() was Removed
*   Obsolete Method ImageData.SetImage() was Removed
*   Obsolete Property PageSetup.MirrorMargins was Removed

Here is a look at just a few of the biggest features and API changes in this month’s release.

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
*   Improved column balancing when column has footnotes
*   Improved handling of table grid when layout is changed programmatically
*   Improved table breaking in 2013 mode when it overlaps footer
*   Improved handling of "don't add space between paragraphs of the same style" option when only one of the paragraphs have this option set
*   Fixed issue when hanging punctuation precedes inline shape
*   Fixed issue when Kinsoku rule is analyzed for shapes

'Aspose.Words for Android via Java' is an advanced Word document processing API to perform a wide range of document processing tasks directly within your native Android applications. Aspose.Words for Android via Java API supports DOC, OOXML, RTF, HTML, OpenDocument, PDF, XPS, EPUB and other formats. You can generate, modify, convert and render documents.  
[Learn more about Aspose.Words for Android via Java][13]

## Aspose.Words for Android via Java API Resources

The following are the links to some useful resources you may need to accomplish your tasks.

*   [Aspose.Words for Android via Java Online Documentation][14] ('Aspose.Words for Android via Java' is very similar to 'Aspose.Words for Java'. So, you can use the same documentation)
*   [Features][15]
*   [Limitations and API Differences][16]
*   [Product Page][17]
*   [Install Aspose.Words for Android via Java from Maven][18]
*   [API Reference Guide][19] (Aspose.Words for Android via Java is very similar to Aspose.Words for Java. So, you can use the same API Reference Guide)
*   [Free Support Forum][20]
*   [Paid Support Helpdesk][21]
*   [GitHub Examples][22]

## Start a Free Trial Today

Start a free trial today – all you need is to [sign up with Aspose][23]. Once you have signed up, you are ready to try all the powerful file processing features offered by Aspose.

You can easily download 'Aspose.Words for Android via Java' API for evaluation. The evaluation download is the same as the purchased download. The evaluation version simply becomes licensed when you add a few lines of code to [apply the license][24].

The evaluation version of Aspose.Words for Android via Java (without a license specified) provides full product functionality, but it inserts an evaluation watermark at the top of the document on open and save, and limits the maximum document size to several hundred paragraphs.

If you want to test 'Aspose.Words for Android via Java' API without the evaluation version limitations, you can also request a 30-day Temporary License. Please refer to [How to get a Temporary License][25]?




[1]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Android+via+Java+API+Differences+and+Limitations
[2]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+18.7+Release+Notes
[3]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Android+via+Java+18.7+Release+Notes
[4]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words/18.7
[5]: https://docs.aspose.com/display/wordsjava/Working+with+Document#WorkingwithDocument-AccessRevisionGroup
[6]: https://docs.aspose.com/display/wordsjava/Rendering#Rendering-ExportBookmarksinOutputPDF
[7]: https://docs.aspose.com/display/wordsjava/True+Type+Fonts#TrueTypeFonts-HowtoGetAvailableFontsforRendering
[8]: https://docs.aspose.com/display/wordsjava/How+to+Compare+Two+Word+Documents#HowtoCompareTwoWordDocuments-CompareWordDocumentsandIgnoreDocumentFormatting
[9]: https://docs.aspose.com/display/wordsjava/Working+with+Text+Document#WorkingwithTextDocument-HowtoHandleLeadingandTrailingSpacesduringLoadingTXT
[10]: https://docs.aspose.com/display/wordsjava/Working+with+Text+Document#WorkingwithTextDocument-HowListItemsareRecognizedDuringLoadingTXT
[11]: https://docs.aspose.com/display/wordsjava/Working+with+Document#WorkingwithDocument-RemovePersonalInformationfromDocument
[12]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+18.7+Release+Notes
[13]: https://products.aspose.com/words/android-java
[14]: https://docs.aspose.com/display/wordsjava/Home
[15]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Android+via+Java+Features
[16]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Android+via+Java+API+Differences+and+Limitations
[17]: https://products.aspose.com/words/android-java
[18]: https://docs.aspose.com/display/wordsjava/Installation#Installation-InstallAspose.WordsforAndroidviaJavafromMavenRepository
[19]: https://apireference.aspose.com/java/words
[20]: https://forum.aspose.com/c/words
[21]: https://helpdesk.aspose.com/
[22]: https://github.com/aspose-words/Aspose.Words-for-Java
[23]: https://www.aspose.com/
[24]: https://docs.aspose.com/display/wordsjava/Licensing
[25]: https://purchase.aspose.com/temporary-license




