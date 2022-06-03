---
title: 'Add Video Frame in PowerPoint PPT using Python'
date: Mon, 14 Feb 2022 02:55:00 +0000
draft: false
url: /2022/02/14/add-video-frame-to-ppt-in-python/
author: ''Usman Aziz''
summary: 'MS PowerPoint allows adding media elements to the presentations such as audio and video. Video frames are used to insert the video clips from local files or web sources. In this article, you will learn **how to add video frames in a PowerPoint PPT or PPTX in Python**. We will also demonstrate how to embed videos from a web source such as YouTube and extract videos from a PPT.'
tags: ['Add YouTube Video in PPT in Python', 'Add a Video Frame in a PowerPoint PPT Python', 'Extract Video from a PowerPoint PPT in Python', 'Python Library to Add Video Frame in PowerPoint PPT']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Embed-Video-in-PowerPoint.jpg" alt="Embed Video Frame in PowerPoint using Python">}}


MS PowerPoint allows adding media elements to the presentations such as audio and video. Video frames are used to insert the video clips from local files or web sources. In this article, you will learn **how to add video frames in a PowerPoint PPT or PPTX in Python**. We will also demonstrate how to embed videos from a web source such as YouTube and extract videos from a PPT.

*   [Python Library to Add Video Frame in PowerPoint PPT][1]
*   [Add a Video Frame in a PowerPoint PPT][2]
    
    *   [Insert Video from a Local File][3]
    
    *   [Add Video from a Web Source][4]
*   [Extract Video from a PowerPoint PPT][5]

**Info**: You may want to check out Aspose FREE [PowerPoint to Video][6] converter because this service allows you to convert presentations into stunning and engaging videos.

## Python Library to Add Video Frame in PowerPoint PPT {#API-to-Embed-Video-in-PowerPoint-Presentation}

To add video frames in PowerPoint PPT/PPTX, we will use [Aspose.Slides for Python via .NET][7]. The library provides a complete package to create and manipulate PowerPoint presentations. You can install it from [PyPI][8] using the following pip command.

```
> pip install aspose.slides
```

## Add a Video Frame to PowerPoint PPT in Python {#Embed-a-Video-in-PowerPoint-Presentation}

You can add a video either from your local storage or a web source, such as YouTube. The following sections demonstrate both scenarios with the help of code samples.

### Insert Video from a Local File {#Insert-Video-from-Local-File}

The following are the steps to add a video frame to a PowerPoint PPT in Python.

*   First, load PPT/PPTX file or create a new one using **Presentation** class.
*   Then, get reference of the desired slide.
*   Add video into the videos collection using **Presentation.videos.add\_video()** method and get its reference.
*   Add a video frame to the slide using **Slide.shapes.add\_video\_frame()** method and get its reference.
*   Set the play mode and volume of the video.
*   Finally, save presentation using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to embed a video in a PowerPoint PPT in Python.

{{< gist aspose-com-gists 6edfdea39b39361dace7737013acc82d "add-video-frame.py" >}}

### Embed Video in PowerPoint PPT from a Web Source {#Embed-Video-from-Web-Source}

You can also add a video in the PowerPoint PPT from a web source. For demonstration, let's embed a YouTube video into the PowerPoint PPT in Python.

*   First, load PPT/PPTX file or create a new one using **Presentation** class.
*   Then, get reference of the desired slide.
*   Add YouTube video from URL using **Slide.shapes.add\_video\_frame()** method and get its reference.
*   Set video thumbnail.
*   Finally, save presentation using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to embed a YouTube video into PowerPoint PPT in Python.

{{< gist aspose-com-gists 6edfdea39b39361dace7737013acc82d "add-video-frame-from-web.py" >}}

## Extract Video from a PowerPoint Presentation in Python {#Extract-Video-from-a-PowerPoint-Presentation}

There could be the case when you want to extract the videos added to a PowerPoint presentation. The following are the steps to achieve this.

*   First, load the PPT/PPTX file using **Presentation** class.
*   Then, loop through slides in **Presentation.slides** collection.
*   For each slide, loop through the collection of shapes it has.
*   If shape is a **VideoFrame**, then extract and save the embedded video.

The following code sample shows how to extract videos from a PowerPoint PPT in Python.

{{< gist aspose-com-gists 6edfdea39b39361dace7737013acc82d "extract-video-from-ppt.py" >}}

## Get a Free License {#Get-a-Free-API-License}

You can use Aspose.Slides for Python via .NET without evaluation limitations by getting a [temporary license][9].

## Conclusion

In this article, you have learned how to add video frames to PowerPoint PPT/PPTX in Python. We have covered how to embed video from a file or a web source such as YouTube. Moreover, you have seen how to extract videos from a presentation programmatically. Besides, you can visit the [documentation][10] to explore more about Aspose.Slides for Python. Also, you can post your queries to our [forum][11].

## See Also

*   [Create PowerPoint Files in Python][12]
*   [Convert PPTX to PDF in Python][13]
*   [Convert PPT to PNG in Python][14]
*   [PPT/PPTX to HTML in Python][15]
*   [Add Watermark in PowerPoint PPT in Python][16]




[1]: #API-to-Embed-Video-in-PowerPoint-Presentation
[2]: #Embed-a-Video-in-PowerPoint-Presentation
[3]: #Insert-Video-from-Local-File
[4]: #Embed-Video-from-Web-Source
[5]: #Extract-Video-from-a-PowerPoint-Presentation
[6]: https://products.aspose.app/slides/video
[7]: https://products.aspose.com/slides/python-net
[8]: https://pypi.org/project/aspose.slides/
[9]: https://purchase.aspose.com/temporary-license
[10]: https://docs.aspose.com/slides/python-net
[11]: https://forum.aspose.com/
[12]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[13]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/
[14]: https://blog.aspose.com/2021/12/29/convert-ppt-to-png-in-python/
[15]: https://blog.aspose.com/2021/12/16/convert-ppt-to-html-in-python/
[16]: https://blog.aspose.com/2022/02/09/add-watermark-to-powerpoint-ppt-in-python/




