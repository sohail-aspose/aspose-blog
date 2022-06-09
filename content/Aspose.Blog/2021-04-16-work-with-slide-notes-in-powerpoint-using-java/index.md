---
title: 'Read, Add, or Remove Slide Notes in PowerPoint using Java'
seoTitle: "Read, Add, Remove Slide Notes in Java | Java PowerPoint API"
description: "Use Java PowerPoint API to work with slide notes in PowerPoint using Java. Read, add or remove PowerPoint slides notes programmatically in Java."
date: Fri, 16 Apr 2021 23:38:00 +0000
draft: false
url: /2021/04/16/work-with-slide-notes-in-powerpoint-using-java/
author: Usman Aziz
summary: 'The slide notes are used to add additional information as a reference in the presentations. The presenters add these notes to recall the essential points relevant to their presentations. In this article, you will learn how to manipulate the slide notes in PowerPoint presentations programmatically. Particularly, the article will cover how to read, add, and remove the slide notes **in PowerPoint presentations using Java**.'
tags: ['Add Slide Notes to a PowerPoint Presentation', 'Read Slide Notes in a PowerPoint Presentation', 'Remove Slide Notes in a PowerPoint Presentation']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Manipulate-PowerPoint-Slide-Notes.jpg" alt="work with powerpoint slide notes in java">}}


The slide notes are used to add additional information as a reference in the presentations. The presenters add these notes to recall the essential points relevant to their presentations. In this article, you will learn how to manipulation of the slide notes in presentations programmatically. Particularly, the article will cover how to read, add, and remove the slide notes **in PowerPoint presentations using Java**.

*   [Java API to Work with PowerPoint Slide Notes][1]
*   [Read Slide Notes in a PowerPoint Presentation][2]
*   [Add Slide Notes to a PowerPoint Presentation][3]
*   [Remove Slide Notes in a PowerPoint Presentation][4]
*   [Get a Free API License][5]

## Java API to Work with PowerPoint Slide Notes {#Java-API-to-Work-with-PowerPoint-Slide-Notes}

In order to work with slide notes, we'll use [Aspose.Slides for Java][6]. It is a feature-rich API that lets you create, edit and convert PowerPoint presentations from within your Java applications. You can either [download][7] the API or install it using the following Maven configurations.

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
    <version>21.3</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Read Slide Notes in a PowerPoint Presentation in Java {#Read-Slide-Notes-in-a-PowerPoint-Presentation}

The following are the steps to read slide notes in PowerPoint presentations using Java.

*   First, load the presentation using the [Presentation][8] class.
*   Access the [INotesSlideManager][9] of the desired slide in the presentation using [Presentation.getSlides().get\_Item(index).getNotesSlideManager()][10] method.
*   Get slide notes in [INotesSlide][11] object using [INotesSlideManager.getNotesSlide()][12] method.
*   Finally, access text of the notes using [INotesSlide.getNotesTextFrame().getText()][13] method.

The following code sample shows how to read slide notes in PowerPoint presentation using Java.

{{< gist aspose-com-gists a605ff4bc972944568c9ccd989373404 "read-slide-notes.java" >}}

## Add Slide Notes to a PowerPoint Presentation using Java {#Add-Slide-Notes-to-a-PowerPoint-Presentation}

The following are the steps to add slide notes to a PowerPoint presentation using Java.

*   First, load or create the presentation using the [Presentation][14] class.
*   Access the [INotesSlideManager][15] of the desired slide in the presentation using [Presentation.getSlides().get\_Item(index).getNotesSlideManager()][16] method.
*   Get slide notes in [INotesSlide][17] object using [INotesSlideManager.getNotesSlide()][18] method.
*   Set text of the notes using [INotesSlide.getNotesTextFrame().setText(String)][19] method.
*   Finally, save the presentation using [Presentation.save(String, SaveFormat.Pptx)][20] method.

The following code sample shows how to add slide notes in a PowerPoint presentation using Java.

{{< gist aspose-com-gists a605ff4bc972944568c9ccd989373404 "add-slide-notes.java" >}}

## Remove Slide Notes in a PowerPoint Presentation {#Remove-Slide-Notes-in-a-PowerPoint-Presentation}

The following are the steps to remove the slides notes in PowerPoint presentations using Java.

*   First, load or create the presentation using the [Presentation][21] class.
*   Access the [INotesSlideManager][22] of the desired slide in the presentation using [Presentation.getSlides().get\_Item(index).getNotesSlideManager()][23] method.
*   Remove slide notes using [INotesSlideManager.removeNotesSlide()][24] method.
*   Finally, save the presentation using [Presentation.save(String, SaveFormat.Pptx)][25] method.

The following code sample shows how to remove slide notes in a PowerPoint presentation using Java.

{{< gist aspose-com-gists a605ff4bc972944568c9ccd989373404 "remove-slide-notes.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [request a free temporary license][26] to use the API without evaluation limitations.

## Conclusion

In this article, you have learned how to work with slide notes in PowerPoint presentations using Java. The step-by-step guide and code samples have shown how to read, add, or remove slide notes. In addition, you can explore more about the API using the [documentation][27]. Alongside, you can post your queries to our [forum][28].

## See Also

*   [Create PowerPoint Presentations using Java][29]




[1]: #Java-API-to-Work-with-PowerPoint-Slide-Notes
[2]: #Read-Slide-Notes-in-a-PowerPoint-Presentation
[3]: #Add-Slide-Notes-to-a-PowerPoint-Presentation
[4]: #Remove-Slide-Notes-in-a-PowerPoint-Presentation
[5]: #Get-a-Free-API-License
[6]: https://products.aspose.com/slides/java
[7]: https://downloads.aspose.com/slides/java
[8]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[9]: https://apireference.aspose.com/slides/java/com.aspose.slides/INotesSlideManager
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide#getNotesSlideManager--
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/INotesSlide
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/INotesSlideManager#getNotesSlide--
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/INotesSlide#getNotesTextFrame--
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/INotesSlideManager
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide#getNotesSlideManager--
[17]: https://apireference.aspose.com/slides/java/com.aspose.slides/INotesSlide
[18]: https://apireference.aspose.com/slides/java/com.aspose.slides/INotesSlideManager#getNotesSlide--
[19]: https://apireference.aspose.com/slides/java/com.aspose.slides/ITextFrame#setText-java.lang.String-
[20]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[21]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[22]: https://apireference.aspose.com/slides/java/com.aspose.slides/INotesSlideManager
[23]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide#getNotesSlideManager--
[24]: https://apireference.aspose.com/slides/java/com.aspose.slides/INotesSlideManager#removeNotesSlide--
[25]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[26]: https://purchase.aspose.com/temporary-license
[27]: https://docs.aspose.com/slides/java/
[28]: https://forum.aspose.com/
[29]: https://blog.aspose.com/2021/01/18/Create-PowerPoint-Presentations-using-Java/





