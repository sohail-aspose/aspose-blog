---
title: 'Insert or Extract Audio in PowerPoint Presentations using C#'
seoTitle: "C#: Insert or Extract Audio in PowerPoint Presentations | Source Code"
description: "Use .NET PowerPoint API to insert audio in PowerPoint presentations using C#. Extract audio from the slides in the presentations programmatically."
date: Tue, 21 Sep 2021 14:04:33 +0000
draft: false
url: /2021/09/21/add-or-extract-audio-in-powerpoint-using-csharp/
author: Usman Aziz
summary: 'In various cases, the presenters include sounds or audio clips in their presentations. MS PowerPoint provides audio frames to insert the sounds into the slides. In this article, you will learn how to automate the manipulation of audio frames in presentations. Particularly, the article will cover **how to insert or extract the audio frames in PowerPoint presentations using C#**.'
tags: ['Add an Audio Frame in PowerPoint Presentations Csharp', 'Csharp API to Manipulate Audio Frames in PowerPoint', 'Extract Audio Frames in Powerpoint Presentations Csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Add-Audio-in-PowerPoint.jpg" alt="Insert audio in PowerPoint C#">}}


In various cases, the presenters include sounds or audio clips in their presentations. MS PowerPoint provides audio frames to insert the sounds into the slides. In this article, you will learn how to automate the manipulation of audio frames in presentations. Particularly, the article will cover **how to insert or extract the audio frames in PowerPoint presentations using C#**.

*   [API to Manipulate Audio Frames in PowerPoint][1]
*   [Insert an Audio Frame in PowerPoint Presentations][2]
*   [Extract Audio Frames in PowerPoint Presentations][3]

**TIP**: If you ever need to extract the audio from a video clip, you can use Aspose [MP4 to MP3 converter][4] to do the job.

## C# API to Insert or Extract Audio Frames in PowerPoint {#API-to-Manipulate-Audio-Frames-in-PowerPoint}

To add or extract audio frames in PowerPoint presentations, we will use [Aspose.Slides for .NET][5]. It is a class library that lets you automate the creation and manipulation of PowerPoint and OpenOffice presentations. You can either install the API via [NuGet][6] or [download][7] its DLL.

```
PM> Install-Package Aspose.Slides.NET
```

## Insert an Audio Frame in PowerPoint Presentations using C# {#Insert-an-Audio-Frame-in-PowerPoint-Presentations}

The following are the steps to insert audio into a PowerPoint presentation using C#.

*   First, create a new presentation or load an existing one using [Presentation][8] class.
*   Then, load the audio from file into a [FileStream][9] object.
*   Insert the audio to the presentation using [ISlide.Shapes.AddAudioFrameEmbedded(Single, Single, Single, Single, Stream)][10] method and get the reference of the returned audio frame into an [IAudioFrame][11] object.
*   Set the additional properties such as PlayMode, Volume, etc.
*   Finally, save the presentation using [Presentation.Save(String, SaveFormat)][12] method.

The following code sample shows how to insert audio in a PowerPoint presentation.

{{< gist aspose-com-gists 355301e6ddc1f10c6d2d0dbf8969971d "insert-audio.cs" >}}

## Extract Audio Frames in PowerPoint Presentations using C# {#Extract-Audio-Frames-in-PowerPoint-Presentations}

You can also extract the audio frames from an existing PowerPoint presentation. The following are the steps to perform this operation.

*   First, load the PowerPoint presentation using [Presentation][13] class.
*   Then, get the desired slide into an [ISlide][14] object from [Presentation.Slides][15] collection.
*   Get reference of slideshow transition into an [ISlideShowTransition][16] object.
*   Retrieve the sound data into a _byte\[\]_ array from [ISlideShowTransition.Sound.BinaryData][17].
*   Finally, use the byte array or save it as a file.

The following code sample shows how to extract audio from a PowerPoint presentation using C#.

{{< gist aspose-com-gists 355301e6ddc1f10c6d2d0dbf8969971d "extract-audio.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

Use Aspose.Slides for .NET without evaluation limitations by getting a free [temporary license][18].

## Conclusion

In this article, you have learned how to insert audio in PowerPoint presentations using C#. Moreover, you have seen how to extract the audio clips from presentations programmatically. Besides, you can explore the [documentation][19] to learn more about Aspose.Slides for .NET. In addition, you can post your question to our [forum][20].

## See Also

*   [Convert PowerPoint PPTX/PPT to PNG Images in C#][21]
*   [Set Slide Background in PowerPoint Presentations using C#][22]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using C#][23]
*   [Apply Animation to Text in PowerPoint using C#][24]
*   [Split PowerPoint Presentations using C#][25]




[1]: #API-to-Manipulate-Audio-Frames-in-PowerPoint
[2]: #Insert-an-Audio-Frame-in-PowerPoint-Presentations
[3]: #Extract-Audio-Frames-in-PowerPoint-Presentations
[4]: https://products.aspose.app/slides/video/mp4-to-mp3
[5]: https://products.aspose.com/slides/net
[6]: https://www.nuget.org/packages/Aspose.Slides.NET
[7]: https://downloads.aspose.com/slides/net
[8]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[9]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream
[10]: https://apireference.aspose.com/slides/net/aspose.slides.ishapecollection/addaudioframeembedded/methods/1
[11]: https://apireference.aspose.com/slides/net/aspose.slides/iaudioframe
[12]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[13]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[14]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[15]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/slides
[16]: https://apireference.aspose.com/slides/net/aspose.slides/islideshowtransition
[17]: https://apireference.aspose.com/slides/net/aspose.slides/iaudio/properties/binarydata
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/slides/net/developer-guide/
[20]: https://forum.aspose.com/
[21]: https://blog.aspose.com/2021/09/01/convert-powerpoint-to-png-in-csharp/
[22]: https://blog.aspose.com/2021/08/31/set-background-in-powerpoint-using-csharp/
[23]: https://blog.aspose.com/2021/08/30/generate-pptx-thumbnails-using-csharp/
[24]: https://blog.aspose.com/2021/08/20/apply-animation-to-text-in-powerpoint-using-csharp/
[25]: https://blog.aspose.com/2021/09/03/split-powerpoint-presentations-using-csharp/




