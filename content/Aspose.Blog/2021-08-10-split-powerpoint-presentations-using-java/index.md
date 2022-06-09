---
title: 'Split PowerPoint Presentations using Java'
seoTitle: "Split PowerPoint Presentations using Java | Java PowerPoint API"
description: "Use Java PowerPoint API to split PPTX/PPT presentations using Java. Split each slide in the presentation and save it as a separate file."
date: Tue, 10 Aug 2021 15:00:00 +0000
draft: false
url: /2021/08/10/split-powerpoint-presentations-using-java/
author: Usman Aziz
summary: 'PowerPoint presentations are often required to be split into multiple PPTX/PPT files. You may split a presentation by each slide, even or odd slides, etc. as per your scenario. In this article, you will learn **how to split the PowerPoint PPTX/PPT presentations using Java**.'
tags: ['Java API to Split PowerPoint Presentations', 'Split a PPT using Java', 'Split a PPTX using Java', 'Split a PowerPoint Presentation using Java']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Split-PowerPoint-Presentation.jpg" alt="Split PowerPoint Presentation Java">}}


PowerPoint presentations are often required to be split into multiple PPTX/PPT files. You may split a presentation by each slide, even or odd slides, etc. as per your scenario. In this article, you will learn **how to split the PowerPoint PPTX/PPT presentations using Java**.

*   [Java API to Split PowerPoint Presentations][1]
*   [Split a PowerPoint Presentation using Java][2]

## Java API to Split PowerPoint Presentations {#NET-API-to-Split-PowerPoint-Presentations}

In order to split PPTX or PPT presentations, we will use [Aspose.Slides for Java][3]. The API is designed to create, modify and convert PowerPoint and OpenOffice presentations from within Java applications. You can either [download][4] the API or install it using the following Maven configurations.

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
    <version>21.8</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Split a PowerPoint Presentation using Java {#Split-a-PowerPoint-Presentation}

The following are the steps to split a PowerPoint presentation using Java.

*   First, create an instance of the [Presentation][5] class to load the PowerPoint presentation.
*   Then, loop through each [ISlide][6] in [Presentation.getSlides()][7] collection.
*   In each iteration, perform the following steps:
    *   Create an instance of [Presentation][8] class.
    *   Remove the default slide using [Presentation.getSlides().get\_item(0).remove()][9] method.
    *   Add the slide to the presentation using [Presentation.getSlides().addClone(ISlide)][10] method.
    *   Finally, save the presentation using [Presentation.save(String, SaveFormat)][11] method.

The following code sample shows how to split a PowerPoint PPTX presentation.

{{< gist aspose-com-gists 45a4f75a2eec6324a9da6541a6f70bf0 "split-presentation.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for Java without evaluation limitations by getting a [temporary license][12].

## Online Demo

Try the [online presentation splitter][13], which is based on Aspose.Slides.

## Conclusion

In this article, you have learned how to split PowerPoint PPTX or PPT presentations using Java. You can customize the provided code sample to split each slide in the presentation, all the even or odd slides, etc. In addition, you can visit the [documentation][14] to explore other features of API. Also, you can feel free to let us know about your queries via our [forum][15].

## See Also

*   [Create MS PowerPoint Presentations in Java][16]
*   [Add Watermark to PowerPoint Slides using Java][17]
*   [Extract Text from PowerPoint Files using Java][18]
*   [Add, Connect, Remove, or Clone PowerPoint Shapes in Java][19]
*   [Convert PowerPoint PPTX/PPT to PNG Images in Java][20]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using Java][21]




[1]: #NET-API-to-Split-PowerPoint-Presentations
[2]: #Split-a-PowerPoint-Presentation
[3]: https://products.aspose.com/slides/java
[4]: https://downloads.aspose.com/slides/java
[5]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[6]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[7]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#getSlides--
[8]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[9]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide#remove--
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlideCollection#addClone-com.aspose.slides.ISlide-
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[12]: https://purchase.aspose.com/temporary-license
[13]: https://products.aspose.app/slides/splitter
[14]: https://docs.aspose.com/slides/java
[15]: https://forum.aspose.com/
[16]: https://blog.aspose.com/2021/01/18/create-powerpoint-presentations-using-java/
[17]: https://blog.aspose.com/2021/06/13/add-watermark-to-powerpoint-using-java/
[18]: https://blog.aspose.com/2021/07/28/extract-text-from-powerpoint-files-using-java/
[19]: https://blog.aspose.com/2021/04/09/add-connect-remove-or-clone-powerpoint-shapes-in-java/
[20]: https://blog.aspose.com/2021/08/01/convert-powerpoint-to-png-in-java/
[21]: https://blog.aspose.com/2021/08/03/generate-thumbnails-for-powerpoint-using-java/





