---
title: 'Extract Text from PowerPoint Files using Java'
seoTitle: "Extract Text From PowerPoint PPTX/PPT in Java | Extract Text from Slides"
description: "Use Java PowerPoint API to extract text from PowerPoint PPTX/PPT presentations in Java. Extract text from a specific slide of from the whole presentation."
date: Wed, 28 Jul 2021 05:47:00 +0000
draft: false
url: /2021/07/28/extract-text-from-powerpoint-files-using-java/
author: Usman Aziz
summary: 'You may often need to extract text from the PowerPoint slides in order to perform text analysis. On the other hand, you may want to extract and save the text in a file or database for further processing. In accordance with that, this article covers **how to extract text from PowerPoint presentations using Java**. Particularly, you will learn how to extract text from a specific slide or whole presentation.'
tags: ['Extract Text from a PowerPoint Presentation Java', 'Extract Text from a PowerPoint Slide Java', 'Java API to Extract Text from PowerPoint PPTX']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Extract-Text-from-PowerPoint.jpg" alt="Extract Text from PowerPoint Java">}}


You may often need to extract text from the PowerPoint slides in order to perform text analysis. On the other hand, you may want to extract and save the text in a file or database for further processing. In accordance with that, this article covers **how to extract text from PowerPoint presentations using Java**. Particularly, you will learn how to extract text from a specific slide or whole presentation.

*   [API to Extract Text from PowerPoint PPTX][1]
*   [Extract Text from a PowerPoint Slide][2]
*   [Extract Text from a PowerPoint Presentation][3]

## Java API to Extract Text from PowerPoint PPTX {#Java-API-to-Extract-Text-From-PowerPoint-PPTX}

In order to manipulate PowerPoint presentations, Aspose offers [Aspose.Slides for Java][4]. The said API is designed to implement PowerPoint automation features in Java applications. It also provides some simple ways of extracting text from the PPT/PPTX presentations. You can either [download][5] the API or install it using the following Maven configurations.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-slides</artifactId>
    <version>21.7</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Extract Text from a PowerPoint Slide in Java {#Extract-Text-from-a-PowerPoint-Slide-in-Java}

The following are the steps to extract text from a slide in a PowerPoint presentation using Java.

*   Load the presentation using [Presentation][6] class.
*   Get all the text frames from a slide into [ITextFrame][7] array using [SlideUtil.getAllTextBoxes()][8] method.
*   Loop through each _ITextFrame_ and access its text using [ITextFrame.getParagraphs()][9] method.
*   Retrieve and print text from each [IPortion][10] of the paragraph.

The following code sample shows how to extract text from a PowerPoint slide.

{{< gist aspose-com-gists 14f529c17523ba866f7c984424a22d77 "extract-text-from-slide.java" >}}

## Extract Text from Whole PowerPoint Presentation {#Extract-Text-from-PowerPoint-Presentation-in-Java}

You can also extract text from the whole PowerPoint presentation. The following are the steps to perform this operation.

*   Load the presentation using [Presentation][11] class.
*   Get all the text frames in presentation using [SlideUtil.getAllTextFrames()][12] method.
*   Loop through each [ITextFrame][13] and access its paragraphs.
*   Access the portions of the paragraphs and print their text.

The following code sample shows how to extract text from a PowerPoint presentation.

{{< gist aspose-com-gists 14f529c17523ba866f7c984424a22d77 "extract-text-from-presentation.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

In case you want to use the API without evaluation limitations, you can [get a free temporary license][14].

## Try Online

You may also try the free online presentation parser, which is developed using Aspose.Slides.

*   [Online Text Extractor from PowerPoint][15]

## Conclusion

In this article, you have learned how to extract text from PowerPoint presentations using Java. The code samples have shown how to extract text from a specific slide or the whole presentation. You can explore more about Aspose.Slides for Java using [documentation][16]. In case you would have any queries, inform us via our [forum][17].

## See Also

*   [Create PowerPoint Presentations in Java][18]




[1]: #Java-API-to-Extract-Text-From-PowerPoint-PPTX
[2]: #Extract-Text-from-a-PowerPoint-Slide-in-Java
[3]: #Extract-Text-from-PowerPoint-Presentation-in-Java
[4]: https://products.aspose.com/slides/java
[5]: https://downloads.aspose.com/slides/java
[6]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[7]: https://apireference.aspose.com/slides/java/com.aspose.slides/ITextFrame
[8]: https://apireference.aspose.com/slides/java/com.aspose.slides/SlideUtil#getAllTextBoxes-com.aspose.slides.IBaseSlide-
[9]: https://apireference.aspose.com/slides/java/com.aspose.slides/ITextFrame#getParagraphs--
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/IPortion
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/SlideUtil#getAllTextFrames-com.aspose.slides.IPresentation-boolean-
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/ITextFrame
[14]: https://purchase.aspose.com/temporary-license
[15]: https://products.aspose.app/slides/parser
[16]: https://docs.aspose.com/slides/java
[17]: https://forum.aspose.com/
[18]: https://blog.aspose.com/2021/01/18/create-powerpoint-presentations-using-java/





