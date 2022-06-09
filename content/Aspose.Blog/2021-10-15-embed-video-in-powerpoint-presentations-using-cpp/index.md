---
title: 'Embed Video in PowerPoint Presentations using C++'
seoTitle: "Embed Video in PowerPoint Presentations using C++"
description: "Embed videos in PowerPoint presentations using C++. Use the C++ PowerPoint API to extract and save embedded videos from PowerPoint presentations."
date: Fri, 15 Oct 2021 17:35:35 +0000
draft: false
url: /2021/10/15/embed-video-in-powerpoint-presentations-using-cpp/
author: Muhammad Ahmad
summary: 'Microsoft PowerPoint provides you the ability to add video frames to your PowerPoint presentations. Videos can be used to enhance the quality of the presentations and help better communicate the message to the audience. There might be situations where you want to add videos to PowerPoint presentations programmatically. To that end, this article will teach you **how to embed video in PowerPoint presentations using C++**.'
tags: ['Embed Video from Web Source in PowerPoint Presentations C++', 'Embed Video in PowerPoint Presentations C++', 'Extract Embedded Video from PowerPoint Presentations C++']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Embed-Video-in-PowerPoint.jpg" alt="Embed Video in PowerPoint Presentations using C++">}}


Microsoft PowerPoint provides you the ability to add video frames to your PowerPoint presentations. Videos can be used to enhance the quality of the presentations and help better communicate the message to the audience. There might be situations where you want to add videos to PowerPoint presentations programmatically. To that end, this article will teach you **how to embed video in PowerPoint presentations using C++**.

*   [C++ API for Embedding Video in PowerPoint Presentations][1]
*   [Embed Video in PowerPoint Presentations using C++][2]
*   [Embedding Video from a Web Source in PowerPoint Presentations][3]
*   [Extract Video from PowerPoint Presentations using C++][4]

**TIP**: You may want to check out Aspose FREE [PowerPoint to Video][5] converter because it allows you to transform your presentations to stunning videos with transition effects.

## C++ API for Embedding Video in PowerPoint Presentations {#CPP-API-for-Embedding-Video-in-PowerPoint-Presentations}

We will use the [Aspose.Slides for C++][6] API to embed videos in PowerPoint presentations. It is a powerful and feature-rich API that supports creating, reading, and modifying PowerPoint files without needing Mircosoft PowerPoint to be installed. You can either install the API through [NuGet][7] or download it directly from the [Downloads][8] section.

```
PM> Install-Package Aspose.Slides.Cpp
```

## Embed Video in PowerPoint Presentations using C++ {#Embed-Video-in-PowerPoint-Presentations-using-CPP}

The following are the steps to embed a video in a PowerPoint presentation.

*   Firstly, create an instance of the [Presentation][9] class to represent a new PowerPoint file.
*   Retrieve the slide where you want to embed the video.
*   Add the video to the presentation using the [Presentation->get\_Videos()->AddVideo (System::SharedPtr<System::IO::Stream> stream)][10] method.
*   Add the video frame using the [ISlide->get\_Shapes()->AddVideoFrame(float x, float y, float width, float height, System::SharedPtr< IVideo > video)][11] method.
*   Embed the video inside the video frame using the [IVideoFrame->set\_EmbeddedVideo(System::SharedPtr<IVideo> value)][12] method.
*   Set the play mode and volume of the video.
*   Lastly, save the presentation using the [Presentation->Save(System::String fname, Export::SaveFormat format)][13] method.

The following sample code shows how to embed a video in a PowerPoint presentation using C++.

{{< gist aspose-com-gists 4a3a1091a76aaef2c5756cc4e36296f4 "Embed_Video.cpp" >}}

## Embedding Video from a Web Source in PowerPoint Presentations {#Embedding-Video-from-a-Web-Source-in-PowerPoint-Presentations}

The following are the steps to embed a video from a web source in a PowerPoint presentation.

*   Firstly, create an instance of the [Presentation][14] class to represent a new PowerPoint file.
*   Retrieve the slide where you want to embed the video.
*   Add a video frame using the [ISlide->get\_Shapes()->AddVideoFrame(float x, float y, float width, float height, System::String fname)][15] method.
*   Set the play mode of the video.
*   Finally, save the presentation using the [Presentation->Save(System::String fname, Export::SaveFormat format)][16] method.

The following sample code shows how to embed a video from a web source in a PowerPoint presentation using C++.

{{< gist aspose-com-gists 4a3a1091a76aaef2c5756cc4e36296f4 "Embed_Video_From_Web.cpp" >}}

## Extract Video from PowerPoint Presentations using C++ {#Extract-Video-from-PowerPoint-Presentations-using-CPP}

The following are the steps to extract a video from a PowerPoint presentation using C++.

*   Firstly, load the PowerPoint file using the [Presentation][17] class.
*   Loop through the slides of the presentation.
*   Loop through the shapes in each slide.
*   For each shape, check if the shape is a [VideoFrame][18]. In case it is a video frame, extract the embedded video and save it.

The following sample code shows how to extract a video from a PowerPoint presentation using C++.

{{< gist aspose-com-gists 4a3a1091a76aaef2c5756cc4e36296f4 "Extract_Video.cpp" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][19].

## Conclusion

In this article, you have learned how to embed videos in PowerPoint presentations using C++. Moreover, you have seen how to extract embedded videos from PowerPoint presentations using Aspose.Slides for C++ API. It is a robust API that provides many additional features for working with PowerPoint files. You can explore the API in detail by visiting the [official documentation][20]. In case of any questions, please feel free to reach us at our [free support forum][21].

## See Also

*   [Add Slide Transitions in PowerPoint Presentations using C++][22]
*   [Set Slide Background in PowerPoint Presentations using C++][23]




[1]: #CPP-API-for-Embedding-Video-in-PowerPoint-Presentations
[2]: #Embed-Video-in-PowerPoint-Presentations-using-CPP
[3]: #Embedding-Video-from-a-Web-Source-in-PowerPoint-Presentations
[4]: #Extract-Video-from-PowerPoint-Presentations-using-CPP
[5]: https://products.aspose.app/slides/video
[6]: https://products.aspose.com/slides/cpp
[7]: https://www.nuget.org/packages/Aspose.Slides.Cpp
[8]: https://downloads.aspose.com/slides/cpp
[9]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[10]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_video_collection#abd6caf592c4a18271553e473e087362a
[11]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_shape_collection#a44394deb32033aafe7a6f0d0b1403064
[12]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_video_frame#a64dd7043d129a18a649d8cc1cf27a4a4
[13]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[14]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[15]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_shape_collection#aae7ae2e77d6f987be81e1c54dd5d14af
[16]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[17]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[18]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.video_frame
[19]: https://purchase.aspose.com/temporary-license
[20]: https://docs.aspose.com/slides/cpp/
[21]: https://forum.aspose.com/c/slides/11
[22]: https://blog.aspose.com/2021/10/14/add-slide-transitions-in-powerpoint-presentations-using-cpp/
[23]: https://blog.aspose.com/2021/10/12/set-slide-background-in-powerpoint-presentations-using-cpp/




