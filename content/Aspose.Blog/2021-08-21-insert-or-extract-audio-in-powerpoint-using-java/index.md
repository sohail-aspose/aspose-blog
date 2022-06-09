---
title: 'Insert or Extract Audio in PowerPoint Presentations using Java'
seoTitle: "Java: Insert or Extract Audio in PowerPoint Presentations | Source Code"
description: "Use Java PowerPoint API to insert audio in PowerPoint presentations using Java. Extract audio from the slides in the presentations programmatically."
date: Sat, 21 Aug 2021 15:43:00 +0000
draft: false
url: /2021/08/21/insert-or-extract-audio-in-powerpoint-using-java/
author: Usman Aziz
summary: 'In various cases, the presenters use sounds or audio clips in their presentations. To include sounds in the presentations, MS PowerPoint provides audio frames. In this article, you are going to learn how to automate the manipulation of the audio frames. Particularly, the article will cover **how to insert or extract the audio frames in PowerPoint presentations using Java**.'
tags: ['Extract Audio Frames in PowerPoint Presentations Java', 'Insert an Audio Frame in PowerPoint Presentations Java', 'Java API to Manipulate Audio Frames in PowerPoint']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Add-Audio-in-PowerPoint.jpg" alt="Insert audio in PowerPoint Java">}}


In various cases, the presenters use sounds or audio clips in their presentations. To include sounds in the presentations, MS PowerPoint provides audio frames. In this article, you are going to learn how to automate the manipulation of the audio frames. Particularly, the article will cover **how to insert or extract the audio frames in PowerPoint presentations using Java**.

*   [API to Manipulate Audio Frames in PowerPoint][1]
*   [Insert an Audio Frame in PowerPoint Presentations][2]
*   [Extract Audio Frames in PowerPoint Presentations][3]

**Info**: Using Aspose [new MP4 to MP3 converter,][4] you can easily extract the audio or sound from a video clip.

## Java API to Insert or Extract Audio Frames in PowerPoint {#API-to-Manipulate-Audio-Frames-in-PowerPoint}

To add or extract audio frames in presentations, we will use [Aspose.Slides for Java][5]. It is a feature-rich API that allows you to create and process PowerPoint and OpenOffice documents. Moreover, it lets you convert the presentations to other file formats. You can either install the API via Maven or [download][6] its JAR.

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
    <version>21.9</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Insert an Audio Frame in PowerPoint Presentations using Java {#Insert-an-Audio-Frame-in-PowerPoint-Presentations}

The following are the steps to insert audio into a PowerPoint presentation using Java.

*   First, create a new presentation or load an existing one using [Presentation][7] class.
*   Then, load the audio from file into a [FileInputStream][8] object.
*   Insert the audio to the presentation using [ISlide.getShapes().addAudioFrameEmbedded(float, float, float, float, InputStream)][9] method and get the reference of the returned audio frame into an [IAudioFrame][10] object.
*   Set the additional properties such as PlayMode, Volume, etc.
*   Finally, save the presentation using [Presentation.save(String, SaveFormat)][11] method.

The following code sample shows how to insert audio in a PowerPoint presentation.

{{< gist aspose-com-gists c09e6c303ca65a21602154c569acc0a5 "insert-audio.java" >}}

## Extract Audio Frames in PowerPoint Presentations using Java {#Extract-Audio-Frames-in-PowerPoint-Presentations}

You can also extract the audio frames from an existing PowerPoint presentation. The following are the steps to perform this operation.

*   First, load the PowerPoint presentation using [Presentation][12] class.
*   Then, get the desired slide into an [ISlide][13] object using [Presentation.getSlides().get\_Item(int index)][14].
*   Get reference of slideshow transition into an [ISlideShowTransition][15] object.
*   Retrieve the sound data into a _byte\[\]_ array using [ISlideShowTransition.getSound().getBinaryData()][16] method.
*   Finally, use the byte array or save it as a file.

The following code sample shows how to extract audio from a PowerPoint presentation using Java.

{{< gist aspose-com-gists c09e6c303ca65a21602154c569acc0a5 "extract-audio.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

Use Aspose.Slides for Java without evaluation limitations by getting a free [temporary license][17].

## Conclusion

In this article, you have learned how to insert audio in PowerPoint presentations using Java. Moreover, you have seen how to extract the audio clips from presentations programmatically. Besides, you can explore the [documentation][18] to learn more about Aspose.Slides for Java. In addition, you can post your question to our [forum][19].

## See Also

*   [Add Watermark to PowerPoint Slides using Java][20]
*   [Extract Text from PowerPoint Files using Java][21]
*   [Add, Connect, Remove, or Clone PowerPoint Shapes in Java][22]
*   [Convert PowerPoint PPTX/PPT to PNG Images in Java][23]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using Java][24]




[1]: #API-to-Manipulate-Audio-Frames-in-PowerPoint
[2]: #Insert-an-Audio-Frame-in-PowerPoint-Presentations
[3]: #Extract-Audio-Frames-in-PowerPoint-Presentations
[4]: https://products.aspose.app/slides/video/mp4-to-mp3
[5]: https://products.aspose.com/slides/java
[6]: https://downloads.aspose.com/slides/java
[7]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[8]: https://docs.oracle.com/javase/7/docs/api/java/io/FileInputStream.html
[9]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection#addAudioFrameEmbedded-float-float-float-float-java.io.InputStream-
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/IAudioFrame
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlideCollection#get_Item-int-
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlideShowTransition
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/IAudio#getBinaryData--
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/slides/java
[19]: https://forum.aspose.com/
[20]: https://blog.aspose.com/2021/06/13/add-watermark-to-powerpoint-using-java/
[21]: https://blog.aspose.com/2021/07/28/extract-text-from-powerpoint-files-using-java/
[22]: https://blog.aspose.com/2021/04/09/add-connect-remove-or-clone-powerpoint-shapes-in-java/
[23]: https://blog.aspose.com/2021/08/01/convert-powerpoint-to-png-in-java/
[24]: https://blog.aspose.com/2021/08/03/generate-thumbnails-for-powerpoint-using-java/





