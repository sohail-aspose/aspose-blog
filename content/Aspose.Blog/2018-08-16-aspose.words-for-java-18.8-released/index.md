---
title: 'Show Revisions in Balloons Nested LINQ Reports Java 10 Supported by Aspose.Words for Java 18.8'
date: Thu, 16 Aug 2018 01:52:53 +0000
draft: false
url: /2018/08/16/aspose.words-for-java-18.8-released/
author: Awais Hafeez
summary: ''
tags: ['Generate nested reports using Java', 'Java LINQ Reporting Engine', 'Show or hide comments in Word Java', 'Show revisions in Word document in Balloon']
categories: ['Aspose.Words Product Family']
---

We are pleased to announce the new monthly release of [**Aspose.Words for Java 18.8**][1]. The release of this month contains a number of new features, enhancements and bug fixes of the issues reported by our users in previous versions. Please check the detailed [release notes of Aspose.Words for Java 18.8][2] to get an idea about all the new features/enhancements and fixes made in this release. Furthermore, if you are planning to upgrade the API from any previous version, we strongly recommend you to check the Public API Changes section of current release and other intermediate releases from release notes folder, to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## Java 10 Supported

We have tested Aspose.Words for Java with Java 10 and are pleased to announce that Java 10 is now supported by the latest versions of Aspose.Words for Java.

## Nested Reports are Supported by LINQ Reporting Engine

You can insert the contents of outer documents to your reports dynamically using LINQ Reporting. Starting from Aspose.Words for Java 18.8, you can enable doc tag to check the template syntax and populate with data using LINQ Reporting. By default, a document being inserted is not checked against template syntax and is not populated with data. Please read the following article for more detail.  
  
[Inserting Documents Dynamically][3]

## Added Feature to Create Snip Corner Rectangle

We have added support to create snip corner rectangles in this version of Aspose.Words for Java. Please refer to the following article for more details.  
  
[Create Snip Corner Rectangle][4]

## Reference Resources in MHTML Documents using the "Content-Id" URL Scheme

We have added HtmlSaveOptions.ExportCidUrlsForMhtmlResources property in Aspose.Words 18.8. You can use this property to save the resources of MHTML document using the “Content-Id” URL Scheme. Please refer to the following article for more detail  
  
[Reference Resources in MHTML Documents using the "Content-Id" URL Scheme  
](https://docs.aspose.com/display/wordsjava/Saving+a+Document#SavingaDocument-ReferenceResourcesinMHTMLDocumentsusingthe%22Content-Id%22URLScheme)

## Show or Hide Comments in Fixed file Format

We have added new property ShowComments in LayoutOptions class. This property is used to show or hide comments in fixed file formats e.g. PDF, XPS. By default, the comments are visible. Please read following article.  
  
[Working with Layout Options][5]

## Show Revisions in Balloons

A new property ShowInBalloons has been added to RevisionOptions class. This property is used to show revisions in the balloons. By default, the revisions in balloons are not shown. Please refer to the following article.  
  
[Working with Layout Options][6]

## Write all CSS Declarations of HtmlFixed Documents into Single File

Previously, Aspose.Words used to save “@font-face” rules of HtmlFixed documents into a separate file “fontFaces.css” while other CSS declarations were written to “styles.css”. We have changed this behavior and now Aspose.Words saves all CSS rules and declarations into the same file “styles.css”. In case the old behavior is required for compatibility with legacy code, it can be restored by using the new public property HtmlFixedSaveOptions.SaveFontFaceCssSeparately. Please read following article.  
  
[Write all CSS Declarations of HtmlFixed Document into Single File][7]

## Detect UTF8 Text While Loading RTF

We have added new property RecognizeUtf8Text in RtfLoadOptions class. This property allows to detect UTF-8 encoded characters and preserve them during import. Please read following article.  
  
[Detect UTF8 Text While Loading RTF][8]

## Obsolete Member NumInDash was Removed from NumberStyle Enum

Obsolete value NumInDash was removed from NumberStyle enum. Please, use NumberStyle.NumberInDash value instead.

## Obsolete Method ToTxt() was Removed from Node Class

Obsolete method ToTxt() was removed from Node class. Please, use ToString(SaveFormat.Text) instead.

## Obsolete Property Location was Removed from FootnoteOptions and EndnoteOptions Classes

The obsolete property Location has been removed from the FootnoteOptions and EndnoteOptions classes. Please use the Position property. Also, the FootnoteLocation emum type has been removed.

## Obsolete Property WarningCallback was Removed from SaveOptions Class

Obsolete property WarningCallback was removed from SaveOptions class. Please, use the Document.WarningCallback property instead.

## Other Improvements

There are 86 improvements and fixes in this regular monthly release. The most notable are:

*   Java 10 tested and supported now
*   New and updated Samples and Examples
*   Change SHA-1 to SHA-256 and public asymmetric key from 1024 to 2048 for the license mechanism
*   Implemented support for “underline trailing spaces” compatibility option
*   Implemented support for paragraph alignment in Omath when inserted using EQ fields
*   Enhanced computation of interscript spacing values based on TTF properties
*   Improved wrapping of text around floating objects
*   Improved calculation of position of floating tables and shapes
*   Improved floater overlapping logic
*   Improved computing of pages numbers in continuous sections which have restart attribute and conflicting oddity
*   Fixed line justification issue when RTL span is at the end of the line
*   Fixed issue with null dml properties
*   Fixed issue with rendering of floating shapes in truncated headers/footers
*   Fixed issue with rendering of lines inside of a field result when updated in truncated part of a cell
*   Improved rendering of math operators in MathML objects
*   Improved rendering of MathML objects with n-ary math element when n-ary character and limit location are not specified
*   Fixed a bug with rendering of a math n-ary element if it is part of a fraction
*   Fixed a bug when polyline with an arrow and a very small line segment at the end 
*   was corrupted upon rendering
*   Fixed a bug when an arrow pointer is incorrectly directed while rendering Bezier curves with arrows
*   Fixed a bug where the end of the line was outside the "stealth arrow" when rendering
*   LINQ Reporting Engine supports nested reports

## Aspose.Words for Java Resources

The following resources will help you work with Aspose.Words for Java:

*   [Home page for Aspose.Words for Java][9]
*   [Install Aspose.Words for Java from Maven][10]
*   Words product family forum – Post your technical questions and queries, or any other problem you faced while running Aspose.Words APIs.
    *   [Free Support Forum][11]
    *   [Paid Support Forum][12]
*   [Aspose.Words for Java online documentation][13]– Help documentation.
*   [Aspose.Words for Java online API reference][14]– API reference documents.
*   [Enable Blog Subscription][15]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words, APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
*   [Aspose.Words for Java Examples][16] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[2]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+18.8+Release+Notes
[3]: https://docs.aspose.com/display/wordsjava/Inserting+Documents+Dynamically
[4]: https://docs.aspose.com/display/wordsjava/Use+DocumentBuilder+to+Insert+Document+Elements#UseDocumentBuildertoInsertDocumentElements-CreateSnipCornerRectangle
[5]: https://docs.aspose.com/display/wordsjava/Rendering#Rendering-WorkingwithLayoutOptions
[6]: https://docs.aspose.com/display/wordsjava/Rendering#Rendering-WorkingwithLayoutOptions
[7]: https://docs.aspose.com/display/wordsjava/Saving+a+Document#SavingaDocument-WriteallCSSDeclarationsofHtmlFixedDocumentintoSingleFile
[8]: https://docs.aspose.com/display/wordsjava/Creating+or+Loading+a+Document#CreatingorLoadingaDocument-DetectUTF8TextWhileLoadingRTF
[9]: https://products.aspose.com/words/java
[10]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[11]: https://forum.aspose.com/c/words
[12]: https://helpdesk.aspose.com/
[13]: https://docs.aspose.com/display/wordsjava/Home
[14]: https://apireference.aspose.com/java/words
[15]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[16]: https://github.com/aspose-words/Aspose.Words-for-Java




