---
title: 'Insert Hyperlink in Word Documents using Java LINQ Reporting Engine'
date: Tue, 19 Jun 2018 12:12:20 +0000
draft: false
url: /2018/06/19/aspose.words-for-java-18.6-released/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

We are pleased to announce the new monthly release of [**Aspose.Words for Java 18.6**][1]. The release of this month contains number of new features, enhancements and bug fixes of the issues reported by our users in previous versions. Please check the detailed [release notes of Aspose.Words for Java 18.6][2] to get an idea about all the new features/enhancements and fixes made in this release. Furthermore, if you are planning to upgrade the API from any previous version, we strongly recommend you to check the Public API Changes section of current release and other intermediate releases from release notes folder, to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## Insert Hyperlink Dynamically in Word Documents using Java

A new feature has been introduced in this version of Aspose.Words to insert hyperlink dynamically using LINQ Reporting engine. Please read the following article for more detail.

*   [Inserting Hyperlinks Dynamically][3]

## Title and Description Properties for Table Class

Starting from Aspose.Words 18.6, you can set the alternative text of the table. We have added Title and Description properties into Table class. Please refer to the following article for more detail.

*   [Working with Alternative Text of Table][4]

## Insert Shapes through DocumentBuilder using ShapeType

We have added the following methods in DocumentBuilder class to insert inline and free-floating shapes. These methods allow inserting DML shape into the document model. For more detail, please read the following article.

*   [Inserting Inline and Free-floating Shapes][5]

## Changed Public Properties of AxisScaling Class

We have removed MinimumIsAuto and MaximumIsAuto properties from the AxisScaling class. The type of the Minimum and Maximum properties has been changed from double to AxisBound. A new class AxisBound has been added in latest API that allows specifying axis bound as a numeric, DateTime or “auto” value. Please check the code examples from following article

*   [How to Set Chart Axis Properties][6]

## Setup Language Preferences

The LanguagePreferences class has been added for this feature. We have added a new feature in this release to setup language preferences. In MS Word, you can setup it from 'Set the Office Language Preferences' dialog. Please read the following article for more detail.

*   [Allowing to Setup Language Preferences][7]

## Move From and Move To Revisions

We have added following public properties into the Inline, Paragraph, ShapeBase and InlineStory classes to work with ‘move from’ and ‘move to ‘ revisions. For more detail, please read the following article.

*   [Programmatically Access Revisions][8]

## Line Break Options for Asian Typography

In this release, we have added support of line break options for Asian Typography. The following public properties have been added into the ParagraphFormat class. Please read the following article for more detail.

*   [Set Line Break Options][9]

## "Add bi-directional marks" for TXT Format

We have added TxtSaveOptions.AddBidiMarks property in this version of Aspose.Words to support the insertion of bi-directional marks in output TXT file format. Please read the following article for more detail.

*   [How to Add Bi-Directional Marks][10]

## Obsolete Enum RowAlignment was Removed

Obsolete enum RowAlignment was Removed from API. Please use TableAlignment enum instead.

## Obsolete Methods

Obsolete method InvalidateFieldTypes was removed from Document and Range classes. Please use NormalizeFieldTypes method instead.

## Obsolete Properties

Obsolete property RowFormat.PreferredWidth was removed. Please use the Table.PreferredWidth property instead.  
Obsolete property RowFormat.RowAlignment was removed. Please use the Table.RowAlignment property instead.  
Obsolete property RowFormat.AllowAutoFit was removed. Please use the Table.AllowAutoFit property instead.  
Obsolete property RowFormat.Bidi was removed. Please use the Table.Bidi property instead.  
Obsolete properties RowFormat.LeftPadding/RightPadding/TopPadding/BottomPadding was removed. Please use these properties from Table class instead.  
Obsolete property RowFormat.CellSpacing was removed. Please use the Table.CellSpacing property instead.  
Obsolete property RowFormat.LeftIndent was removed. Please use the Table.LeftIndent property instead.  
Obsolete method RowFormat.ClearCellPadding() was removed. Please use padding properties on the Table instead.

## Other Improvements

There are 66 improvements and fixes in this regular monthly release. The most notable are:

*   Exposed Title and Description properties into Table class
*   Added feature to insert shapes through the DocumentBuilder using ShapeType
*   Changed public properties of AxisScaling class
*   Implemented API allowing to set up language preferences
*   Added IsMoveFromRevision and IsMoveToRevision properties
*   Exposed properties for Asian typography into ParagraphFormat class
*   Public TXT save option AddBidiMarks is added
*   Implemented "left" and "right" alignment support for Ruby objects rendering
*   Improved rendering of DrawingML chart data labels with percentage values and the specified format
*   Flat shapes that are perpendicular to the projection plane are not rendered now
*   Zero-width characters in DrawingML textboxes no longer cause an exception during rendering
*   Fixed an issue with font fallback rendering for 1F600 - 1F64F (Emoticons) Unicode range
*   Fixed a bug with the rendering of the chart data labels, when label text and SpPr are specified
*   Fixed a bug with the maximum value of the chart axis when rendering DrawingML charts
*   Fixed a problem with rendering of subscript and superscript text in DrawingML charts
*   Fixed a bug where the shadowed shapes with compound outline lost their fill
*   Fixed MathML alignment issue inside text boxes
*   Fixed layout when large inline shape is attached to a paragraph with space after overflowing page
*   Fixed issue with preferred width of vertically merged table cells accounted for during width computation
*   Fixed exception when revision balloons are displayed in certain cases
*   Enhanced logic which handles page breaks inside text frames
*   LINQ Reporting Engine supports dynamic insertion of hyperlinks

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
[2]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+18.6+Release+Notes
[3]: https://docs.aspose.com/display/wordsjava/Inserting+Hyperlinks+Dynamically
[4]: https://docs.aspose.com/display/wordsjava/Applying+Formatting+to+Table%2C+Row+and+Cell#ApplyingFormattingtoTable,RowandCell-WorkingwithAlternativeTextofTable
[5]: https://docs.aspose.com/display/wordsjava/Use+DocumentBuilder+to+Insert+Document+Elements#UseDocumentBuildertoInsertDocumentElements-InsertingInlineandFree-floatingShapes
[6]: https://docs.aspose.com/display/wordsjava/Working+with+Charts#WorkingwithCharts-HowtoSetChartAxisProperties
[7]: https://docs.aspose.com/display/wordsjava/Working+with+Document#WorkingwithDocument-AllowingtoSetupLanguagePreferences
[8]: https://docs.aspose.com/display/wordsjava/Working+with+Document#WorkingwithDocument-ProgrammaticallyAccessRevisions
[9]: https://docs.aspose.com/display/wordsjava/Using+DocumentBuilder+to+Modify+a+Document#UsingDocumentBuildertoModifyaDocument-SetLineBreakOptions
[10]: https://docs.aspose.com/display/wordsjava/Saving+a+Document#SavingaDocument-HowtoAddBi-DirectionalMarks
[11]: https://products.aspose.com/words/java
[12]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[13]: https://forum.aspose.com/c/words
[14]: https://helpdesk.aspose.com/
[15]: https://docs.aspose.com/display/wordsjava/Home
[16]: https://apireference.aspose.com/java/words
[17]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[18]: https://github.com/aspose-words/Aspose.Words-for-Java




