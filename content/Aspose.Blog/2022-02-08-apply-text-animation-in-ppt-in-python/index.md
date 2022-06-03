---
title: 'Apply Animation Effects to Text in PowerPoint PPT using Python'
date: Tue, 08 Feb 2022 17:26:00 +0000
draft: false
url: /2022/02/08/apply-text-animation-in-ppt-in-python/
author: ''Usman Aziz''
summary: 'MS PowerPoint provides various animation effects which are used to make the presentations interesting and draw the attention of the viewers. These animations can be applied to slides, text, shapes, or other elements. In this article, we will focus on animating text in a PowerPoint PPT. Particularly, you will learn **how to apply and retrieve text animation programmatically in Python**.'
tags: ['Apply Animation to Text in PowerPoint', 'Create animated text in PowerPoint PPT in Python', 'Get Animation Effects from a Text in PowerPoint', 'Python Library to Apply Animation to Text in PowerPoint']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Apply-Animation-Effects-to-Text-in-PPT.png" alt="Apply Animation Effects to Text in PowerPoint PPT using Python">}}


MS PowerPoint provides various animation effects which are used to make the presentations interesting and draw the attention of the viewers. These animations can be applied to slides, text, shapes, or other elements. In this article, we will focus on animating text in a PowerPoint PPT. Particularly, you will learn **how to apply and retrieve text animation programmatically in Python**.

*   [Python Library to Apply Animation to Text in PowerPoint][1]
*   [Apply Animation to Text in PowerPoint][2]
*   [Get Animation Effects from a Text in PowerPoint][3]

## Python Library to Apply Animation to Text in PPT {#API-to-Apply-Animation-to-Text-in-PowerPoint}

To apply animation to the text in PowerPoint presentations, we will use [Aspose.Slides for Python via .NET][4]. It is a feature-rich library that is designed to create and manipulate PPT and PPTX presentations. Use the following pip command to install the library from [PyPI][5].

```
> pip install aspose.slides 
```

## Apply Animation to Text in PowerPoint PPT in Python {#Apply-Animation-to-Text-in-PowerPoint}

There are over 150 animation effects that Aspose.Slides for Python supports, such as Bounce, PathFootball, Zoom, etc. In addition, you can also use specific animation effects such as OLEObjectShow and OLEObjectOpen. You can view the complete list of animations in [EffectType][6] enumeration.

The following are the steps to apply animation to text in a PowerPoint PPT using Python.

*   First, load the PPT/PPTX file using **Presentation** class.
*   Then, get reference of the paragraph to which you want to apply animation.
*   Apply animation effect using **Presentation.slides\[index\].timeline.main\_sequence.add\_effect()** method.
*   Finally, save the presentation using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to apply an animation effect to text in a PowerPoint PPT.

{{< gist aspose-com-gists 295bab13c921469e6d04b78223bf4704 "apply-text-animation.py" >}}

## Get Animation Effects from a Text in PowerPoint {#Get-Animation-Effects-from-a-Text-in-PowerPoint}

There could be the case when you need to replicate the animation from one text to another. In that case, you can get information about the animation effect applied to a particular text.

The following are the steps to get information about the animation effect applied to a text in Python.

*   First, load the presentation using **Presentation** class.
*   Then, get sequence of the desired slide in an object.
*   Access the desired shape from the slide in an object.
*   Loop through each paragraph in **shape.text\_frame.paragraph** collection.
*   Finally, get the effects using **sequence.get\_effects\_by\_paragraph()** method.

The following code sample shows how to get the information of an animation effect in PPT.

{{< gist aspose-com-gists 295bab13c921469e6d04b78223bf4704 "get-text-animation.py" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for Python via .NET without evaluation limitations by getting a [temporary license][7].

## Conclusion

In this article, you have learned how to apply animation effects on text in PowerPoint PPT using Python. Furthermore, you have seen how to get animation effects from a particular text in a PPT/PPTX. Besides, you can explore other features of Aspose.Slides for Python using [documentation][8]. Moreover, you can feel free to let us know about your queries via our [forum][9].

## See Also

*   [Create PowerPoint Files in Python][10]
*   [Convert PPTX to PDF in Python][11]
*   [Convert PPT to PNG in Python][12]
*   [PPT/PPTX to HTML in Python][13]




[1]: #API-to-Apply-Animation-to-Text-in-PowerPoint
[2]: #Apply-Animation-to-Text-in-PowerPoint
[3]: #Get-Animation-Effects-from-a-Text-in-PowerPoint
[4]: https://products.aspose.com/slides/python-net
[5]: https://pypi.org/project/aspose.slides/
[6]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides.animation/effecttype/
[7]: https://purchase.aspose.com/temporary-license
[8]: https://docs.aspose.com/slides/python-net/
[9]: https://forum.aspose.com/
[10]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[11]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/
[12]: https://blog.aspose.com/2021/12/29/convert-ppt-to-png-in-python/
[13]: https://blog.aspose.com/2021/12/16/convert-ppt-to-html-in-python/




