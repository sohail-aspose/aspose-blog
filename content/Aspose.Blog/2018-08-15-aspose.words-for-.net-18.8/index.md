---
title: 'Snip Corner Rectangle Nested Reports by LINQ Reporting Engine'
date: Wed, 15 Aug 2018 16:58:53 +0000
draft: false
url: /2018/08/15/aspose.words-for-.net-18.8/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-net.png" alt="Aspose.Words for .NET logo">}}


We are pleased to announce our next version [Aspose.Words for .NET 18.8][1]. This month’s release contains over 81 useful new features, enhancements, and bug fixes. Please check the release notes to get an idea about all new features, enhancements, and fixes made in this release. If you are planning to upgrade from an older version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][2] section to know what APIs are changed so far.

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Implemented support for “underline trailing spaces” compatibility option
*   Implemented support for paragraph alignment in Omath when inserted using EQ fields
*   Enhanced computation of interscript spacing values based on TTF properties
*   Improved wrapping of text around floating objects
*   Improved calculation of position of floating tables and shapes
*   Improved floater overlapping logic
*   Improved computing of pages numbers in continuous sections which have restart attribute and conflicting oddity
*   Fixed line justification issue when RTL span is at the end of the line
*   Fixed issue with null dml properties
*   Fixed issue with rendering of floating shapes in truncated headers/footers
*   Fixed issue with rendering of lines inside of a field result when updated in truncated part of a cell
*   Improved rendering of math operators in MathML objects
*   Improved rendering of MathML objects with n-ary math element when n-ary character and limit location are not specified
*   Fixed a bug with rendering of a math n-ary element if it is part of a fraction
*   Fixed a bug when polyline with an arrow and a very small line segment at the end
*   Fixed a bug when an arrow pointer is incorrectly directed while rendering Bezier curves with arrows
*   Fixed a bug where the end of the line was outside the "stealth arrow" when rendering
*   LINQ Reporting Engine supports nested reports

## Support of Nested Reports By LINQ Reporting Engine

You can insert contents of outer documents to your reports dynamically using LINQ Reporting. Starting from Aspose.Words 18.8, you can enable _doc_ tag to check the template syntax and populate with data uisng LINQ Reporting. By default, a document being inserted is not checked against template syntax and is not populated with data. Please read following article for more detail.

[Inserting Documents Dynamically][3]

## Added Feature to Create Snip Corner Rectangle

We have added support to create snip corner rectangles in this version of Aspose.Wrods. The following shape types have been added to the "ShapeType" enumeration. Please refer to the following article for more detail.

[Create Snip Corner Rectangle][4]

```
/// Snip single corner rectangle object.
/// </summary>
/// <remarks>
/// Applicable only for DML shapes.
/// </remarks>
SingleCornerSnipped = 203,
/// <summary>
/// Snip same side corner rectangle.
/// </summary>
/// <remarks>
/// Applicable only for DML shapes.
/// </remarks>
TopCornersSnipped = 204,
/// <summary>
/// Snip diagonal corner rectangle.
/// </summary>
/// <remarks>
/// Applicable only for DML shapes.
/// </remarks>
DiagonalCornersSnipped = 205,
/// <summary>
/// Snip and round single corner rectangle.
/// </summary>
/// <remarks>
/// Applicable only for DML shapes.
/// </remarks>
TopCornersOneRoundedOneSnipped = 206,
/// <summary>
/// Round single corner rectangle.
/// </summary>
/// <remarks>
/// Applicable only for DML shapes.
/// </remarks>
SingleCornerRounded = 207,
/// <summary>
/// Round same side corner rectangle.
/// </summary>
/// <remarks>
/// Applicable only for DML shapes.
/// </remarks>
TopCornersRounded = 208,
/// <summary>
/// Round diagonal corner rectangle.
/// </summary>
/// <remarks>
/// Applicable only for DML shapes.
/// </remarks>
DiagonalCornersRounded = 209
```

## Support of Reference Resources in MHTML Document

We have added HtmlSaveOptions.ExportCidUrlsForMhtmlResources property in Aspose.Words 18.8. You can use this property to save the resources of MHTML document using the "Content-Id" URL Scheme. Please refer to the following article for more detail.

[Add Reference Resources in MHTML Documents using the "Content-Id" URL Scheme][5]

## Added Feature to Show or Hide Comments in Fixed file Format

We have added new property ShowComments in LayoutOptions class. This property is used to show or hide comments in fixed file formats e.g. PDF, XPS. By default, the comments are visible. Please read following article.

[Working with Layout Options][6]

## Added Feature to Show Revisions in Balloons

A new property ShowInBalloons has been added to RevisionOptions class. This property is used to show revisions in the balloons. By default, the revisions in balloons are not shown. Please refer to the following article.

[Working with Layout Options][7]

```
/// <summary>
/// Allows to specify whether the revisions are rendered in the balloons.
/// Default value for this property is <see cref="Layout.ShowInBalloons.None"/>
/// </summary>
public ShowInBalloons ShowInBalloons
{
      get; set;
 
}
```
```
/// <summary>
/// Specifies which revisions are rendered in balloons.
/// </summary>
/// <remarks>
/// Note that these values do not affect rendering of comments, which are controlled by <see cref="LayoutOptions.ShowComments"/>.
/// </remarks>
public enum ShowInBalloons
{
     /// <summary>
     /// Renders insert, delete and format revisions inline.
     /// </summary>
     None,
     /// <summary>
     /// Renders insert and delete revisions inline, format revisions in balloons.
     /// </summary>
     Format,
     /// <summary>
     /// Renders insert revisions inline, delete and format revisions in balloons.
     /// </summary>
     FormatAndDelete,
}
```

## Write all CSS Declarations of HtmlFixed Documents into Single File

Previously, Aspose.Words saved "@font-face" rules of HtmlFixed documents into a separate file "fontFaces.css" while other CSS declarations were written to "styles.css". We have changed this behavior and now Aspose.Words saves all CSS rules and declarations into the same file "styles.css". In case the old behavior is required for compatibility with legacy code, it can be restored by using the new public property HtmlFixedSaveOptions.SaveFontFaceCssSeparately. Please read following article.

[Write all CSS Declarations of HtmlFixed Document into Single File][8]

## Detect UTF8 Text While Loading RTF

We have added new property RecognizeUtf8Text in RtfLoadOptions class. This property allows to detect UTF-8 encoded characters and preserve them during import. Please read following article.

[Detect UTF8 Text While Loading RTF  
](https://docs.aspose.com/display/wordsnet/Creating+or+Loading+a+Document#CreatingorLoadingaDocument-DetectUTF8TextWhileLoadingRTF)

```
/// <summary>
/// <para> When set to true, <see cref="CharsetDetector"/> will try to detect UTF8 characters,
/// they will be preserved during import.
/// </para>
/// Default value is false.
/// </summary>
public bool RecognizeUtf8Text
```

## Obsolete Member NumInDash was Removed from NumberStyle Enum

Obsolete value NumInDash was removed from NumberStyle enum. Please use NumberStyle.NumberInDash value instead.

## Obsolete Method ToTxt() was Removed from Node Class

Obsolete method ToTxt() was removed from Node class. Please use ToString(SaveFormat.Text) instead.

## Obsolete Property Location was Removed from FootnoteOptions and EndnoteOptions Classes

The obsolete property Location has been removed from the FootnoteOptions and EndnoteOptions classes. Please use the Position property. Also, the FootnoteLocation emum type has been removed.

## Obsolete Property WarningCallback was Removed from SaveOptions Class

Obsolete property WarningCallback was removed from SaveOptions class. Please, use the Document.WarningCallback property instead.

## Aspose.Words for .NET Resources

The following resources will help you work with Aspose.Words for .NET:

1.  [Home page of .NET API][9].
2.  [Install using NuGet Package][10]
3.  [Documentation][11] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
4.  [API Reference Guide][12] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
5.  Aspose.Words Product Family Forum – post your technical questions and queries, or any other problem you are facing while working with Aspose.Words APIs.
    *   [Free Support Forum][13]
    *   [Paid Support Forum][14]
6.  [Enable Blog Subscription][15] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
7.  [Examples][16] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Words/
[2]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET
[3]: https://docs.aspose.com/display/wordsnet/Template+Syntax#TemplateSyntax-InsertingDocumentsDynamically
[4]: https://docs.aspose.com/display/wordsnet/Use+DocumentBuilder+to+Insert+Document+Elements#UseDocumentBuildertoInsertDocumentElements-CreateSnipCornerRectangle
[5]: https://docs.aspose.com/display/wordsnet/Saving+a+Document#SavingaDocument-AddReferenceResourcesinMHTMLDocumentsusingthe%22Content-Id%22URLScheme
[6]: https://docs.aspose.com/display/wordsnet/Rendering#Rendering-WorkingwithLayoutOptions
[7]: https://docs.aspose.com/display/wordsnet/Rendering#Rendering-WorkingwithLayoutOptions
[8]: https://docs.aspose.com/display/wordsnet/Saving+a+Document#SavingaDocument-WriteallCSSDeclarationsofHtmlFixedDocumentintoSingleFile
[9]: https://products.aspose.com/words/net
[10]: https://www.nuget.org/packages/Aspose.Words/
[11]: https://docs.aspose.com/display/wordsnet
[12]: https://apireference.aspose.com/net/words
[13]: https://forum.aspose.com/c/words
[14]: https://helpdesk.aspose.com/
[15]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[16]: https://github.com/aspose-words/Aspose.Words-for-.NET




