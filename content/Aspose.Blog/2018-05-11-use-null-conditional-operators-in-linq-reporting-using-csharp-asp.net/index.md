---
title: 'Use Null-Conditional Operators in LINQ Reporting using C#'
date: Fri, 11 May 2018 15:42:10 +0000
draft: false
url: /2018/05/11/use-null-conditional-operators-in-linq-reporting-using-csharp-asp.net/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-net.png" alt="Aspose.Words for .NET logo">}}


We are pleased to announce our next version [Aspose.Words for .NET 18.5][1]. This month’s release contains over 68 useful new features, enhancements and bug fixes. Please see the [release notes][2] for more detail. If you are planning to upgrade from an older version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][3] section to know what APIs are changed so far.

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Added public property StructuredDocumentTag.Color
*   Fixed line wrapping with trailing spaces at the end
*   Fixed issue with paragraph after spacing in headers/footers
*   Fixed issue with table width when widthAfter is specified for a jagged table
*   Fixed issue with table width with complex column layout and default widths
*   Fixed breaking of floating table row in compatibility mode
*   Fixed issue with floating frame pushed from the page because of invalid wrap point
*   Implemented support for "distribute space" and "distribute letter" types of alignment when rendering Ruby objects
*   Improved rendering of a Doughnut DrawingML Chart with multiple series
*   Improved rendering of DrawingML Charts data labels with the direct layout and a layout specified in the extension properties
*   Fixed a problem with metafile rendering when glyph offsets were wrongly read for EMF\_EXTTEXTOUT record with glyph indices
*   Fixed a problem with the processing of control character (U+0019) in the text when rendering
*   Fixed a problem with Adobe “Fast Find” function (words searching) in rendered PDF documents
*   Fixed a bug with inaccurate processing of EMR\_ALPHABLEND record while rendering metafiles. This bug caused a loss of fill in some figures
*   Fixed a bug with rendering of PieChart data label separator when it is set directly
*   Fixed rendering of dashed line shapes with a shadow
*   LINQ Reporting Engine supports ?. and ?\[\] null-conditional operators in template expressions

## Added Support to Change the Color of Content Control

We have added StructuredDocumentTag.Color property in this version of Aspose.Words. This property gets or sets the color of the structured document tag. Please read the following article for more detail.

*   [Change the Color of Content Control][4]

```
/// <summary>
/// Gets or sets the color of the structured document tag.
/// </summary>
public System.Drawing.Color Color
```

## Supported Null-Conditional Operators in Template Expressions for LINQ Reporting Engine

We have added a new feature in LINQ Reporting Engine to support null-conditional (A?.B) and null-coalescing (A ?? B) operators. Please read the following article for more detail.

*   [Using Operators][5]

## Obsolete Property HtmlSaveOptions.ExportMetafileAsRaster Removed

We have removed obsolete property ExportMetafileAsRaster from the HtmlSaveOptions class in Aspose.Words 18.5. Please use the HtmlSaveOptions.MetafileFormat property instead.

## Aspose.Words for .NET Resources

The following resources will help you work with Aspose.Words for .NET:

1.  [Home page of .NET API][6].
2.  [Install using NuGet Package][7]
3.  [Documentation][8] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
4.  [API Reference Guide][9] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
5.  Aspose.Words Product Family Forum – post your technical questions and queries, or any other problem you are facing while working with Aspose.Words APIs.
    *   [Free Support Forum][10]
    *   [Paid Support Forum][11]
6.  [Enable Blog Subscription][12] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
7.  [Examples][13] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.



[1]: https://www.nuget.org/packages/Aspose.Words/
[2]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+18.5+Release+Notes
[3]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET
[4]: https://docs.aspose.com/display/wordsnet/Working+with+Content+Control+SDT#WorkingwithContentControlSDT-ChangetheColorofContentControl
[5]: https://docs.aspose.com/display/wordsnet/Template+Syntax#TemplateSyntax-UsingOperators
[6]: https://products.aspose.com/words/net
[7]: https://www.nuget.org/packages/Aspose.Words/
[8]: https://docs.aspose.com/display/wordsnet
[9]: https://apireference.aspose.com/net/words
[10]: https://forum.aspose.com/c/words
[11]: https://helpdesk.aspose.com/
[12]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[13]: https://github.com/aspose-words/Aspose.Words-for-.NET




