---
title: 'Dynamic Chart Series and Individual Series Points Coloring in Java LINQ Reporting Engine'
date: Thu, 15 Mar 2018 09:06:03 +0000
draft: false
url: /2018/03/15/aspose.words-for-java-18.3-released/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

We are pleased to announce the new monthly release of [**Aspose.Words for Java 18.3**][1]. The release of this month contains number of new features, enhancements and bug fixes of the issues reported by our users in previous versions. Please check the detailed [release notes of Aspose.Words for Java 18.3][2] to get an idea about all the new features/enhancements and fixes made in this release. Furthermore, if you are planning to upgrade the API from any previous version, we strongly recommend you to check the Public API Changes section of current release and other intermediate releases from release notes folder, to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## Set Chart Series Color and Individual Series Points using LINQ Reporting Engine

In this version of Aspose.Words fo Java, we have added the support to set the color of chart series and individual series points using LINQ Reporting Engine. Please read following article for more detail.  
[Using Charts to Represent Sequential Data][3]

## PdfSaveOptions.EscapeUri Property Added

In some cases, user wants to encode the URI e.g. encode "/" character to the "%2F". Starting from Aspose.Words for Java 18.3, we have added support to escape the URI before writing it into PDF. Please refer to the following article for more detail:  
[Escape the URI in Output PDF][4]

## HtmlSaveOptions.CssClassNamePrefix Property Added

We have added new feature in this release to add prefix to all CSS class names when document is exported to HTML. A new property HtmlSaveOptions.CssClassNamePrefix has been added in Aspose.Words 18.3. Please read following article for more detail.  
[Add Prefix to CSS Class Name][5]  

## Obsolete Properties and Methods were Removed from Aspose.Words API

*   Obsolete method FormFieldCollection.Remove was removed. Please use the FormField.RemoveField method instead.
*   Obsolete property MailMerge.RemoveEmptyParagraphs was removed. Please use the MailMerge.CleanupOptions property instead.
*   Obsolete property MailMerge.RemoveEmptyRegions was removed. Please use the MailMerge.CleanupOptions property instead.
*   Obsolete property MailMerge.RtlCleanupMode was removed.
*   Obsolete value GeneralFormat.Auieo was removed. Please use the GeneralFormat.Aiueo value instead.

## Obsolete Properties Removed from PdfSaveOptions

Following obsolete properties were removed from the PdfSaveOptions class:

<figure class="wp-block-table"><table class=""><tbody><tr><td>**Removed property</strong></td><td><strong>Property to use instead**</td></tr><tr><td>HeadingsOutlineLevels</td><td>OutlineOptions.HeadingsOutlineLevels</td></tr><tr><td>ExpandedOutlineLevels</td><td>OutlineOptions.ExpandedOutlineLevels</td></tr><tr><td>BookmarksOutlineLevel</td><td>OutlineOptions.DefaultBookmarksOutlineLevel</td></tr><tr><td>EmbedStandardWindowsFonts</td><td>FontEmbeddingMode</td></tr><tr><td>ExportCustomPropertiesAsMetadata</td><td>CustomPropertiesExport</td></tr><tr><td>MetafileRenderingMode</td><td>MetafileRenderingOptions.RenderingMode</td></tr><tr><td>DownsampleImages</td><td>DownsampleOptions.DownsampleImages</td></tr><tr><td>DownsampleResolution</td><td>DownsampleOptions.Resolution</td></tr></tbody></table></figure>

## Other Improvements

There are 71 improvements and fixes in this regular monthly release. The most notable are:

*   Public API to get Subject and Issuer names from DigitalCertificate (instead obsolete properties).
*   Add support of CssClassNamesPrefix in HtmlSaveOptions
*   A number of obsolete properties were removed from PdfSaveOptions class. Please refer to public API changes section for details
*   PdfSaveOptions.EscapeUri property was added to allow the usage of custom URI strings without the automatic escape while rendering into PDF
*   The automatic font color calculation now takes the fill of the background shape into account while rendering
*   Added fallback rendering for Unicode range \[U+1F300; U+1F5FF\] - Miscellaneous Symbols and Pictographs; This range includes such symbols as Emoji and alike
*   Implemented processing of empty EMR\_EXTTEXTOUTW records in metafiles rendering
*   Improved rendering of DML Chart plot area with a manual layout. The additional offset is calculated for the rotated labels of horizontal axis
*   Fixed a bug where the gradient brush with transformation would mess up the texture upon rendering. Texture scaling improved
*   Fixed a problem of axis scaling when rendering DML Charts with Arial Narrow font
*   Fixed a bug causing freezes when converting to PDF a document with DML Charts with a huge number of data points
*   Fixed a symbol positioning bug when rendering MathML equations
*   A reflection effect is now applied correctly for 3D rotated WordArt objects

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
[2]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+18.3+Release+Notes
[3]: https://docs.aspose.com/display/wordsjava/Using+Charts+to+Represent+Sequential+Data
[4]: https://docs.aspose.com/display/wordsjava/Rendering#Rendering-EscapetheURIinOutputPDF
[5]: https://docs.aspose.com/display/wordsjava/Saving+a+Document#SavingaDocument-AddPrefixtoCSSClassName
[6]: https://products.aspose.com/words/java
[7]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-words/
[8]: https://forum.aspose.com/c/words
[9]: https://helpdesk.aspose.com/
[10]: https://docs.aspose.com/display/wordsjava/Home
[11]: https://apireference.aspose.com/java/words
[12]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[13]: https://github.com/aspose-words/Aspose.Words-for-Java




