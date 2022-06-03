---
title: 'Add or Remove Hyperlinks in PowerPoint PPT in C#'
date: Wed, 02 Feb 2022 21:25:00 +0000
draft: false
url: /2022/02/02/work-with-hyperlinks-in-powerpoint-ppt-in-csharp/
author: 'Usman Aziz'
summary: 'Hyperlinks in documents are used to navigate from one location to another. Generally, in PowerPoint presentations, they are used to insert URLs of webpages. You can create a hyperlink of text, image, shape, or a media element in PowerPoint PPT slides. In this article, you will learn **how to add hyperlinks to PowerPoint PPT/PPTX in C#**. Moreover, we will cover how to remove hyperlinks from PPT slides programmatically.'
tags: ['add hyperlink to ppt in csharp', 'add hyperlink to ppt slides in csharp', 'add hyperlink to pptx in csharp', 'insert hyperlink to ppt in csharp', 'remove hyperlink from ppt in csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Add-hyperlink-in-PowerPoint-PPT.png" alt="Add or Remove Hyperlinks from PowerPoint PPT in C#">}}


Hyperlinks in documents are used to navigate from one location to another. Generally, in PowerPoint presentations, they are used to insert URLs of webpages. You can create a hyperlink of text, image, shape, or a media element in PowerPoint PPT slides. In this article, you will learn **how to add hyperlinks to PowerPoint PPT/PPTX in C#**. Moreover, we will cover how to remove hyperlinks from PPT slides programmatically.

*   [.NET API to Work with Hyperlinks in PowerPoint][1]
*   [Add a Hyperlink in PowerPoint PPT/PPTX][2]
    *   [Add Text Hyperlink][3]
    *   [Insert Shape Hyperlink][4]
    *   [Add Image Hyperlink][5]
    *   [Add Audio Hyperlink][6]
    *   [Insert Video Hyperlink][7]
*   [Remove Hyperlinks from PowerPoint PPT][8]

## C# .NET API to Add or Remove Hyperlinks in PowerPoint PPT {#API-to-Work-with-Hyperlinks-in-PowerPoint}

To work with hyperlinks in PowerPoint presentations, we will use [Aspose.Slides for .NET][9]. It is a popular API that is used to create and modify PPT/PPTX presentations. Moreover, it lets you convert the presentations to other popular formats. You can [download][10] its DLL or install it from [NuGet][11].

```
PM> Install-Package Aspose.Slides.NET 
```

## Add a Hyperlink in PowerPoint PPT/PPTX in C# {#Add-a-Hyperlink-in-PowerPoint-PPT}

You can add different types of hyperlinks in PowerPoint presentations using Aspose.Slides for .NET. The hyperlink could be a text, image, shape, audio, or video element. In the following sections, we will cover how to add all these hyperlinks in a PPT/PPTX presentation.

### Add Text Hyperlink in PowerPoint PPT {#Add-Text-Hyperlink}

The following are the steps to add a text hyperlink in a PowerPoint PPT/PPTX in C#.

*   First, load the presentation file or create a new one using [Presentation][12] class.
*   Then, add a rectangular auto shape to the shapes collection using [ISlide.Shapes.AddAutoShape(ShapeType, single, single, single, single)][13] method.
*   Add text to the shape using [IAutoShape.AddTextFrame(string)][14] method.
*   Create hyperlink using [IAutoShape.TextFrame.Paragraphs\[0\].Portions\[0\].PortionFormat.HyperlinkClick][15] property.
*   Set other properties of hyperlink such as tooltip.
*   Finally, save presentation using [Presentation.Save(string, SaveFormat)][16] method.

The following code sample shows how to add a text hyperlink in a PowerPoint PPTX using C#.

{{< gist aspose-com-gists 98b601922a6701e34618c68d5bdc2536 "add-text-hyperlink.cs" >}}

### Insert a Shape Hyperlink in PowerPoint {#Insert-Shape-Hyperlink}

The following steps demonstrate how to insert a shape hyperlink in a PowerPoint presentation in C#.

*   First, load the presentation file or create a new one using [Presentation][17] class.
*   Then, add an auto shape of desired type using [ISlide.Shapes.AddAutoShape(ShapeType, single, single, single, single)][18] method.
*   Create hyperlink using [IAutoShape.HyperlinkClick][19] property.
*   Finally, save presentation using [Presentation.Save(string, SaveFormat)][20] method.

The following code sample shows how to create a hyperlink of shape in PowerPoint using C#.

{{< gist aspose-com-gists 98b601922a6701e34618c68d5bdc2536 "add-shape-hyperlink.cs" >}}

### Insert an Image Hyperlink in PowerPoint {#Add-Image-Hyperlink}

The following are the steps to insert an image hyperlink in a PowerPoint PPT in C#.

*   First, load the presentation file or create a new one using [Presentation][21] class.
*   Then, add image to the collection using [Presentation.Images.AddImage()][22] method.
*   Add picture frame to the desired slide using [Presentation.Slides\[index\].Shapes.AddPictureFrame()][23] method.
*   Create hyperlink by setting [IPictureFrame.HyperlinkClick][24] property.
*   Finally, save presentation using [Presentation.Save(string, SaveFormat)][25] method.

The following code sample shows how to create a hyperlink of an image in PowerPoint using C#.

{{< gist aspose-com-gists 98b601922a6701e34618c68d5bdc2536 "add-image-hyperlink.cs" >}}

### Add an Audio Hyperlink in PPT {#Add-Audio-Hyperlink}

You can add an audio hyperlink to a PowerPoint PPT/PPTX by following the steps below:

*   First, load the presentation file or create a new one using [Presentation][26] class.
*   Then, add audio to the collection using [Presentation.Audios.AddAudio()][27] method.
*   After that, add audio frame to the desired slide using [Presentation.Slides\[index\].Shapes.AddAudioFrameEmbedded()][28] method.
*   Create hyperlink by setting [IAudioFrame.HyperlinkClick][29] property.
*   Finally, save presentation using [Presentation.Save(string, SaveFormat)][30] method.

The following code snippet demonstrates how to add an audio hyperlink in PowerPoint in C#:

{{< gist aspose-com-gists 98b601922a6701e34618c68d5bdc2536 "add-audio-hyperlink.cs" >}}

### Add a Video Hyperlink in PowerPoint PPT {#Insert-Video-Hyperlink}

To add a video hyperlink to a PowerPoint PPT/PPTX, follow the steps below:

*   First, load the presentation file or create a new one using [Presentation][31] class.
*   Then, add video to the collection using [Presentation.Videos.AddVideo()][32] method.
*   Add video frame to the desired slide using [Presentation.Slides\[index\].Shapes.AddVideoFrame()][33] method.
*   Create hyperlink by setting [IVideoFrame.HyperlinkClick][34] property.
*   Finally, save presentation using [Presentation.Save(string, SaveFormat)][35] method.

The following code snippet demonstrates how to add a video hyperlink in PowerPoint in C#:

{{< gist aspose-com-gists 98b601922a6701e34618c68d5bdc2536 "add-video-hyperlink.cs" >}}

## Remove Hyperlinks from PowerPoint PPT in C# {#Remove-Hyperlinks-from-PowerPoint-PPT}

In this section, we will demonstrate how to remove the hyperlinks from a PowerPoint slide. These hyperlinks could be of any type we have discussed above. The following are the steps to perform this operation.

*   First, load the presentation file using [Presentation][36] class.
*   Then, loop through all the shapes in the slide using [ISlide.Shapes][37] collection.
*   After that, remove hyperlink from shape using [IShape.HyperlinkManager.RemoveHyperlinkClick()][38] method.
*   To remove text hyperlinks, cast shape to [IAutoShape][39].
*   Loop through the paragraphs of the shape.
*   Loop through text portions of each paragraph.
*   Remove text hyperlink using [IPortion.PortionFormat.HyperlinkManager.RemoveHyperlinkClick()][40] method.
*   Finally, save presentation using [Presentation.Save(string, SaveFormat)][41] method.

The following code sample shows how to remove hyperlinks from a slide in PowerPoint PPT in C#.

{{< gist aspose-com-gists 98b601922a6701e34618c68d5bdc2536 "remove-hyperlink.cs" >}}

## Get a Free License

Use Aspose.Slides for .NET without evaluation limitations by getting a [free temporary license][42].

## Conclusion

In this article, you have learned how to add or remove hyperlinks in PowerPoint PPT in C#. Moreover, we have covered how to make hyperlinks of text, image, shape, audio, and video elements. Besides, you can explore more about Aspose.Slides for .NET by visiting the [documentation][43]. Also, you can post your queries to our [forum][44].

## See Also

*   [Create MS PowerPoint Presentations in C#][45]
*   [Add or Remove Shapes in PowerPoint Slides using C#][46]
*   [Extract Images from PowerPoint PPT in C#][47]




[1]: #API-to-Work-with-Hyperlinks-in-PowerPoint
[2]: #Add-a-Hyperlink-in-PowerPoint-PPT
[3]: #Add-Text-Hyperlink
[4]: #Insert-Shape-Hyperlink
[5]: #Add-Image-Hyperlink
[6]: #Add-Audio-Hyperlink
[7]: #Insert-Video-Hyperlink
[8]: #Remove-Hyperlinks-from-PowerPoint-PPT
[9]: https://products.aspose.com/slides/net
[10]: https://downloads.aspose.com/slides/net
[11]: https://www.nuget.org/packages/Aspose.Slides.Net
[12]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[13]: https://apireference.aspose.com/slides/net/aspose.slides/ishapecollection/methods/addautoshape
[14]: https://apireference.aspose.com/slides/net/aspose.slides/iautoshape/methods/addtextframe
[15]: https://apireference.aspose.com/slides/net/aspose.slides/ihyperlinkcontainer/properties/hyperlinkclick
[16]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[17]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[18]: https://apireference.aspose.com/slides/net/aspose.slides/ishapecollection/methods/addautoshape
[19]: https://apireference.aspose.com/slides/net/aspose.slides/ihyperlinkcontainer/properties/hyperlinkclick
[20]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[21]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[22]: https://apireference.aspose.com/slides/net/aspose.slides.iimagecollection/addimage/methods/2
[23]: https://apireference.aspose.com/slides/net/aspose.slides/ishapecollection/methods/addpictureframe
[24]: https://apireference.aspose.com/slides/net/aspose.slides/ihyperlinkcontainer/properties/hyperlinkclick
[25]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[26]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[27]: https://apireference.aspose.com/slides/net/aspose.slides.iaudiocollection/addaudio/methods/1
[28]: https://apireference.aspose.com/slides/net/aspose.slides/ishapecollection/methods/addaudioframeembedded
[29]: https://apireference.aspose.com/slides/net/aspose.slides/iaudioframe
[30]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[31]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[32]: https://apireference.aspose.com/slides/net/aspose.slides.ivideocollection/addvideo/methods/1
[33]: https://apireference.aspose.com/slides/net/aspose.slides/ishapecollection/methods/addvideoframe
[34]: https://apireference.aspose.com/slides/net/aspose.slides/ivideoframe
[35]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[36]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[37]: https://apireference.aspose.com/slides/net/aspose.slides/ibaseslide/properties/shapes
[38]: https://apireference.aspose.com/slides/net/aspose.slides/ihyperlinkmanager/methods/removehyperlinkclick
[39]: https://apireference.aspose.com/slides/net/aspose.slides/iautoshape
[40]: https://apireference.aspose.com/slides/net/aspose.slides/ihyperlinkmanager/methods/removehyperlinkclick
[41]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[42]: https://purchase.aspose.com/temporary-license
[43]: https://docs.aspose.com/slides/net
[44]: https://forum.aspose.com/
[45]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/
[46]: https://blog.aspose.com/2020/12/24/add-shapes-to-powerpoint-slides-in-csharp/
[47]: https://blog.aspose.com/2022/01/13/extract-images-from-ppt-in-csharp-net/




