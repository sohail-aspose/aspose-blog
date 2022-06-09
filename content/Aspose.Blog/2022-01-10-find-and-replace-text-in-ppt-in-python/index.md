---
title: 'Find and Replace Text in PowerPoint PPT in Python'
seoTitle: "Python Find and Replace Text in PowerPoint PPTX PPT | Python PPTX"
description: "Use Python PowerPoint library to find and replace text in PPT/PPTX programmatically. Search a particular text in PPT slides and replace it dynamically."
date: Mon, 10 Jan 2022 13:56:00 +0000
draft: false
url: /2022/01/10/find-and-replace-text-in-ppt-in-python/
author: Usman Aziz
summary: 'While processing digital documents, you often need to find and replace a specific text in the content. This could be required when a piece of information is to be censored before sharing the documents. To accomplish this programmatically, this article covers **how to find and replace text in PowerPoint [PPT][1] or [PPTX][2] in Python**.'
tags: ['Find and Replace Text in PPT in Python', 'Find and Replace Text in PPTX in Python', 'Python Library to Find and Replace Text in PowerPoint', 'Search Text in PowerPoint PPT in Python']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Find-and-Replace-Text-in-PowerPoint.jpg" alt="Find and Replace Text in PowerPoint PPT in Python">}}


While processing digital documents, you often need to find and replace a specific text in the content. This could be required when a piece of information is to be censored before sharing the documents. To accomplish this programmatically, this article covers **how to find and replace text in PowerPoint [PPT][3] or [PPTX][4] in Python**.

*   [Python Library to Find and Replace Text in PowerPoint][5]
*   [Find and Replace Text in PPTX in Python][6]

**Info**: Aspose recently developed a free online [Text to GIF][7] service that allows you to animate texts or generate GIFs from simple texts.

## Python Library to Find and Replace Text in PowerPoint PPT {#API-to-Find-and-Replace-Text-in-PowerPoint}

[Aspose.Slides for Python via .NET][8] is an amazing library that simplifies the manipulation of PowerPoint presentations from within Python applications. Moreover, you can create rich presentations from scratch seamlessly. We will use this library to find and replace text inPPT/PPTX files. You can use the following pip command to install the library from [PyPI][9].

```
> pip install aspose.slides
```

## Find and Replace Text in PowerPoint PPT using Python {#Find-and-Replace-Text-in-PPTX}

To replace a particular piece of text in the presentation, you will have to go through the content of all the slides, which is quite easy using Aspose.Slides. The following are the steps to find and replace text in a PPTX presentation in Python.

*   First, load the PowerPoint PPT/PPTX using **Presentation** class.
*   Then, loop through the slides using **Presentation.slides** collection.
*   In each iteration, get text frames of the slide using **SlideUtil.get\_all\_text\_boxes(slide)** method.
*   Loop through text frames and in each iteration, perform the following operations:
    *   Loop through the paragraphs in the text frame.
    *   Access the text portions in each paragraph.
    *   Check if text portion contains the search string.
    *   If yes, find the position of the search string and replace the text.
*   Save the updated PPT using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to find and replace text in a PowerPoint PPTX in Python.

{{< gist aspose-com-gists 2d16793c6097e415c7603742f163acae "find-replace-text-in-ppt.py" >}}

The following screenshot shows the input PowerPoint presentation.



{{< figure align=center src="images/Find-and-Replace-Text-in-PowerPoint-PPT.png" alt="Find and Replace Text in PPT using Python">}}


Below is the screenshot of the resultant presentation after replacing the text.



{{< figure align=center src="images/Replace-Text-in-PowerPoint-PPT.png" alt="Replace Text in PowerPoint PPT in Python">}}


## Get a Free License {#Get-a-Free-API-License}

You can use Aspose.Slides for Python via .NET without evaluation limitations by requesting a [temporary license][10].

## Conclusion

In this article, you have learned how to find and replace text in PowerPoint PPT in Python. You can install Aspose.Slides and automate finding and replacing text from within your Python applications. Besides, you can read the [documentation][11] to explore more about Aspose.Slides for Python. Also, you can post your queries to our [forum][12].

## See Also

*   [Create PowerPoint Files in Python][13]
*   [Add Text or Image Watermark to PowerPoint PPT in Python][14]
*   [Apply Animation Effects to Text in PowerPoint PPT in Python][15]




[1]: https://docs.fileformat.com/presentation/ppt
[2]: https://docs.fileformat.com/presentation/pptx/
[3]: https://docs.fileformat.com/presentation/ppt
[4]: https://docs.fileformat.com/presentation/pptx/
[5]: #API-to-Find-and-Replace-Text-in-PowerPoint
[6]: #Find-and-Replace-Text-in-PPTX
[7]: https://products.aspose.app/slides/text-to-gif
[8]: https://products.aspose.com/slides/python-net
[9]: https://pypi.org/project/aspose.slides/
[10]: https://purchase.aspose.com/temporary-license
[11]: https://docs.aspose.com/slides/python-net/
[12]: https://forum.aspose.com/
[13]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[14]: https://blog.aspose.com/2022/02/09/add-watermark-to-powerpoint-ppt-in-python/
[15]: https://blog.aspose.com/2022/02/08/apply-text-animation-in-ppt-in-python/




