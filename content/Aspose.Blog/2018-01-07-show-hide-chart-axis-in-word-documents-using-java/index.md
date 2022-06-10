---
title: 'Show or Hide Chart Axis in Word Documents using Java'
date: Sun, 07 Jan 2018 07:07:35 +0000
draft: false
url: /2018/01/07/show-hide-chart-axis-in-word-documents-using-java/
author: Awais Hafeez
summary: ''
tags: ['Preserve meta-characters in Word in Java', 'Show or Hide Chart Axis in Word in Java']
categories: ['Aspose.Words Product Family']
---

We are pleased to announce the new monthly release of Aspose.Words for Java 18.1. The release of this month contains a number of new features, enhancements and bug fixes of the issues reported by our users in previous versions. Please check the detailed [release notes of Aspose.Words for Java 18.1][1] to get an idea about all the new features/enhancements and fixes made in this release. Furthermore, if you are planning to upgrade the API from any previous version, we strongly recommend you to check the Public API Changes section of current release and other intermediate releases from release notes folder, to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## Show or Hide Chart Axis in Word Document

We have added a new feature in the release of Aspose.Words to show or hide the chart axis. You can use ChartAxis.Hidden property to achieve this.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-charts-WorkingWithChartAxis-HideChartAxis.java" >}}

Please refer to the following article for more detail.

*   [How to Hide Chart Axis][2]

## Preserve Meta-Characters During Replacement

We have added FindReplaceOptions.PreserveMetaCharacters property in Aspose.Words 18.1 to preserve meta-characters beginning with “&” during replacement.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-find_replace-ReplaceHtmlTextWithMeta_Characters-ReplaceHtmlTextWithMetaCharacters.java" >}}

Please check the detail and code example from the following article.

*   [How to Preserve Meta-Characters During Replacement][3]

## Enhanced Support of Single-Column Table Data Bands and Conditional Blocks for LINQ Reporting Engine

We have enhanced the support of data band inside a single-column table row for LINQ Reporting Engine. In previous versions of Aspose.Words, when opening and closing foreach tags are inside the same cell, the output contents would be in the same cell. Starting from Aspose.Words 18.1, you can export the single-column data band in a separate new row using the greedy switch. Please refer to the following article for more detail.

*   [Working with Table-Row Data Bands][4]

In this release, we have enhanced the support of conditional blocks in table’s row for LINQ Reporting Engine. If you put an opening if, elseif, or else tag and closing if the tag in the same cell, the engine treats a template option formed by these tags as a common one rather than a table-row one by default. However, you can override this behavior making the engine to treat such a template option as a table-row one by specifying a greedy switch. Please refer to the following article for more detail.

*   [Working with Table-Row Conditional Blocks][5]

## Removed Obsolete Method in CompositeNode

In this release, we have removed following obsolete public method from CompositeNode class. The parameter “isLive” is not used anymore. Please use CompositeNode.GetChildNodes(NodeType nodeType, bool isDeep) instead.

```
public NodeCollection getChildNodes(NodeType nodeType, boolean isDeep, boolean isLive)
```

## Get StoreItemID Property of StructuredDocumentTag

XmlMapping.StoreItemId property has been added in this release to specify the custom XML data identifier for the custom XML data part. Please read DataBinding class for more detail about storeItemID property.

```
/// 
/// Specifies the custom XML data identifier for the custom XML data part which
/// shall be used to evaluate the  expression.
/// 
public String StoreItemId
```

## Other Improvements

There are 63 improvements and fixes in this regular monthly release. The most notable are:

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




[1]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+18.1+Release+Notes
[2]: https://docs.aspose.com/display/wordsjava/Working+with+Charts#WorkingwithCharts-HowtoHideChartAxis
[3]: https://docs.aspose.com/display/wordsjava/Find+and+Replace#FindandReplace-HowtoPreserveMeta-CharactersDuringReplacement
[4]: https://docs.aspose.com/display/wordsjava/Working+with+Table-Row+Data+Bands
[5]: https://docs.aspose.com/display/wordsjava/Working+with+Table-Row+Conditional+Blocks
[6]: https://products.aspose.com/words/java
[7]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-words/
[8]: https://forum.aspose.com/c/words
[9]: https://helpdesk.aspose.com/
[10]: https://docs.aspose.com/display/wordsjava/Home
[11]: https://apireference.aspose.com/java/words
[12]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[13]: https://github.com/aspose-words/Aspose.Words-for-Java




