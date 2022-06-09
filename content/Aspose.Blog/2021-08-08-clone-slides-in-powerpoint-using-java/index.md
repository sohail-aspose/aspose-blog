---
title: 'Clone Slides in PowerPoint Presentations using Java'
seoTitle: "Java Clone Slides in PowerPoint PPTX/PPT | Java Presentation API"
description: "Use Java PowerPoint API to clone slides in PowerPoint PPTX PPT presentations using Java. Clone slides within presentation or in another presentation."
date: Sun, 08 Aug 2021 14:09:00 +0000
draft: false
url: /2021/08/08/clone-slides-in-powerpoint-using-java/
author: Usman Aziz
summary: 'In various cases, you may need to make copies or clones of the slides in PowerPoint presentations. The cloning process makes the copy of a slide without disturbing the original slide. Furthermore, the clone of a slide can be made into the same presentation or into another one. In this article, you will learn how to automate slide cloning in PowerPoint presentations. Particularly, the article will cover **how to clone slides within the same or another PowerPoint presentation using Java**.'
tags: ['Clone Slide into Another Presentation Java', 'Clone Slide within a PowerPoint Presentation Java', 'Java API to Clone Slides in PowerPoint Presentations']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Clone-Slides-in-PowerPoint.jpg" alt="Clone Slides in PowerPoint C#">}}


In various cases, you may need to make copies or clones of the slides in PowerPoint presentations. The cloning process makes the copy of a slide without disturbing the original slide. Furthermore, the clone of a slide can be made into the same presentation or into another one. In this article, you will learn how to automate slide cloning in PowerPoint presentations. Particularly, the article will cover **how to clone slides within the same or another PowerPoint presentation using Java**.

*   [Java API to Clone Slides in PowerPoint Presentations][1]
*   [Clone Slide within a PowerPoint Presentation][2]
    *   [Copy Slide at the End of Presentation][3]
    *   [Clone Slide to a Specific Position][4]
*   [Clone Slide into Another Presentation][5]
    *   [Copy Slide at the End of Another Presentation][6]
    *   [Clone Slide to a Specific Position of Another Presentation][7]

## Java API to Clone Slides in PowerPoint Presentations {#API-to-Clone-Slides-in-PowerPoint-Presentations}

In order to clone slides in PPTX or PPT presentations, we will use [Aspose.Slides for Java][8]. It is a presentation manipulation API for creating, modifying, and converting PowerPoint and OpenOffice presentations. You can either [download][9] the API or install it using the following Maven configurations.

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

## Clone Slides within a PowerPoint Presentation in Java {#Clone-Slide-within-a-PowerPoint-Presentations}

You can clone a slide either at a specified location or at the end of the PowerPoint presentation. The following sections demonstrate each of the above-mentioned scenarios with code samples.

### Clone Slide at the End of Presentation {#Clone-Slide-at-the-End-of-Presentation}

The following are the steps to clone a slide at the end of a PowerPoint presentation using Java.

1.  First, load the PowerPoint presentation using [Presentation][10] class.
2.  Get reference of the slide collection using [Presentation.getSlides()][11] into an [ISlideCollection][12] object.
3.  Clone desired slide using [ISlideCollection.addClone(ISlide)][13] method by specifying the slide to be cloned as a parameter.
4.  Finally, save the presentation using [Presentation.save(String, SaveFormat)][14] method.

The following code sample shows how to clone a slide at the end of the PowerPoint presentation.

{{< gist aspose-com-gists 16fa693aad9f16ff60c2e21a80089fc2 "clone-slide-at-end.java" >}}

### Clone Slide to a Specific Position in Presentation {#Clone-Slide-to-a-Specific-Position}

The following are the steps to clone a slide at a specific position in the PowerPoint presentation using Java.

1.  First, load the PowerPoint presentation using [Presentation][15] class.
2.  Get reference of the slide collection using [Presentation.getSlides()][16] into an [ISlideCollection][17] object.
3.  Clone desired slide using [ISlideCollection.insertClone(Int32, ISlide)][18] method by specifying the destination index and slide to be cloned as parameters.
4.  Finally, save the presentation using [Presentation.save(String, SaveFormat)][19] method.

The following code sample shows how to clone a slide at a specific position in a PowerPoint presentation.

{{< gist aspose-com-gists 16fa693aad9f16ff60c2e21a80089fc2 "clone-slide-at-index.java" >}}

## Clone Slides into Another Presentation using Java {#Clone-Slide-into-Another-Presentation}

In this section, you will learn how to clone a slide from one presentation to another. The following subsections will cover the cloning of a slide at the end or at a specific position in the destination presentation.

### Clone Slide at the End of Another Presentation {#Copy-Clone-Slide-at-the-End-of-Another-Presentation}

The following are the steps to clone a slide at the end of another presentation using Java.

1.  Load the source PowerPoint presentation using [Presentation][20] class.
2.  Load the destination PowerPoint presentation using [Presentation][21] class.
3.  Get reference of the slide collection from destination presentation into an [ISlideCollection][22] object.
4.  Clone desired slide using [ISlideCollection.addClone(ISlide)][23] method by specifying the slide to be cloned as a parameter.
5.  Save the destination presentation using [Presentation.save(String, SaveFormat)][24] method.

The following code sample shows how to clone a slide from one presentation to another.

{{< gist aspose-com-gists 16fa693aad9f16ff60c2e21a80089fc2 "clone-slide-other-presentation.java" >}}

### Clone Slide to a Specific Position in Another Presentation {#Clone-Slide-to-a-Specific-Position-in-Another-Presentation}

The following are the steps to clone a slide at a specific position in another presentation using Java.

1.  Load the source PowerPoint presentation using [Presentation][25] class.
2.  Load the destination PowerPoint presentation using [Presentation][26] class.
3.  Get reference of the slide collection from destination presentation into an [ISlideCollection][27] object.
4.  Clone desired slide using [ISlideCollection.insertClone(Int32, ISlide)][28] method by specifying the destination index and slide to be cloned as parameters.
5.  Save the destination presentation using [Presentation.save(String, SaveFormat)][29] method.

The following code sample shows how to clone a slide into another PowerPoint presentation.

{{< gist aspose-com-gists 16fa693aad9f16ff60c2e21a80089fc2 "clone-slide-at-index-other-presentation.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for Java without evaluation limitations by requesting a [temporary license][30].

Tip: You may want to check out [Aspose FREE PowerPoint Splitter][31] used to split the slides in presentations and save them as separate files.

## Conclusion

In this article, you have learned how to clone slides in PowerPoint presentations using Java. The article explicitly covered the cloning of slides within a presentation or from one presentation to another. In addition, you can visit the [documentation][32] to explore other features of API. Also, you can feel free to let us know about your queries via our [forum][33].

## See Also

*   [Create MS PowerPoint Presentations in Java][34]
*   [Add Watermark to PowerPoint Slides using Java][35]
*   [Extract Text from PowerPoint Files using Java][36]
*   [Add, Connect, Remove, or Clone PowerPoint Shapes in Java][37]
*   [Convert PowerPoint PPTX/PPT to PNG Images in Java][38]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using Java][39]




[1]: #API-to-Clone-Slides-in-PowerPoint-Presentations
[2]: #Clone-Slide-within-a-PowerPoint-Presentations
[3]: #Clone-Slide-at-the-End-of-Presentation
[4]: #Clone-Slide-to-a-Specific-Position
[5]: #Clone-Slide-into-Another-Presentation
[6]: #Copy-Clone-Slide-at-the-End-of-Another-Presentation
[7]: #Clone-Slide-to-a-Specific-Position-in-Another-Presentation
[8]: https://products.aspose.com/slides/java
[9]: https://downloads.aspose.com/slides/java
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#getSlides--
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlideCollection
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlideCollection#addClone-com.aspose.slides.ISlide-
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#getSlides--
[17]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlideCollection
[18]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlideCollection#insertClone-int-com.aspose.slides.ISlide-
[19]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[20]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[21]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[22]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlideCollection
[23]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlideCollection#addClone-com.aspose.slides.ISlide-
[24]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[25]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[26]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[27]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlideCollection
[28]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlideCollection#insertClone-int-com.aspose.slides.ISlide-
[29]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[30]: https://purchase.aspose.com/temporary-license
[31]: https://products.aspose.app/slides/splitter
[32]: https://docs.aspose.com/slides/java
[33]: https://forum.aspose.com/
[34]: https://blog.aspose.com/2021/01/18/create-powerpoint-presentations-using-java/
[35]: https://blog.aspose.com/2021/06/13/add-watermark-to-powerpoint-using-java/
[36]: https://blog.aspose.com/2021/07/28/extract-text-from-powerpoint-files-using-java/
[37]: https://blog.aspose.com/2021/04/09/add-connect-remove-or-clone-powerpoint-shapes-in-java/
[38]: https://blog.aspose.com/2021/08/01/convert-powerpoint-to-png-in-java/
[39]: https://blog.aspose.com/2021/08/03/generate-thumbnails-for-powerpoint-using-java/





