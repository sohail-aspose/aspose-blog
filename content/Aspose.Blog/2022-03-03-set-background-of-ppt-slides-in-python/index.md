---
title: 'Set Background of PowerPoint PPT Slides in Python'
seoTitle: "Python: Set Background Image or Color of Slide in PowerPoint PPT PPTX"
description: "Use Python PowerPoint library to set the slide background color or image in PPT/PPTX presentations using Python. Download source code."
date: Thu, 03 Mar 2022 15:12:00 +0000
draft: false
url: /2022/03/03/set-background-of-ppt-slides-in-python/
author: Usman Aziz
summary: "PowerPoint allows you to set different types of slide backgrounds in the presentations. For example, you can set an image, a solid color, etc. as background. In this article, we will show you **how to set the background of PowerPoint PPT slides in Python**. We will explicitly cover how to fill a PPT slide's background with an image, color, or a gradient programmatically."
tags: ['Python Library to Set Slide Background in PowerPoint', 'Set Background Color of PPT Slides Python', 'Set Background Image of PPT Slides Python', 'Set Gradient of PPT Slide in Python']
categories: ['Aspose.Slides Product Family']
---

PowerPoint allows you to set different types of slide backgrounds in the presentations. For example, you can set an image, a solid color, etc. as background. In this article, we will show you **how to set the background of PowerPoint PPT slides in Python**. We will explicitly cover how to fill a PPT slide's background with an image, color, or a gradient programmatically.

*   [Python Library to Set Slide Background in PowerPoint][1]
*   [Set Background Image of PPT Slides][2]
*   [Set Background Color of Slides][3]
*   [Apply Background Color to Master Slide][4]
*   [Set Gradient as Slide Background][5]

## Python Library to Set Slide Background in PowerPoint {#API-to-Set-Slide-Background-in-PowerPoint}

[Aspose.Slides for Python][6] is a popular and feature-rich library to create and manipulate PowerPoint presentations. We will utilize this library to set slide backgrounds in our PowerPoint presentations. To install the library from [PyPI][7], you can use the following command.

```
> pip install aspose.slides
```

## Set Image as PPT Slide Background in Python {#Set-Background-Image-of-PPT-Slides}

The following are the steps to set a background image in a PowerPoint PPT/PPTX slide in Python.

*   First, use **Presentation** class to load or create the PPT/PPTX presentation.
*   Then, get reference of the desired slide from **Presentation.slides** collection.
*   Set slide background's fill type to **FillType.PICTURE**.
*   Set fill mode of picture to **PictureFillMode.STRETCH**.
*   Add image to the collection of presentation using **Presentation.images.add\_image()** method.
*   Set background image of the slide using **Slide.background.fill\_format.picture\_fill\_format.picture.image** property.
*   Finally, save the updated presentation using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to set background image of PowerPoint PPT slides in Python.

{{< gist aspose-com-gists b5506333713a0aa636c76d6f1ffa4748 "set-slide-background-image.py" >}}

The following screenshot shows the resultant PPT slide after adding background image.



{{< figure align=center src="images/Set-PPT-Slide-Background-Image.png" alt="Set Image as PPT Slide Background in Python">}}


## Set Background Color of PPT Slides in Python {#Set-Background-Color-of-Normal-Slides}

The following are the steps to set the background color of the slides in a PowerPoint PPT using Python.

*   First, load or create the PowerPoint PPT/PPTX using **Presentation** class.
*   Set slide background's fill type to **FillType.SOLID**.
*   Then, set the background color of slide using **Slide.background.fill\_format.solid\_fill\_color.color** property.
*   Finally, save the updated presentation using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to set the background color of a PPT slide in Python.

{{< gist aspose-com-gists b5506333713a0aa636c76d6f1ffa4748 "set-slide-background-color.py" >}}

## Set Background Color of Master Slide in Python {#Set-Background-Color-of-Master-Slide}

You can also set the background of the master slide that will be applied to all the slides in the presentation. The following are the steps to change the background color of the master slide in Python.

*   First, load or create the PowerPoint PPT/PPTX using **Presentation** class.
*   Set master slide background's fill type to **FillType.SOLID**.
*   Then, set the background color of master slide using **MasterSlide.background.fill\_format.solid\_fill\_color.color** property.
*   Finally, save the updated presentation using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to change the background color of the master slide in PowerPoint PPT.

{{< gist aspose-com-gists b5506333713a0aa636c76d6f1ffa4748 "set-master-background-color.py" >}}

## Set Gradient as PPT Slide Background in Python {#Gradient-as-Slide-Background-Color}

You can also set the gradient background of the PPT slides using Aspose.Slides for Python, as demonstrated in the steps below.

*   First, load or create the PowerPoint PPT/PPTX using **Presentation** class.
*   Set slide background's fill type to **FillType.GRADIENT**.
*   Then, set the background gradient format using **Slide.background.fill\_format.gradient\_format.tile\_flip** property.
*   Finally, save the updated presentation using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to set the gradient background of PPT slides in Python.

{{< gist aspose-com-gists b5506333713a0aa636c76d6f1ffa4748 "set-slide-background-gradient.py" >}}

The following screenshot shows the gradient background of the slide.



{{< figure align=center src="images/Set-PPT-Slide-Background-Gradient.png" alt="Set Gradient Background Color of Slides in Python">}}


## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for Python without evaluation limitations by requesting a??[temporary license][8].

## Conclusion

In this article, you have learned how to set the background color or image of slides in PowerPoint PPT using Python. Furthermore, you have seen how to set gradient background of normal or master slides in PowerPoint presentations. You can visit the??[documentation][9]??to explore other features of Aspose.Slides for Python. Also, you can feel free to let us know about your queries via our??[forum][10].

## See Also

*   [Create PowerPoint Files in Python][11]
*   [Convert PPTX to PDF in Python][12]
*   [Convert PPT to PNG in Python][13]
*   [Add Watermark in PowerPoint PPT in Python][14]
*   [Apply 3D Effects in PowerPoint PPT using Python][15]




[1]: #API-to-Set-Slide-Background-in-PowerPoint
[2]: #Set-Background-Image-of-PPT-Slides
[3]: #Set-Background-Color-of-Normal-Slides
[4]: #Set-Background-Color-of-Master-Slide
[5]: #Gradient-as-Slide-Background-Color
[6]: https://products.aspose.com/slides/python-net/
[7]: https://pypi.org/project/aspose.slides/
[8]: https://purchase.aspose.com/temporary-license
[9]: https://docs.aspose.com/slides/python-net/
[10]: https://forum.aspose.com/
[11]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[12]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/
[13]: https://blog.aspose.com/2021/12/29/convert-ppt-to-png-in-python/
[14]: https://blog.aspose.com/2022/02/09/add-watermark-to-powerpoint-ppt-in-python/
[15]: https://blog.aspose.com/2022/01/08/create-three-d-effects-in-ppt-python/




