---
title: 'Merge PowerPoint Presentations using Java'
seoTitle: "Merge PowerPoint Presentations in Java | Merge Slides in PPTX in Java"
description: "Merge PowerPoint PPTX presentations using Java. Merge all or selected slides from source to target presentations and select slide layout from slide master."
date: Wed, 09 Dec 2020 17:18:47 +0000
draft: false
url: /2020/12/09/merge-powerpoint-presentations-using-java/
author: Usman Aziz
summary: 'In this post, you will learn **how to merge PowerPoint PPTX presentations using Java**. MS PowerPoint presentations are widely used to create interactive slide shows related to business, education, and other domains. In particular cases, you may need to merge multiple presentations into a single file programmatically. In accordance with that, this post provides you some simple ways of merging PowerPoint presentations from within the Java applications.'
tags: ['merge powerpoint slides using java', 'merge presentation in java']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Merge-PowerPoint-files.jpg" alt="merge powerpoint presentation in java">}}


In this post, you will learn **how to merge PowerPoint PPTX presentations using Java**. MS PowerPoint presentations are widely used to create interactive slide shows related to business, education, and other domains. In particular cases, you may need to merge multiple presentations into a single file programmatically. In accordance with that, this post provides you some simple ways of merging PowerPoint presentations from within the Java applications.

*   [Java PowerPoint Merger API][1]
*   [Merge PowerPoint Presentations using Java][2]
*   [Merge Particular Slides of PowerPoint Presentations][3]
*   [Select Layout for Merged Slides using Slide Master][4]

## Java PowerPoint Merger API - Free Download {#Java-PowerPoint-Merger-API}

[Aspose.Slides for Java][5] is a powerful presentation manipulation API that provides almost all the features for PowerPoint automation in Java. Using the API, you can easily merge multiple PowerPoint presentations into a single file within a few lines of code. You can either [download][6] the API's JAR or install it within your Mave-based applications using the following configurations.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-slides</artifactId>
    <version>20.11</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Merge PowerPoint Presentations using Java {#Merge-PowerPoint-Presentations-using-Java}

The following are the steps to merge all the slides from one presentation to another using Aspose.Slides for Java.

*   Load the source and target presentations using [Presentation][7] class.
*   Loop through the slides of source presentation using [Presentation.getSlides()][8] method.
*   Merge the slides from source presentation to target using [Presentation.getSlides().addClone(ISlide)][9] method.
*   Save the target presentation using [Presentation.save(String, SaveFormat)][10] method.

The following code sample shows how to merge PowerPoint presentations using Java.

{{< gist aspose-com-gists a38246fe270c43b630c91d28b872412f "merge-presentations.java" >}}

### Target Presentation



{{< figure align=center src="images/merge-presentation1.jpg" alt="powerpoint presentation">}}


### Source Presentation



{{< figure align=center src="images/merge-presentation2.jpg" alt="source presentation ">}}


### Merged Presentation



{{< figure align=center src="images/merged-presentation.jpg" alt="merged presentation in java">}}


## Merge Particular Slides of PowerPoint Presentations {#Merge-Particular-Slides-of-PowerPoint-Presentations}

Instead of merging all the slides from one presentation to another, you can select a few to be merged. For this, you can access the slides using their index. The following are the steps to merge selected slides from source to target presentation.

*   Load the source and target presentations using [Presentation][11] class.
*   Loop through the slides of source presentation using [Presentation.getSlides()][12] method.
*   Select the slides to be merged using [Presentation.getSlides().get\_Item(index)][13] method.
*   Merge slides using [Presentation.getSlides().addClone(ISlide)][14] method.
*   Save the target presentation using [Presentation.save(String, SaveFormat)][15] method.

The following code sample shows how to merge particular slides of PowerPoint presentations in Java.

{{< gist aspose-com-gists a38246fe270c43b630c91d28b872412f "merge-presentations-selected-slides.java" >}}

## Select Layout for Merged Slides using Slide Master {#Select-Layout-for-Merged-Slides-using-Slide-Master}

In the previous examples, you didn't change the layout of the slides after merging. However, there might be a case when you need to modify the slides' layout according to the target presentation. For this, you can mention the master slide to be used using the [addClone(ISlide sourceSlide, IMasterSlide destMaster, boolean allowCloneMissingLayout)][16] method.

The following code sample shows how to define the master slide when merging the presentations.

{{< gist aspose-com-gists a38246fe270c43b630c91d28b872412f "merge-presentations-slide-master.java" >}}

### Merged Presentation



{{< figure align=center src="images/merged-presentation-slide-master.jpg" alt="merged presentation with layout">}}


## Conclusion

PowerPoint automation provides you with a wide range of features to manipulate presentations from within your own applications. In this article, you have learned one of the widely used features of merging PowerPoint presentations using Java. The step-by-step guide along with the API references has shown different ways of merging slides from one presentation to another. In case you would want to explore more about the API, visit the [documentation][17].

## See Also

*   [Convert PowerPoint to PDF using Java][18]




[1]: #Java-PowerPoint-Merger-API
[2]: #Merge-PowerPoint-Presentations-using-Java
[3]: #Merge-Particular-Slides-of-PowerPoint-Presentations
[4]: #Select-Layout-for-Merged-Slides-using-Slide-Master
[5]: https://products.aspose.com/slides/java
[6]: https://downloads.aspose.com/slides/java
[7]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[8]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#getSlides--
[9]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlideCollection#addClone-com.aspose.slides.ISlide-
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#getSlides--
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlideCollection#get_Item-int-
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlideCollection#addClone-com.aspose.slides.ISlide-
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlideCollection#addClone-com.aspose.slides.ISlide-com.aspose.slides.IMasterSlide-boolean-
[17]: https://docs.aspose.com/slides/java/
[18]: https://blog.aspose.com/2019/12/31/convert-powerpoint-ppt-pptx-to-pdf-in-java-using-aspose-slides/





