---
title: 'Embed or Extract Videos in PowerPoint Presentations using Java'
seoTitle: "Java: Embed or Extract Videos in PowerPoint Presentations | Source Code"
description: "Use Java PowerPoint API to embed video in PowerPoint presentations using Java. Extract the videos from the presentations programmatically."
date: Mon, 20 Sep 2021 13:49:15 +0000
draft: false
url: /2021/09/20/embed-or-extract-videos-in-powerpoint-using-java/
author: Usman Aziz
summary: 'PowerPoint presentations often contain video frames to demonstrate something or to attract the audience. In many cases, the videos are used to save time and make the presentations effective. In this article, you will learn how to work with videos in PowerPoint files programmatically. Particularly, the article will cover **how to embed or extract a video in a PowerPoint presentation using Java**.'
tags: ['Embed Video from Web Source in Java', 'Embed a Video in a PowerPoint Presentation using Java', 'Extract Video from a PowerPoint Presentation in Java', 'Java API to Embed Video in PowerPoint Presentations']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Embed-Video-in-PowerPoint.jpg" alt="Embed Video in PowerPoint using Java">}}


PowerPoint presentations often contain video frames to demonstrate something or to attract the audience. In many cases, the videos are used to save time and make the presentations effective. In this article, you will learn how to work with videos in PowerPoint files programmatically. Particularly, the article will cover **how to embed or extract a video in a PowerPoint presentation using Java**.

*   [Java API to Embed Video in PowerPoint Presentations][1]
*   [Embed a Video in a PowerPoint Presentation using Java][2]
*   [Embed Video from Web Source][3]
*   [Extract Video from a PowerPoint Presentation][4]

**Info**: Aspose recently developed a free [MP4 to MP3][5] web app that can be used to extract audio from video files.

## Java API to Embed Video in PowerPoint Presentations {#API-to-Embed-Video-in-PowerPoint-Presentation}

In order to embed or extract videos in PowerPoint presentations, we will use [Aspose.Slides for Java][6]. The API is designed to create and manipulate PowerPoint and OpenOffice documents. You can either [download][7] the API's JAR or install it using the following Maven configurations.

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

## Embed a Video in PowerPoint Presentation using Java {#Embed-a-Video-in-PowerPoint-Presentation}

The following are the steps to embed a video in a PowerPoint presentation using Java.

*   First, load the PowerPoint file or create a new one using [Presentation][8] class.
*   Then, get reference of the desired slide in an [ISlide][9] object.
*   Add a new video into the videos collection of the presentation using [Presentation.getVideos().addVideo()][10] method and get its reference into an [IVideo][11] object.
*   Add a new video frame in the slide using [ISlide.getShapes().addVideoFrame(single, single, single, single, IVideo)][12] method.
*   Get reference of the video frame into an [IVideoFrame][13] object.
*   Set the play mode and volume of the video.
*   Finally, save presentation using [Presentation.save(String, SaveFormat)][14] method.

The following code sample shows how to embed a video in a PowerPoint presentation using Java.

{{< gist aspose-com-gists 5c16c66ab53f4a56c8a1391764741097 "embed-video.java" >}}

## Embed Video from a Web Source using Java {#Embed-Video-from-Web-Source}

You can also embed a video in the PowerPoint presentations from a web source. The following are the steps to achieve this.

*   First, load the PowerPoint file or create a new one using [Presentation][15] class.
*   Then, get reference of the desired slide in an [ISlide][16] object.
*   Add a new video frame in the slide by specifying the video's URL in [ISlide.getShapes().addVideoFrame(single, single, single, single, String)][17] method.
*   Get reference of the video frame into an [IVideoFrame][18] object.
*   Set the play mode and volume of the video.
*   Set thumbnail of the video.
*   Finally, save presentation using [Presentation.save(String, SaveFormat)][19] method.

The following code sample shows how to embed a video into the presentation from a web source.

{{< gist aspose-com-gists 5c16c66ab53f4a56c8a1391764741097 "embed-video-web.java" >}}

## Extract Video from a PowerPoint Presentation in Java {#Extract-Video-from-a-PowerPoint-Presentation}

Aspose.Slides for Java also allows you to extract a video from a presentation. Below are the simple steps to achieve this.

*   First, load the PowerPoint file using [Presentation][20] class.
*   Then, loop through each [ISlide][21] in [Presentation.getSlides()][22] collection.
*   For each _ISlide_ object, loop through the collection of [IShape][23] in it.
*   If _IShape_ is a [VideoFrame][24], then extract and save the embedded video.

The following code sample shows how to extract videos from a PowerPoint presentation using Java.

{{< gist aspose-com-gists 5c16c66ab53f4a56c8a1391764741097 "extract-video.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for Java without evaluation limitations by requesting a [temporary license][25].

## Conclusion

In this article, you have learned how to embed videos in PowerPoint presentations using Java. Moreover, you have seen how to extract videos from a presentation programmatically. In addition to this, you can visit the [documentation][26] to explore more about Aspose.Slides for Java. Also, you can post your queries to our [forum][27].

## See Also

*   [Add Watermark to PowerPoint Slides using Java][28]
*   [Extract Text from PowerPoint Files using Java][29]
*   [Add, Connect, Remove, or Clone PowerPoint Shapes in Java][30]
*   [Convert PowerPoint PPTX/PPT to PNG Images in Java][31]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using Java][32]




[1]: #API-to-Embed-Video-in-PowerPoint-Presentation
[2]: #Embed-a-Video-in-PowerPoint-Presentation
[3]: #Embed-Video-from-Web-Source
[4]: #Extract-Video-from-a-PowerPoint-Presentation
[5]: https://products.aspose.app/slides/video/mp4-to-mp3
[6]: https://products.aspose.com/slides/java
[7]: https://downloads.aspose.com/slides/java
[8]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[9]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/IVideoCollection#addVideo-java.io.InputStream-
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/IVideo
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection#addVideoFrame-float-float-float-float-com.aspose.slides.IVideo-
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/IVideoFrame
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[17]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection#addVideoFrame-float-float-float-float-java.lang.String-
[18]: https://apireference.aspose.com/slides/java/com.aspose.slides/IVideoFrame
[19]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[20]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[21]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[22]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#getSlides--
[23]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShape
[24]: https://apireference.aspose.com/slides/java/com.aspose.slides/IVideoFrame
[25]: https://purchase.aspose.com/temporary-license
[26]: https://docs.aspose.com/slides/java
[27]: https://forum.aspose.com/
[28]: https://blog.aspose.com/2021/06/13/add-watermark-to-powerpoint-using-java/
[29]: https://blog.aspose.com/2021/07/28/extract-text-from-powerpoint-files-using-java/
[30]: https://blog.aspose.com/2021/04/09/add-connect-remove-or-clone-powerpoint-shapes-in-java/
[31]: https://blog.aspose.com/2021/08/01/convert-powerpoint-to-png-in-java/
[32]: https://blog.aspose.com/2021/08/03/generate-thumbnails-for-powerpoint-using-java/




