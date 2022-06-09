---
title: 'Split PowerPoint PPT Slides in Python'
seoTitle: "Split Slides in PPT using Python | Python PowerPoint PPT Splitter"
description: "Use Python PowerPoint library to split slides in PPT or PPTX in Python. Split each slide in the presentation and save it as a separate PPT or PPTX."
date: Thu, 23 Dec 2021 13:21:00 +0000
draft: false
url: /2021/12/23/split-ppt-slides-in-python/
author: Usman Aziz
summary: 'While manipulating the PowerPoint presentations programmatically, you may need to split the slides and save them as separate PPT files. For example, you may want to split each slide, all odd or even slides, and so on. In this article, you will learn **how to split slides in PowerPoint [PPT][1] or [PPTX][2] in Python**.'
tags: ['Python Library to Split PowerPoint PPT', 'Python PowerPoint PPT Splitter', 'Split PPT into Multiple Files in Python', 'Split Slides in a PPT using Python']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Split-PowerPoint-Presentation.jpg" alt="Split Slides in PowerPoint PPT or PPTX in Python">}}


While manipulating the PowerPoint presentations programmatically, you may need to split the slides and save them as separate PPT files. For example, you may want to split each slide, all odd or even slides, and so on. In this article, you will learn **how to split slides in PowerPoint [PPT][3] or [PPTX][4] in Python**.

*   [Python Library to Split PowerPoint PPT][5]
*   [Split Slides in a PowerPoint PPT][6]

**Info**: Aspose provides a free [online PowerPoint Splitter][7], which is a live implementation of the presentation splitting process described on this page.

## Python Library to Split PowerPoint PPT {#Python-Library-to-Split-PowerPoint-PPT}

[Aspose.Slides for Python via .NET][8] is a feature-rich Python library that allows you to create and manipulate PowerPoint presentations. Moreover, it lets you convert the presentations to other formats seamlessly. We will use this library to split the slides in PowerPoint PPT. You can install the library from [PyPI][9] using the following pip command.

```
> pip install aspose.slides 
```

## Split PowerPoint PPT Slides in Python {#Split-Slides-in-a-PPT-using-Python}

Aspose.Slides for Python makes it quite easier for you to split a presentation. Just load the presentation file, loop through slides, and save each slide as a separate PPT/PPTX file. The following are the steps to split slides in a PowerPoint PPT in Python.

*   First, load the presentation using [Presentation][10] class.
*   Loop through number of slides and in each iteration, perform following steps:
    *   Create a new presentation using **Presentation** class.
    *   Remove the default slide in the presentation using **ISlide.remove()** method.
    *   Add a clone of the slide using **Presentation.slides.add\_clone(ISlide)** method.
    *   Save presentation using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to split slides in a PowerPoint PPTX using Python.

{{< gist aspose-com-gists ede3f01641aca14a3dbda2812f54e67e "split-ppt.py" >}}

## Get a Free License

You can use Aspose.Slides for Python via .NET without evaluation limitations by getting a [temporary license][11].

## Conclusion

In this article, you have seen how to split slides in a PowerPoint PPT using Python. You can modify the provided code sample to change the splitting criteria as per your requirements, such as splitting all even or odd slides, etc. To explore more about Aspose.Slides for Python via .NET, you can visit the [documentation][12]. Also, you can share your queries with us via our [forum][13].

## See Also

*   [Convert PPTX to PDF in Python][14]
*   [Create PowerPoint Presentations in Python][15]
*   [Convert PPT to PNG in Python][16]
*   [Convert PPT to JPG in Python][17]




[1]: https://docs.fileformat.com/presentation/ppt/
[2]: https://docs.fileformat.com/presentation/pptx/
[3]: https://docs.fileformat.com/presentation/ppt/
[4]: https://docs.fileformat.com/presentation/pptx/
[5]: #Python-Library-to-Split-PowerPoint-PPT
[6]: #Split-Slides-in-a-PPT-using-Python
[7]: https://products.aspose.app/slides/splitter
[8]: https://products.aspose.com/slides/python-net/
[9]: https://pypi.org/project/aspose.slides/
[10]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/presentation/
[11]: https://purchase.aspose.com/temporary-license
[12]: https://docs.aspose.com/slides/python-net
[13]: https://forum.aspose.com/
[14]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/
[15]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[16]: https://blog.aspose.com/2021/12/29/convert-ppt-to-png-in-python/
[17]: https://blog.aspose.com/2021/12/03/convert-ppt-to-jpg-in-python/




