---
title: 'Embed Video in PowerPoint Presentations using C#'
seoTitle: "Embed Video in PowerPoint Presentations using C# | .NET Source Code"
description: "Use .NET PowerPoint API to embed video in PowerPoint presentations using C# or VB.NET. Extract the videos from the presentations programmatically."
date: Fri, 17 Sep 2021 17:24:00 +0000
draft: false
url: /2021/09/17/embed-video-in-powerpoint-using-csharp/
author: Usman Aziz
summary: 'Video frames are used in PowerPoint presentations to demonstrate something or to attract the audience. Often, the videos are used to save time and make the presentations more effective. In this article, you will learn how to work with videos in presentations programmatically. Particularly, the article will cover **how to embed or extract a video in a PowerPoint presentation using C#**.'
tags: ['Embed Video from Web Source in PowerPoint Csharp', 'Embed a Video in PowerPoint Presentation using Csharp', 'Extract Video from a PowerPoint Presentation Csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Embed-Video-in-PowerPoint.jpg" alt="Embed Video in PowerPoint using C#">}}


Video frames are used in PowerPoint presentations to demonstrate something or to attract the audience. Often, the videos are used to save time and make the presentations more effective. In this article, you will learn how to work with videos in presentations programmatically. Particularly, the article will cover **how to embed or extract a video in a PowerPoint presentation using C#**.

*   [.NET API to Embed Video in PowerPoint Presentations][1]
*   [Embed a Video in a PowerPoint Presentation using C#][2]
*   [Embed Video from Web Source][3]
*   [Extract Video from a PowerPoint Presentation][4]

## .NET API to Embed Video in PowerPoint Presentations {#API-to-Embed-Video-in-PowerPoint-Presentation}

In order to embed or extract videos in PowerPoint presentations, we will use [Aspose.Slides for .NET][5]. The API is designed to create and manipulate PowerPoint and OpenOffice documents. You can either install the API via [NuGet][6] or [download][7] its DLL.

```
PM> Install-Package Aspose.Slides.NET
```

## Embed a Video in PowerPoint Presentation using C# {#Embed-a-Video-in-PowerPoint-Presentation}

The following are the steps to embed a video in a PowerPoint presentation using C#.

*   First, load the PowerPoint file or create a new one using [Presentation][8] class.
*   Then, get reference of the desired slide in an [ISlide][9] object.
*   Add a new video into the videos collection of the presentation using [Presentation.Videos.AddVideo()][10] method and get its reference into an [IVideo][11] object.
*   Add a new video frame in the slide using [ISlide.Shapes.AddVideoFrame(single, single, single, single, IVideo)][12] method.
*   Get reference of the video frame into an [IVideoFrame][13] object.
*   Set the play mode and volume of the video.
*   Finally, save presentation using [Presentation.Save(String, SaveFormat)][14] method.

The following code sample shows how to embed a video in a PowerPoint presentation using C#.

{{< gist aspose-com-gists 1ac63941dc836f9c33282db0bedfb3d0 "embed-video.cs" >}}

## Embed Video in Presentations from a Web Source {#Embed-Video-from-Web-Source}

You can also embed a video in the PowerPoint presentations from a web source. The following are the steps to achieve this.

*   First, load the PowerPoint file or create a new one using [Presentation][15] class.
*   Then, get reference of the desired slide in an [ISlide][16] object.
*   Add a new video frame in the slide by specifying the video's URL in [ISlide.Shapes.AddVideoFrame(single, single, single, single, String)][17] method.
*   Get reference of the video frame into an [IVideoFrame][18] object.
*   Set the play mode and volume of the video.
*   Set thumbnail of the video using a [WebClient][19].
*   Save presentation using [Presentation.Save(String, SaveFormat)][20] method.

The following code sample shows how to embed a video into the presentation from a web source.

{{< gist aspose-com-gists 1ac63941dc836f9c33282db0bedfb3d0 "embed-video-web.cs" >}}

## Extract Video from a PowerPoint Presentation in C# {#Extract-Video-from-a-PowerPoint-Presentation}

Aspose.Slides for .NET also allows you to extract a video from a presentation. Below are the simple steps to achieve this.

*   First, load the PowerPoint file using [Presentation][21] class.
*   Then, loop through each [ISlide][22] in [Presentation.Slides][23] collection.
*   For each _ISlide_ object, loop through the collection of [IShape][24] in it.
*   If _IShape_ is a [VideoFrame][25], then extract and save the embedded video.

The following code sample shows how to extract videos from a PowerPoint presentation using C#.

{{< gist aspose-com-gists 1ac63941dc836f9c33282db0bedfb3d0 "extract-video.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for .NET without evaluation limitations by requesting a [temporary license][26].

## Conclusion

In this article, you have learned how to embed videos in PowerPoint presentations using C#. Moreover, you have seen how to extract videos from a presentation programmatically. In addition to this, you can visit the [documentation][27] to explore more about Aspose.Slides for .NET. Also, you can post your queries to our [forum][28].

## See Also

*   [Create MS PowerPoint Presentations in C#][29]
*   [Convert PowerPoint PPTX/PPT to PNG Images in C#][30]
*   [Set Slide Background in PowerPoint Presentations using C#][31]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using C#][32]
*   [Apply Animation to Text in PowerPoint using C#][33]
*   [Split PowerPoint Presentations using C#][34]




[1]: #API-to-Embed-Video-in-PowerPoint-Presentation
[2]: #Embed-a-Video-in-PowerPoint-Presentation
[3]: #Embed-Video-from-Web-Source
[4]: #Extract-Video-from-a-PowerPoint-Presentation
[5]: https://products.aspose.com/slides/net
[6]: https://www.nuget.org/packages/Aspose.Slides.NET
[7]: https://downloads.aspose.com/slides/net
[8]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[9]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[10]: https://apireference.aspose.com/slides/net/aspose.slides.ivideocollection/addvideo/methods/2
[11]: https://apireference.aspose.com/slides/net/aspose.slides/ivideo
[12]: https://apireference.aspose.com/slides/net/aspose.slides/ishapecollection/methods/addvideoframe
[13]: https://apireference.aspose.com/slides/net/aspose.slides/ivideoframe
[14]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[15]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[16]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[17]: https://apireference.aspose.com/slides/net/aspose.slides.ishapecollection/addvideoframe/methods/1
[18]: https://apireference.aspose.com/slides/net/aspose.slides/ivideoframe
[19]: https://docs.microsoft.com/en-us/dotnet/api/system.net.webclient
[20]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[21]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[22]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[23]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/slides
[24]: https://apireference.aspose.com/slides/net/aspose.slides/ishape
[25]: https://apireference.aspose.com/slides/net/aspose.slides/videoframe
[26]: https://purchase.aspose.com/temporary-license
[27]: https://docs.aspose.com/slides/net/developer-guide/
[28]: https://forum.aspose.com/
[29]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/
[30]: https://blog.aspose.com/2021/09/01/convert-powerpoint-to-png-in-csharp/
[31]: https://blog.aspose.com/2021/08/31/set-background-in-powerpoint-using-csharp/
[32]: https://blog.aspose.com/2021/08/30/generate-pptx-thumbnails-using-csharp/
[33]: https://blog.aspose.com/2021/08/20/apply-animation-to-text-in-powerpoint-using-csharp/
[34]: https://blog.aspose.com/2021/09/03/split-powerpoint-presentations-using-csharp/




