---
title: 'Add Audio to PowerPoint PPT in Python'
date: Sat, 15 Jan 2022 07:29:00 +0000
draft: false
url: /2022/01/15/add-audio-to-powerpoint-ppt-in-python/
author: ''Usman Aziz''
summary: 'In various cases, audio clips are used to make the PowerPoint presentations more interactive. To add audio in a PPT/PPTX presentation, MS PowerPoint provides an audio frame object. In this article, you will learn **how to add an audio frame to a PowerPoint PPT in Python**. Moreover, you will come to know how to extract audio from a presentation and save it as a file.'
tags: []
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Add-Audio-in-PowerPoint.jpg" alt="add audio in PowerPoint PPT in Python">}}


In various cases, audio clips are used to make the PowerPoint presentations more interactive. To add audio in a PPT/PPTX presentation, MS PowerPoint provides an audio frame object. In this article, you will learn **how to add an audio frame to a PowerPoint PPT in Python**. Moreover, you will come to know how to extract audio from a presentation and save it as a file.

*   [Python Library to Add Audio in PowerPoint PPT][1]
*   [Add an Audio in a PowerPoint PPT][2]
*   [Extract Audio from a PowerPoint PPT][3]

**Info**: Aspose, through its [online MP4 to MP3][4] converter, now provides an online tool that allows you to extract the audio from a video.

## Python Library to Add Audio in PowerPoint {#API-to-Manipulate-Audio-Frames-in-PowerPoint}

To add and extract audio in PowerPoint presentations, we will use [Aspose.Slides for Python via .NET][5]. It is a powerful library that is used to create and manipulate PowerPoint presentations seamlessly. You can install it from [PyPI][6] using the following command.

```
> pip install aspose.slides
```

## Add Audio in PowerPoint PPT in Python {#Insert-an-Audio-Frame-in-PowerPoint-Presentations}

The following are the steps to insert audio into a PowerPoint PPT in Python.

*   First, create a new presentation or load an existing one using **Presentation** class.
*   Get reference of a slide from **Presentations.slides** collection.
*   Load the audio from file.
*   Add audio frame using **Slide.shapes.add\_audio\_frame\_embedded()** method.
*   Set the additional properties such as play mode and volume.
*   Finally, save the presentation using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to add audio in a PowerPoint PPT in Python.

{{< gist aspose-com-gists ee09e5bcac0baed7e7ba13e052ffa85e "add-audio-in-ppt.py" >}}

## Extract Audio from PowerPoint in Python {#Extract-Audio-Frames-in-PowerPoint-Presentations}

You can also extract the audios which are embedded into a PPT/PPTX presentation. The following are the steps to perform this operation.

*   First, load the PPT/PPTX file using **Presentation** class.
*   Then, loop through slides in **Presentation.slides** collection.
*   For each slide, loop through the collection of shapes it has.
*   If shape is a **AudioFrame**, then extract and save the embedded audio.

The following code sample shows how to extract audio from a PowerPoint PPTX in Python.

{{< gist aspose-com-gists ee09e5bcac0baed7e7ba13e052ffa85e "extract-audio-in-ppt.py" >}}

## Get a Free License {#Get-a-Free-API-License}

Use Aspose.Slides for Python without evaluation limitations by getting a free [temporary license][7].

## Conclusion

In this article, you have learned how to add audio in PowerPoint PPT or PPTX in Python. Moreover, you have seen how to extract the audios from PowerPoint presentations programmatically. Besides, you can read more about Aspose.Slides for Python using the [documentation][8]. In addition, you can post your question to our [forum][9].

## See Also

*   [Create PowerPoint Files in Python][10]
*   [Convert PPTX to PDF in Python][11]
*   [PPT/PPTX to HTML in Python][12]
*   [Add Watermark in PowerPoint PPT in Python][13]




[1]: #API-to-Manipulate-Audio-Frames-in-PowerPoint
[2]: #Insert-an-Audio-Frame-in-PowerPoint-Presentations
[3]: #Extract-Audio-Frames-in-PowerPoint-Presentations
[4]: https://products.aspose.app/slides/video/mp4-to-mp3
[5]: https://products.aspose.com/slides/python-net
[6]: https://pypi.org/project/aspose.slides/
[7]: https://purchase.aspose.com/temporary-license
[8]: https://docs.aspose.com/slides/python-net/
[9]: https://forum.aspose.com/
[10]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[11]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/
[12]: https://blog.aspose.com/2021/12/16/convert-ppt-to-html-in-python/
[13]: https://blog.aspose.com/2022/02/09/add-watermark-to-powerpoint-ppt-in-python/




