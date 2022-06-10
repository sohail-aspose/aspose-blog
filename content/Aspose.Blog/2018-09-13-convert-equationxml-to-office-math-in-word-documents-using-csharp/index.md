---
title: 'Convert EquationXML to Office Math in Word Documents using C#'
date: Thu, 13 Sep 2018 08:02:48 +0000
draft: false
url: /2018/09/13/convert-equationxml-to-office-math-in-word-documents-using-csharp/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-net.png" alt="Aspose.Words for .NET logo">}}


We are pleased to announce our next version [Aspose.Words for .NET 18.9][1]. This month’s release contains over 73 useful new features, enhancements and bug fixes. Please check the [**release notes**][2] to get an idea about all new features, enhancements and fixes made in this release. If you are planning to upgrade from older version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][3] section to know what APIs are changed so far.

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Bookmarks are allowed on block, cell, row level
*   Added load option to treat Shapes with math XML as Shapes in the model
*   Provided option to choose between Old and New Mail Merge behaviors
*   Improved PDF encryption in case when owner password is not specified
*   Metafile rendering improved: fixed drawing records processing when path bracket is opened, fixed processing of EMR\_SETBKMODE record when incorrect values specified
*   Improved output image quality when rendering metafiles with raster operations set
*   Fixed handling of glyphs without outlines when parsing glyph data while rendering
*   Fixed a bug with a glow effect, if the specified glow size is less than 10
*   Fixed several problems in DrawingML Charts rendering: incorrect default axis color, bug with the date format for axis values, bug with rendering of the trend line with unsorted x-values
*   Improved rendering of the mathematical element "Apostrophe" of the MathML object
*   Improved justification of Asian texts
*   Improved rendering of revisions in balloons
*   Improved text placement around floating shapes
*   Fixed issue with paragraph spacing in footnotes
*   Fixed issue with line wrapping when it has single glyph wider than the line followed by page break
*   Fixed issue with table row height calculation when cells in vertical merge have horizontal borders

## Convert EquationXML to Office Math

A new proeprty LoadOptions.ConvertShapeToOfficeMath has been added in this version of Aspose.Words to convert shapes with EquationXML to Office Math objects. Please refer to the following article for more detail.

*   [Import Shapes with Math XML as Shapes into DOM][4]

```
/// <summary>
/// Gets or sets whether to convert shapes with EquationXML to Office Math objects.
/// </summary>
public bool ConvertShapeToOfficeMath
{
    get { return mConvertShapeToOfficeMath; }
    set { mConvertShapeToOfficeMath = value; }
}
```

## Bookmarks are Allowed on Block, Cell, Row Levels

Starting from Aspose.Words 18.9, the bookmarks are allowed on block, cell and row levels. We have added AnnotationsAtBlockLevel and AnnotationsAtBlockLevelAsDefault properties in LoadOptions class to work with block level bookmarks. Please read following article for more detail.

*   [Working with Bookmark on Block, Cell, Row Level][5]

```
/// <summary>
/// Gets or sets a flag indicating whether cross structure annotation nodes can be added at block/cell/row level (<see cref="Node.NodeLevel"/>).
/// </summary>
/// <remarks>
/// Currently only bookmarks are affected by this option.
/// </remarks>
public bool AnnotationsAtBlockLevel { get; set; }
 
/// <summary>
/// Gets or sets a default value for the <see cref="AnnotationsAtBlockLevel"/> property.
/// </summary>
/// <remarks>
/// Allows defining necessary behaviour when an instance of <see cref="LoadOptions"/> is not specified on opening a document.
/// </remarks>
public static bool AnnotationsAtBlockLevelAsDefault { get; set; }
```

## Switch Between Old and New Mail Merge Behaviors

We have added new property UnconditionalMergeFieldsAndRegions in MailMerge class to merge fields and merge regions regardless of the parent IF field's condition. Please refer to the following article for more detail.

*   [Switch Between Old and New Mail Merge Behaviors][6]

```
/// <summary>
/// Gets or sets a value indicating whether merge fields and merge regions are merged regardless of the parent IF field's condition.
/// </summary>
/// <remarks>
/// The default value is <b>false</b>.
/// </remarks>
public bool UnconditionalMergeFieldsAndRegions
```

## Improved PDF Encryption When Owner Password is not Specified

Previously Aspose.Words created random owner password in the produced PDF document when PdfEncryptionDetails.OwnerPassword was not set by the user.  
Starting from this release i.e. 18.9, Aspose.Words properly sets the empty owner password when saving to PDF.

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
[2]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+18.9+Release+Notes
[3]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET
[4]: https://docs.aspose.com/display/wordsnet/Use+DocumentBuilder+to+Insert+Document+Elements#UseDocumentBuildertoInsertDocumentElements-ImportShapeswithMathXMLasShapesintoDOM
[5]: https://docs.aspose.com/display/wordsnet/Working+with+Bookmarks#WorkingwithBookmarks-WorkingwithBookmarkonBlock,Cell,RowLevels
[6]: https://docs.aspose.com/display/wordsnet/How+to+Execute+Mail+Merge#HowtoExecuteMailMerge-SwitchBetweenOldandNewMailMergeBehaviors
[7]: https://products.aspose.com/words/net
[8]: https://www.nuget.org/packages/Aspose.Words/
[9]: https://docs.aspose.com/display/wordsnet
[10]: https://apireference.aspose.com/net/words
[11]: https://forum.aspose.com/c/words
[12]: https://helpdesk.aspose.com/
[13]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[14]: https://github.com/aspose-words/Aspose.Words-for-.NET




