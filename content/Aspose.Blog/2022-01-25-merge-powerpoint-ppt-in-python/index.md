---
title: 'Merge PowerPoint Presentations in Python'
seoTitle: "Merge PowerPoint PPT in Python | Merge Multiple PPT/PPTX | Python Lib"
description: "Merge or combine PowerPoint PPT/PPTX presentations using Python. Merge all or selected slides from one PowerPoint PPT to other programmatically."
date: Tue, 25 Jan 2022 15:32:08 +0000
draft: false
url: /2022/01/25/merge-powerpoint-ppt-in-python/
author: Usman Aziz
summary: 'While working with PowerPoint automation in Python, you may need to merge the content of multiple presentations. This could be required when a presentation is created by multiple people in parts that need to be merged eventually. To automate this merging, this article shows **how to merge PowerPoint [PPT][1] or [PPTX][2] programmatically in Python**.'
tags: ['Combine PPT with Different Slide Sizes in Python', 'Merge PPT Slides to a Specific Section in Python', 'Merge PowerPoint Presentations in Python', 'Python PowerPoint Merger Library']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Merge-PowerPoint-files.jpg" alt="Merge PowerPoint files in Python">}}


While working with PowerPoint automation in Python, you may need to merge the content of multiple presentations. This could be required when a presentation is created by multiple people in parts that need to be merged eventually. To automate this merging, this article shows **how to merge PowerPoint [PPT][3] or [PPTX][4] programmatically in Python**.

*   [Python PowerPoint Merger Library][5]
*   [Merge PowerPoint Presentations][6]
*   [Combine Presentations with Different Slide Sizes][7]
*   [Merge PPT Slides to a Specific Section][8]
*   [Use Slide Master while Merging PowerPoint Presentations][9]

## Python Library to Merge PowerPoint PPT {#PowerPoint-Merger-API}

[Aspose.Slides for Python via .NET][10] is a powerful Python library for creating and manipulating presentation files. Moreover, it provides flexible ways to merge multiple PPT/PPTX presentations. We will utilize this library to merge presentations in this article. You can install it from [PyPI][11] using the following pip command.

```
> pip install aspose.slides
```

## Merge PowerPoint Presentations in Python {#Merge-PowerPoint-Presentations}

To merge the PPT presentations, you will need to clone the slides from one presentation to the other. The following are the steps to merge two PPT files in Python.

*   Create an object of **Presentation** class to load the first presentation.
*   Create another **Presentation** object to load the second presentation.
*   Start a loop to iterate through the slides in the second presentation.
*   In each iteration, merge the slide to first presentation using **Presentation.slides.add\_clone(ISlide)** method.
*   Finally, save the merged presentation using **Presentation.save(String, SaveFormat)** method.

The following code sample shows how to merge two PowerPoint PPTX presentations in Python.

{{< gist aspose-com-gists 603b0e997ea07b37a82d910a1c03d3b1 "merge-ppt.py" >}}

### First Presentation



{{< figure align=center src="images/merge-presentation1.jpg" alt="target powerpoint presentation">}}


### Second Presentation



{{< figure align=center src="images/merge-presentation2.jpg" alt="source powerpoint presentation to be merged">}}


### Merged Presentation



{{< figure align=center src="images/merged-presentation.jpg" alt="merged  powerpoint ppt in python">}}


## Merge Presentations with Different Slide Sizes {#Combine-Presentations-with-Different-Slide-Sizes}

It is possible that the presentations you are going to merge use different sizes for their slides. In such cases, it is better to synchronize the size of the slides before merging. Let's see how to merge PowerPoint PPT files having different slide sizes.

*   Create an object of **Presentation** class to load the first PPT.
*   Create another **Presentation** object to load the second PPT.
*   Change size of slides in second PPT using **Presentation.slide\_size.set\_size(int, int, SlideSizeScaleType)** method.
*   Start a loop to iterate through the slides in the second PPT.
*   In each iteration, merge the slide to first PPT using **Presentation.slides.add\_clone(ISlide)** method.
*   Finally, save the merged PPT using **Presentation.save(String, SaveFormat)** method.

The following code sample shows how to merge PPT presentations having different slide sizes.

{{< gist aspose-com-gists 603b0e997ea07b37a82d910a1c03d3b1 "merge-ppt-size.py" >}}

## Merge PPT Slides to a Specific Section in Python {#Merge-PPT-Slides-to-a-Specific-Section}

You can also merge PPT slides to a specific section of the target presentation. For this, **Presentation.slides.add\_clone(ISlide, ISection)** method is used. The following code sample shows how to merge slides from the first presentation to a particular section of the second presentation.

{{< gist aspose-com-gists 603b0e997ea07b37a82d910a1c03d3b1 "merge-ppt-section.py" >}}

## Use Slide Master while Merging PowerPoint PPT {#Use-Slide-Master-while-Merging-PowerPoint-Presentations}

In the previous sections, we have merged the slides keeping the design and template of the second PPT. However, we may need to use the layout of the first (or destination) presentation for the cloned slides. In such cases, the overloaded method **Presentation.slides.add\_clone(ISlide, Presentation.masters\[int\], allow\_clone\_missing\_layout = True)** is used where second parameter defines the slide master.

The following code sample shows how to merge PPT presentations using desired slide master in Python.

{{< gist aspose-com-gists 603b0e997ea07b37a82d910a1c03d3b1 "merge-ppt-master.py" >}}

### Merged Presentation



{{< figure align=center src="images/merged-presentation-slide-master.jpg" alt="combined powerpoint ppt in python">}}


## Get a Free License

You can get a [free temporary license][12] to use Aspose.Slides for Python via .NET without evaluation limitations.

**Info**: Aspose free [online PowerPoint Merger][13] is a live implementation of the presentation merging process as a service.

## Conclusion

In this article, you have learned how to merge PowerPoint PPT/PPTX presentations in Python. We have covered various scenarios of merging multiple PowerPoint presentations with the help of code samples. You can simply install the library and use the provided code samples in your applications. In case you want to explore more about Aspose.Slides for Python, you can visit the [documentation][14]. Also, you can ask your questions via our [forum][15].

## See Also

*   [Create PowerPoint Files in Python][16]
*   [Convert PPTX to PDF in Python][17]
*   [Convert PPT to PNG in Python][18]
*   [PPT/PPTX to HTML in Python][19]




[1]: https://docs.fileformat.com/presentation/ppt/
[2]: https://docs.fileformat.com/presentation/pptx/
[3]: https://docs.fileformat.com/presentation/ppt/
[4]: https://docs.fileformat.com/presentation/pptx/
[5]: #PowerPoint-Merger-API
[6]: #Merge-PowerPoint-Presentations
[7]: #Combine-Presentations-with-Different-Slide-Sizes
[8]: #Merge-PPT-Slides-to-a-Specific-Section
[9]: #Use-Slide-Master-while-Merging-PowerPoint-Presentations
[10]: https://products.aspose.com/slides/python-net
[11]: https://pypi.org/project/aspose.slides/
[12]: https://purchase.aspose.com/temporary-license
[13]: https://products.aspose.app/slides/merger
[14]: https://docs.aspose.com/slides/python-net
[15]: https://forum.aspose.com/
[16]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[17]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/
[18]: https://blog.aspose.com/2021/12/29/convert-ppt-to-png-in-python/
[19]: https://blog.aspose.com/2021/12/16/convert-ppt-to-html-in-python/




