---
title: 'Add Text or Image Watermark to PowerPoint PPT in Python'
date: Wed, 09 Feb 2022 13:48:02 +0000
draft: false
url: /2022/02/09/add-watermark-to-powerpoint-ppt-in-python/
author: 'Usman Aziz'
summary: 'Watermarks are commonly used to protect a document or to specify its ownership. On the other hand, they are used to display the status of a document such as manuscript, draft, etc. In this article, we will demonstrate how to insert watermarks in PowerPoint presentations. You will learn **how to add text or image watermark to PowerPoint PPT slides in Python**.'
tags: ['Add Text Watermark to PPT Slides in Python', 'Insert Image Watermark to PPT Slides in Python', 'Python Library to Add Watermark to PowerPoint Slides', 'Remove Watermark from PPT in Python']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Add-Watermark-in-PowerPoint.jpg" alt="Add Watermark to PowerPoint PPT in Python">}}


Watermarks are commonly used to protect a document or to specify its ownership. On the other hand, they are used to display the status of a document such as manuscript, draft, etc. In this article, we will demonstrate how to insert watermarks in PowerPoint presentations. You will learn **how to add text or image watermark to PowerPoint PPT slides in Python**.

*   [Python Library to Add Watermark to PowerPoint Slides][1]
*   [Add Watermark to PPT Slides in Python][2]
    *   [Add Text Watermark to Slides][3]
    *   [Insert Image Watermark to Slides][4]
*   [Remove Watermark from PowerPoint PPT][5]

**Info**: You may want to check out the **free online tools** offered by Aspose.Slides to  [add watermarks][6] and [remove watermarks][7] from PowerPoint presentations.

## Python Library to Add Watermark to PowerPoint Slides {#API-to-Add-Watermark-to-PowerPoint-Slides}

To add or remove watermarks in PPT slides, we will use [Aspose.Slides for Python via .NET][8]. The library enables you to create and manipulate PowerPoint presentations seamlessly from within Python applications. Use the following pip command to install the library from [PyPI][9].

```
> pip install aspose.slides
```

## Add Watermark to PowerPoint PPT Slides in Python {#Add-Watermark-to-PPT-Slides-in-Python}

There are two types of watermark that can be added to PowerPoint slides: image and text. In image-based watermarking, an image is added to the PPT slides. Whereas, a text fragment is placed on the slides in case of text-based watermarking. The following sections explicitly cover both types of watermark.

### Add Text Watermark to PowerPoint Slides in Python {#Add-Text-Watermark-to-PowerPoint-Slides}

The following are the steps to add a text watermark to the PPT slides in Python.

*   First, load the PowerPoint PPT/PPTX using the **Presentation** class.
*   Get reference of the slide to which you want to add the watermark.
*   Calculate the position of the watermark.
*   Add a new auto shape for watermark using **add\_auto\_shape()** method.
*   Add text frame to the shape using **add\_text\_frame()** method.
*   Set font size, color, order and rotation angle of the watermark.
*   Lock watermark to avoid removal or modification.
*   Finally, save the updated PowerPoint file using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to add a text watermark to the PowerPoint slides.

{{< gist aspose-com-gists 5ad7480776c4d0d54a31cb34628415d8 "add-text-watermark-to-ppt-slide.py" >}}

To add the watermark to all the slides, you can either loop through the slides or add the watermark to the master slide, as shown in the following code sample.

{{< gist aspose-com-gists 5ad7480776c4d0d54a31cb34628415d8 "add-text-watermark-to-ppt.py" >}}

The following is the screenshot of the PowerPoint slide after adding the watermark.



{{< figure align=center src="images/Add-Text-Watermark-in-PowerPoint-PPT-Slide.png" alt="Add Text Watermark to PowerPoint Slides in Python">}}


### Add Image Watermark to PowerPoint Slides in Python {#Add-Image-Watermark-to-PowerPoint-Slides}

The following are the steps to add an image watermark to the PowerPoint slides in Python.

*   First, load the PowerPoint presentation using the **Presentation** class.
*   Get reference of the slide to which you want to add the watermark.
*   Calculate the position of the watermark.
*   Load the watermark image from file.
*   Add a new shape for watermark using **add\_auto\_shape()** method and set **shape.fill\_format.fill\_type** to **FillType.PICTURE**.
*   Set watermark image using **shape.fill\_format.picture\_fill\_format.picture.image** property.
*   Set order of watermark and lock it to avoid modification.
*   Finally, save the updated PPT using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to add an image watermark to PowerPoint slides.

{{< gist aspose-com-gists 5ad7480776c4d0d54a31cb34628415d8 "add-image-watermark-to-ppt.py" >}}

The following is the screenshot of the PPT slide after adding an image watermark.



{{< figure align=center src="images/Add-Image-Watermark-in-PowerPoint-PPT-Slide.png" alt="Add Image Watermark to PowerPoint Slides in Python">}}


## Remove Watermark from PPT Slides in Python {#Remove-Watermark-from-PowerPoint-PPT}

In the previous sections, you must have noticed that we have assigned a name to the watermark shapes. This name is used to filter the shapes that are used as a watermark. Thus, we can access, modify or remove the watermark shapes easily. The following code sample shows how to remove the watermarks that we have added to PPT slides in Python.

{{< gist aspose-com-gists 5ad7480776c4d0d54a31cb34628415d8 "remove-watermark.py" >}}

## Get a Free License {#Get-a-Free-API-License}

You can use Aspose.Slides for Python via .NET without evaluation limitations by requesting a [temporary license][10].

## Conclusion

In this article, you have learned how to add a watermark to the PowerPoint slides in Python. We have covered how to add text and image watermarks to PPT slides. Moreover, you have seen how to remove watermark from a PowerPoint PPT programmatically. In addition, you can read the [documentation][11] to explore other features of Aspose.Slides for Python. Also, you can post your queries to our [forum][12].

## See Also

*   [Create PowerPoint Files in Python][13]
*   [Convert PPTX to PDF in Python][14]
*   [Convert PPT to PNG in Python][15]
*   [PPT/PPTX to HTML in Python][16]




[1]: #API-to-Add-Watermark-to-PowerPoint-Slides
[2]: #Add-Watermark-to-PPT-Slides-in-Python
[3]: #Add-Text-Watermark-to-PowerPoint-Slides
[4]: #Add-Image-Watermark-to-PowerPoint-Slides
[5]: #Remove-Watermark-from-PowerPoint-PPT
[6]: https://products.aspose.app/slides/watermark
[7]: https://products.aspose.app/slides/watermark/remove-watermark
[8]: https://products.aspose.com/slides/python-net
[9]: https://pypi.org/project/aspose.slides/
[10]: https://purchase.aspose.com/temporary-license
[11]: https://docs.aspose.com/slides/python-net/
[12]: https://forum.aspose.com/
[13]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[14]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/
[15]: https://blog.aspose.com/2021/12/29/convert-ppt-to-png-in-python/
[16]: https://blog.aspose.com/2021/12/16/convert-ppt-to-html-in-python/




