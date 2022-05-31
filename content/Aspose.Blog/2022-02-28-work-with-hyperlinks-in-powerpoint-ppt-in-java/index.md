---
title: 'Add or Remove Hyperlinks in PowerPoint PPT in Java'
date: Mon, 28 Feb 2022 16:06:49 +0000
draft: false
url: /2022/02/28/work-with-hyperlinks-in-powerpoint-ppt-in-java/
author: ''Usman Aziz''
summary: 'In various cases, we have to insert hyperlinks in the PowerPoint presentations, such as for providing the URL of a webpage. You can create a hyperlink of text, image, shape, or a media element in PowerPoint PPT slides. In this article, you will learn **how to add hyperlinks to PowerPoint PPT/PPTX in Java**. In the end, we will also discuss how to remove hyperlinks from PPT slides programmatically.'
tags: ['Add Audio Video Hyperlink in PPT in Java', 'Add Text Hyperlink in PPT in Java', 'Add image Hyperlink in PPT in Java', 'Java API to Work with Hyperlinks in PowerPoint', 'Remove Hyperlink in PPT in Java']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Add-hyperlink-in-PowerPoint-PPT.png" alt="Add or Remove Hyperlinks from PowerPoint PPT in Java">}}


In various cases, we have to insert hyperlinks in the PowerPoint presentations, such as for providing the URL of a webpage. You can create a hyperlink of text, image, shape, or a media element in PowerPoint PPT slides. In this article, you will learn **how to add hyperlinks to PowerPoint PPT/PPTX in Java**. In the end, we will also discuss how to remove hyperlinks from PPT slides programmatically.

*   [Java API to Work with Hyperlinks in PowerPoint][1]
*   [Add a Hyperlink in PowerPoint PPT/PPTX][2]
    *   [Add Text Hyperlink][3]
    *   [Insert Shape Hyperlink][4]
    *   [Add Image Hyperlink][5]
    *   [Add Audio Hyperlink][6]
    *   [Insert Video Hyperlink][7]
*   [Remove Hyperlinks from PowerPoint PPT][8]

## Java API to Add or Remove Hyperlinks in PowerPoint PPT {#API-to-Work-with-Hyperlinks-in-PowerPoint}

To insert or remove hyperlinks in PowerPoint presentations, we will use [Aspose.Slides for Java][9]. The API provides a bunch of features to create and manipulate PPT/PPTX presentations seamlessly. Also, it allows you to convert the presentations to other document or image formats. You can [download][10] its JAR or install it using the following Maven configurations.

```
**Repository:**
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>

**Dependency:**
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-slides</artifactId>
    <version>22.2</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Add a Hyperlink in PowerPoint PPT/PPTX in Java {#Add-a-Hyperlink-in-PowerPoint-PPT}

The hyperlink in PowerPoint presentations can be added to a text, image, shape, audio, or video element. The following sections cover how to add hyperlinks to these elements in a PPT/PPTX presentation using Java.

### Add Text Hyperlink in PowerPoint PPT {#Add-Text-Hyperlink}

The following are the steps to add a text hyperlink in a PowerPoint PPT/PPTX in Java.

*   First, load the presentation file or create a new one using [Presentation][11] class.
*   Then, add a rectangular auto shape to the slide using [addAutoShape(ShapeType, float, float, float, float)][12] method.
*   Add text to the shape using [IAutoShape.addTextFrame(String)][13] method.
*   Get reference of [IPortionFormat][14] from the shape.
*   Create hyperlink using [IPortionFormat.setHyperlinkClick()][15] method.
*   Set other properties of hyperlink such as tooltip.
*   Finally, save presentation using [Presentation.save(String, SaveFormat)][16] method.

The following code sample shows how to add a text hyperlink in a PowerPoint PPTX using Java.

{{< gist aspose-com-gists f83f986aec97dbfcacb3bed11c1a3451 "add-text-hyperlink.java" >}}

### Insert a Shape Hyperlink in PowerPoint {#Insert-Shape-Hyperlink}

The following steps demonstrate how to insert a shape hyperlink in a PowerPoint presentation in Java.

*   First, load the presentation file or create a new one using [Presentation][17] class.
*   Then, add an auto shape of desired type using [addAutoShape(ShapeType, float, float, float, float)][18] method.
*   Create hyperlink using [IAutoShape.setHyperlinkClick()][19] method.
*   Finally, save presentation using [Presentation.save(string, SaveFormat)][20] method.

The following code sample shows how to create a hyperlink of shape in PowerPoint using Java.

{{< gist aspose-com-gists f83f986aec97dbfcacb3bed11c1a3451 "add-shape-hyperlink.java" >}}

### Insert an Image Hyperlink in PowerPoint {#Add-Image-Hyperlink}

The following are the steps to insert an image hyperlink in a PowerPoint PPT in Java.

*   First, load the presentation file or create a new one using [Presentation][21] class.
*   Then, add image to the collection using [Presentation.getImages().addImage()][22] method.
*   After that, add an [IPictureFrame][23] to the desired slide using [addPictureFrame()][24] method.
*   Create hyperlink using [IPictureFrame.setHyperlinkClick()][25] method.
*   Finally, save presentation using [Presentation.save(String, SaveFormat)][26] method.

The following code sample shows how to create a hyperlink of an image in PowerPoint using Java.

{{< gist aspose-com-gists f83f986aec97dbfcacb3bed11c1a3451 "add-image-hyperlink.java" >}}

### Add an Audio Hyperlink in PPT {#Add-Audio-Hyperlink}

You can add an audio hyperlink to a PowerPoint PPT/PPTX by following the steps below:

*   First, load the presentation file or create a new one using [Presentation][27] class.
*   Then, add audio to the collection using [Presentation.getAudios().addAudio()][28] method.
*   After that, add [IAudioFrame][29] to the desired slide using [addAudioFrameEmbedded()][30] method.
*   Create hyperlink by using [IAudioFrame.setHyperlinkClick()][31] method.
*   Finally, save presentation using [Presentation.Save(String, SaveFormat)][32] method.

The following code snippet demonstrates how to add an audio hyperlink in PowerPoint in Java.

{{< gist aspose-com-gists f83f986aec97dbfcacb3bed11c1a3451 "add-audio-hyperlink.java" >}}

### Add a Video Hyperlink in PowerPoint PPT {#Insert-Video-Hyperlink}

To add a video hyperlink to a PowerPoint PPT/PPTX, follow the steps below:

*   First, load the presentation file or create a new one using [Presentation][33] class.
*   Then, add video to the collection using [Presentation.getVideos().addVideo()][34] method.
*   Add [IVideoFrame][35] to the desired slide using [addVideoFrame()][36] method.
*   Create hyperlink by using [IVideoFrame.setHyperlinkClick()][37] method.
*   Finally, save presentation using [Presentation.save(String, SaveFormat)][38] method.

The following code snippet demonstrates how to add a video hyperlink in PowerPoint in Java:

{{< gist aspose-com-gists f83f986aec97dbfcacb3bed11c1a3451 "add-video-hyperlink.java" >}}

## Remove Hyperlinks from PowerPoint PPT in Java {#Remove-Hyperlinks-from-PowerPoint-PPT}

In this section, we will demonstrate how to remove the hyperlinks from a PowerPoint slide. These hyperlinks could be of any type we have discussed above. The following are the steps to perform this operation.

*   First, load the presentation file using [Presentation][39] class.
*   Then, loop through all the shapes in the slide using [ISlide.getShapes()][40] method.
*   After that, remove hyperlink from shape using [IShape.getHyperlinkManager().removeHyperlinkClick()][41] method.
*   To remove text hyperlinks, cast shape to [IAutoShape][42].
*   Loop through the paragraphs of the shape.
*   Loop through text portions of each paragraph.
*   Remove text hyperlink using [IPortion.getPortionFormat().getHyperlinkManager().removeHyperlinkClick()][43] method.
*   Finally, save presentation using [Presentation.save(String, SaveFormat)][44] method.

The following code sample shows how to remove hyperlinks from a slide in PowerPoint PPT in Java.

{{< gist aspose-com-gists f83f986aec97dbfcacb3bed11c1a3451 "remove-hyperlink.java" >}}

## Get a Free License

Use Aspose.Slides for Java without evaluation limitations by getting a [free temporary license][45].

## Conclusion

In this article, you have learned how to add or remove hyperlinks in PowerPoint PPT in Java. Particularly, you have seen how to make hyperlinks of text, image, shape, audio, and video elements. Also, we have covered how to remove text or shape hyperlinks explicitly. Besides, you can explore more about Aspose.Slides for Java by visiting the [documentation][46]. Also, you can post your queries to our [forum][47].

## See Also

*   [Create PowerPoint Presentations using Java][48]
*   [Apply 3D Effects in PowerPoint PPT in Java][49]
*   [Extract Images from PowerPoint PPT in Java][50]
*   [Create and Manipulate Tables in PowerPoint using Java][51]




[1]: #API-to-Work-with-Hyperlinks-in-PowerPoint
[2]: #Add-a-Hyperlink-in-PowerPoint-PPT
[3]: #Add-Text-Hyperlink
[4]: #Insert-Shape-Hyperlink
[5]: #Add-Image-Hyperlink
[6]: #Add-Audio-Hyperlink
[7]: #Insert-Video-Hyperlink
[8]: #Remove-Hyperlinks-from-PowerPoint-PPT
[9]: https://products.aspose.com/slides/java
[10]: https://downloads.aspose.com/slides/java
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection#addAutoShape-int-float-float-float-float-
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/IAutoShape#addTextFrame-java.lang.String-
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/IPortionFormat
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/IHyperlinkContainer#setHyperlinkClick-com.aspose.slides.IHyperlink-
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[17]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[18]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection#addAutoShape-int-float-float-float-float-
[19]: https://apireference.aspose.com/slides/java/com.aspose.slides/IHyperlinkContainer#setHyperlinkClick-com.aspose.slides.IHyperlink-
[20]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[21]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[22]: https://apireference.aspose.com/slides/java/com.aspose.slides/IImageCollection#addImage-byte:A-
[23]: https://apireference.aspose.com/slides/java/com.aspose.slides/IPictureFrame
[24]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection#addPictureFrame-int-float-float-float-float-com.aspose.slides.IPPImage-
[25]: https://apireference.aspose.com/slides/java/com.aspose.slides/IHyperlinkContainer#setHyperlinkClick-com.aspose.slides.IHyperlink-
[26]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[27]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[28]: https://apireference.aspose.com/slides/java/com.aspose.slides/IAudioCollection#addAudio-byte:A-
[29]: https://apireference.aspose.com/slides/java/com.aspose.slides/IAudioFrame
[30]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection#addAudioFrameEmbedded-float-float-float-float-com.aspose.slides.IAudio-
[31]: https://apireference.aspose.com/slides/java/com.aspose.slides/IHyperlinkContainer#setHyperlinkClick-com.aspose.slides.IHyperlink-
[32]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[33]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[34]: https://apireference.aspose.com/slides/java/com.aspose.slides/IVideoCollection#addVideo-byte:A-
[35]: https://apireference.aspose.com/slides/java/com.aspose.slides/IVideoFrame
[36]: https://apireference.aspose.com/slides/java/com.aspose.slides/IShapeCollection#addVideoFrame-float-float-float-float-com.aspose.slides.IVideo-
[37]: https://apireference.aspose.com/slides/java/com.aspose.slides/IHyperlinkContainer#setHyperlinkClick-com.aspose.slides.IHyperlink-
[38]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[39]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[40]: https://apireference.aspose.com/slides/java/com.aspose.slides/IBaseSlide#getShapes--
[41]: https://apireference.aspose.com/slides/java/com.aspose.slides/IHyperlinkManager#removeHyperlinkClick--
[42]: https://apireference.aspose.com/slides/java/com.aspose.slides/IAutoShape
[43]: https://apireference.aspose.com/slides/java/com.aspose.slides/IHyperlinkManager#removeHyperlinkClick--
[44]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[45]: https://purchase.aspose.com/temporary-license
[46]: https://docs.aspose.com/slides/java
[47]: https://forum.aspose.com/
[48]: https://blog.aspose.com/2021/01/18/create-powerpoint-presentations-using-java/
[49]: https://blog.aspose.com/2022/02/04/apply-three-d-effects-in-ppt-in-java/
[50]: https://blog.aspose.com/2022/01/13/extract-images-from-ppt-in-java/
[51]: https://blog.aspose.com/2021/09/23/manipulate-tables-in-powerpoint-using-java/




