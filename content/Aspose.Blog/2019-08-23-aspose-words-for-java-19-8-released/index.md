---
title: 'Process Original or Revised Version of Word Document using Java'
date: Fri, 23 Aug 2019 07:49:18 +0000
draft: false
url: /2019/08/23/aspose-words-for-java-19-8-released/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Following list highlights major features and you will also learn how you can use [Aspose.Words for Java 19.8][1] to:

*   Define default options for ChartDataLabels of ChartSeries
*   Access the revised version of a Document
*   Aspose.Words for Java is tested on Java 12. It works fine both on Oracle JDK 12.0.2 and OpenJDK 12.0.2.
*   Aspose.Words for Java will now use simplified TIFFImageWriter when external TIFF image libs (JAI, etc.) are not available.

## Define Default Options for ChartDataLabels of ChartSeries

The [ChartDataLabelCollection][2] class defines properties which can be used to set default options for [ChartDataLabel][3] for Chart Series. These properties include [setShowCategoryName][4], [setShowBubbleSize][5], [setShowPercentage][6], [setShowSeriesName][7], [setShowValue][8] etc. Following code example shows how to use these properties:

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-charts-DefaultOptionsForDataLabels-DefaultOptionsForDataLabels.java" >}}

Chart layout/result in output Word document will look like this:



{{< figure align=center src="images/DefaultDataLabels.png" alt="">}}


## Access Revised Version of a Document

The API now provides [RevisionsView][9] public enumeration which allows specifying whether to work with the original or revised version of a document. The document class provides [RevisionsView property][10] which can be used to get or set enumeration value. The default value is Aspose.Words.RevisionsView.Original.

The code example given below shows how to use this enumeration and access the revised version.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-TrackChanges-AccessRevisedVersion.java" >}}

## See also Useful Links

*   [Aspose.Words for Java Online Documentation][11] - up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Words for Java Product Page][12]
*   [Install Aspose.Words for Java from Maven][13]
*   [Aspose.Words for Java API Reference Guide][14] - detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Download Examples at GitHub Repository][15] - we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

Keeping the Aspose tradition, you are welcome to shape the upcoming releases of Aspose.Words for Java API by posting your suggestions and concerns in the [Aspose.Words for Java Support Forum][16].




[1]: https://downloads.aspose.com/words/java/new-releases/aspose.words-for-java-19.8/
[2]: https://apireference.aspose.com/java/words/com.aspose.words/ChartDataLabelCollection
[3]: https://apireference.aspose.com/java/words/com.aspose.words/ChartDataLabel
[4]: https://apireference.aspose.com/java/words/com.aspose.words/chartdatalabel#ShowCategoryName
[5]: https://apireference.aspose.com/java/words/com.aspose.words/chartdatalabel#ShowBubbleSize
[6]: https://apireference.aspose.com/java/words/com.aspose.words/chartdatalabel#ShowPercentage
[7]: https://apireference.aspose.com/java/words/com.aspose.words/chartdatalabel#ShowSeriesName
[8]: https://apireference.aspose.com/java/words/com.aspose.words/chartdatalabel#ShowValue
[9]: https://apireference.aspose.com/java/words/com.aspose.words/RevisionsView
[10]: https://apireference.aspose.com/java/words/com.aspose.words/document#RevisionsView
[11]: https://docs.aspose.com/display/wordsjava/Home
[12]: https://products.aspose.com/words/java
[13]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[14]: https://apireference.aspose.com/java/words
[15]: https://github.com/aspose-words/Aspose.Words-for-Java
[16]: https://forum.aspose.com/c/words




