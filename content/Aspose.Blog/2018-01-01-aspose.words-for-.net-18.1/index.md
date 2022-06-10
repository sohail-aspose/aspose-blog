---
title: 'Support of Single-Column Table Data Bands and Conditional Blocks for LINQ Reporting Engine'
date: Mon, 01 Jan 2018 13:58:33 +0000
draft: false
url: /2018/01/01/aspose.words-for-.net-18.1/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-net.png" alt="Aspose.Words for .NET logo">}}


We are pleased to announce our next version [Aspose.Words for .NET 18.1][1]. This month’s release contains over 61 useful new features, enhancements and bug fixes. Please see the [release notes][2] for more detail. If you are planning to upgrade from an older version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][3] section to know what APIs are changed so far.

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Signing of PDF document is supported in .NET Standard 2.0.
*   Saving to BMP is supported in .NET Standard 2.0.
*   Improved rendering of Path gradients in .NET Standard 2.0/Xamarin.
*   Improved character spacing control logic.
*   Improved space shrinking for Verdana font.
*   Improved "allow handing punctuation" handling when kerning is enabled.
*   Fixed clip issue with semi-broken tables.
*   Fixed draw order of wrapped shapes in 2013 mode.
*   Fixed repeated header height problem during field update.
*   Fixed the bug causing error in page numbers in multi-page documents rendered into PostScript.
*   Proper calculation of undocumented margins in DrawingML Charts implemented.
*   Horizontal axis of Bubble Chart scaling fixed.
*   Vertical axis of 3DArea Chart scaling fixed.
*   MS Word 2016 approach for rendering of DrawingML Charts axis labels implemented; (Labels are rotated to fit the chart).
*   Fixed rendering of Legend markers for 3D-LineChart.
*   Improved rendering of composite (with multiple series) charts.
*   Chart title with ManualLayout rendering fixed.

## Enhanced Support of Single-Column Table Data Bands and Conditional Blocks for LINQ Reporting Engine

We have enhanced the support of data band inside a single-column table row for LINQ Reporting Engine. In previous versions of Aspose.Words, when opening and closing foreach tags are inside the same cell, the output contents would be in the same cell. Starting from Aspose.Words 18.1, you can export the single-column data band in a separate new row using _greedy_ switch. Please refer to the following article for more detail.  
[Working with Table-Row Data Bands][4]

In this release, we have enhanced the support of conditional blocks in the table's row for LINQ Reporting Engine. If you put an opening if, elseif, or else tag and closing _if_ tag in the same cell, the engine treats a template option formed by these tags as a common one rather than a table-row one by default. However, you can override this behavior making the engine to treat such a template option as a table-row one by specifying a _greedy_ switch. Please refer to the following article for more detail.  
[Working with Table-Row Conditional Blocks][5]

## Preserve Meta-Characters During Replacement

We have added FindReplaceOptions.PreserveMetaCharacters property in Aspose.Words 18.1 to preserve meta-characters beginning with "&" during replacement. Please check the detail and code example from following article.  
[How to Preserve Meta-Characters During Replacement][6]

```
/// <summary>
/// True indicates that meta-characters beginning with "&" are preserved.
/// Default value is false.
/// </summary>
public bool PreserveMetaCharacters
```

## Removed Obsolete Method in CompositeNode

In this release, we have removed the following obsolete public method from CompositeNode class. The parameter "isLive" is not used anymore. Please use CompositeNode.GetChildNodes(NodeType nodeType, bool isDeep) instead.

```
public NodeCollection GetChildNodes(NodeType nodeType, bool isDeep, bool isLive)
```

## Show or Hide Chart Axis

We have added a new feature in the release of Aspose.Words to show or hide the chart axis. You can use ChartAxis.Hidden property to achieve this. Please refer to the following article for more detail.  
[How to Hide Chart Axis][7]

```
/// <summary>
/// Gets or sets a flag indicating whether this axis is hidden or not.
/// </summary>
/// <remarks>
/// Default value is false.
/// </remarks>
public bool Hidden
{
    get; set;
}
```

## Get StoreItemID Property of StructuredDocumentTag

XmlMapping.StoreItemId property has been added in this release to specify the custom XML data identifier for the custom XML data part. Please read [DataBinding][8].aspx) class for more detail about storeItemID property.

```
/// <summary>
/// Specifies the custom XML data identifier for the custom XML data part which
/// shall be used to evaluate the <see cref="XPath"/> expression.
/// </summary>
public string StoreItemId
```

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
[2]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+18.1+Release+Notes
[3]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET
[4]: https://docs.aspose.com/display/wordsnet/Template+Syntax#TemplateSyntax-WorkingwithTable-RowDataBands
[5]: https://docs.aspose.com/display/wordsnet/Template+Syntax#TemplateSyntax-WorkingwithTable-RowConditionalBlocks
[6]: https://docs.aspose.com/display/wordsnet/Find+and+Replace#FindandReplace-HowtoPreserveMeta-CharactersDuringReplacement
[7]: https://docs.aspose.com/display/wordsnet/Working+with+Charts#WorkingwithCharts-HowtoHideChartAxis
[8]: https://msdn.microsoft.com/en-us/library/documentformat.openxml.wordprocessing.databinding(v=office.14
[9]: https://products.aspose.com/words/net
[10]: https://www.nuget.org/packages/Aspose.Words/
[11]: https://docs.aspose.com/display/wordsnet
[12]: https://apireference.aspose.com/net/words
[13]: https://forum.aspose.com/c/words
[14]: https://helpdesk.aspose.com/
[15]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[16]: https://github.com/aspose-words/Aspose.Words-for-.NET




