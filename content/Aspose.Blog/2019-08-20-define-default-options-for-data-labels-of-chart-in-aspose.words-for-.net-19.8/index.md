---
title: 'Set Default Options for Data Labels of Chart in Word using C#'
date: Tue, 20 Aug 2019 17:22:34 +0000
draft: false
url: /2019/08/20/define-default-options-for-data-labels-of-chart-in-aspose.words-for-.net-19.8/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-net.png" alt="Aspose.Words for .NET logo">}}


Hi guys! We are gratified to announce the new version of [Aspose.Words for .NET i.e. 19.8][1]. Starting from this release, you can define default options for data labels of chart series. You can also work with original or revised version of Word document. let's check out how to work with these features.  

## Work with Original and Revised Version of Word Document

Revision (track change) is a way for Word document to keep track of changes you make in a document. We have added new feature in this release to work with original and revised version of a document. A new property Document.RevisionsView has been added for this feature along with RevisionsView enumeration. This property is used to get or set a value indicating whether to work with the original or revised version of a document. Following code example shows how to work with revised version of document.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Programming-Documents-Document-WorkingWithRevisions-AccessRevisedVersion.cs" >}}

## Define Default Options for Data Labels of Chart Series

You may have worked with data labels of chart series in Word document. Data Labels make a chart easier to understand as they show detail of data series or individual data points. You can add labels to chart series depending on your requirement. We have added new properties e.g. ShowSeriesName, ShowPercentage, ShowLegendKey, ShowBubbleSize, ShowCategoryName etc. in ChartDataLabelCollection class. You can use these properties to set default options for data labels. Following code example shows how to use these properties.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Programming-Documents-Charts-WorkWithChartDataLabels-DefaultOptionsForDataLabels.cs" >}}

We recommend you please check the release notes of [Aspose.Words for .NET 19.8][2] for complete detail of API changes.

When time allows you can check Aspose.Words' [API reference guide][3], [examples at Github][4], talk about this release and other API related issues in our [forum][5].




[1]: https://www.nuget.org/packages/Aspose.Words/19.8.0
[2]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+19.8+Release+Notes
[3]: https://apireference.aspose.com/net/words
[4]: https://github.com/aspose-words/Aspose.Words-for-.NET
[5]: https://forum.aspose.com/c/words




