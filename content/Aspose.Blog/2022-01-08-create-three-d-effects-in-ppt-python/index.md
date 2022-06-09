---
title: 'Apply 3D Effects in PowerPoint PPT using Python'
seoTitle: "Apply 3D Effects in PowerPoint in Python | Create 3D Text Shape Image"
description: "Use Python PowerPoint API to apply 3D effects in PPT or PPTX presentations. Apply 3D effects to text, shapes and images in PowerPoint programmatically."
date: Sat, 08 Jan 2022 06:08:00 +0000
draft: false
url: /2022/01/08/create-three-d-effects-in-ppt-python/
author: Usman Aziz
summary: 'MS PowerPoint provides 3D effects to make the presentations more attractive. You can use 3D text, shapes, and images to enhance the interactivity of the content. In this article, you will learn **how to apply the 3D effects in PowerPoint PPT programmatically in Python**. We will cover how to create 3D effects for text, shapes, and images in the presentations.'
tags: ['Apply 3D Effects to an Image in PowerPoint Python', 'Create a 3D Shape in PowerPoint in Python', 'Create a 3D Text in PowerPoint in Python', 'Python Library to Create 3D Effects in PowerPoint']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Apply-3D-Effects-in-PowerPoint.psd_.png" alt="Apply 3D Effects in PowerPoint using Python">}}


MS PowerPoint provides 3D effects to make the presentations more attractive. You can use 3D text, shapes, and images to enhance the interactivity of the content. In this article, you will learn **how to apply the 3D effects in PowerPoint PPT programmatically in Python**. We will cover how to create 3D effects for text, shapes, and images in the presentations.

*   [Python Library to Create 3D Effects in PowerPoint][1]
*   [Create a 3D Text in PowerPoint in Python][2]
*   [Create a 3D Shape in PowerPoint in Python][3]
*   [Set Gradient for 3D Shapes][4]
*   [Apply 3D Effects to an Image in PowerPoint][5]

## Python Library to Apply 3D Effects in PowerPoint {#API-to-Create-3D-Effects-in-PowerPoint}

[Aspose.Slides for Python via .NET][6] is a feature-rich Python library that is designed to create and manipulate PowerPoint presentations. We will use this library to apply 3D effects in the PowerPoint PPT/PPTX presentations. Use the following command to install the library from [PyPI][7].

```
> pip install aspose.slides
```

## Create a 3D Text in PowerPoint in Python {#Create-a-3D-Text-in-PowerPoint}

The following are the steps to create a 3D text fragment in PowerPoint PPT using Python.

*   First, create a new PPT or load existing one using **Presentation** class.
*   Then, add a new rectangle shape using **add\_auto\_shape()** method.
*   Set shape's properties such as fill type, text, etc.
*   Get reference of the text portion inside shape into an object.
*   Apply formatting to the text portion.
*   Get reference of the **text\_frame** inside shape.
*   Apply 3D effects using properties in **text\_frame.text\_frame\_format.three\_dformat**.
*   Finally, save presentation using **Presentation.save(String, SaveFormat)** method.

The following code sample shows how to create a 3D text in PowerPoint in Python.

{{< gist aspose-com-gists c320d27a1615976b33ff7a7c8e229c13 "create-3d-text-in-ppt.py" >}}

The following screenshot shows the output of the code sample above.



{{< figure align=center src="images/Create-3D-Text-in-PPT.png" alt="Create a 3D Text in PowerPoint in python">}}


## Create a 3D Shape in PowerPoint in Python {#Create-a-3D-Shape-in-PowerPoint}

Similar to text, you can apply 3D effects to the shapes in PowerPoint presentations. The following are the steps to create a 3D shape in PowerPoint in Python.

*   First, create a new PPT using **Presentation** class.
*   Then, add a new rectangle shape using **add\_auto\_shape()** method.
*   Set shape's text using **shape.text\_frame.text** property.
*   Apply 3D effects to shape using properties in **shape.three\_dformat**.
*   Finally, save presentation using **Presentation.save(String, SaveFormat)** method.

The following code sample shows how to apply 3D effects to shapes in PowerPoint using Python.

{{< gist aspose-com-gists c320d27a1615976b33ff7a7c8e229c13 "create-3d-shape-in-ppt.py" >}}

The following is the 3D shape that we get after executing this code.



{{< figure align=center src="images/Create-3D-Shape-in-PPT.png" alt="Create a 3D Shape in PowerPoint in Python">}}


## Create Gradient for 3D Shapes {#Set-Gradient-for-3D-Shapes}

You can also apply gradient effects to the shapes following the steps below.

*   First, create a new PPT using **Presentation** class.
*   Then, add a new rectangle shape using **add\_auto\_shape()** method.
*   Set shape's text using **shape.text\_frame.text** property.
*   Set **shape.fill\_format.fill\_type** to **FillType.GRADIENT** and set gradient colors.
*   Apply 3D effects to shape using properties in **shape.three\_dformat**.
*   Finally, save presentation using **Presentation.save(String, SaveFormat)** method.

The following code sample shows how to apply gradient effects to shapes in PowerPoint.

{{< gist aspose-com-gists c320d27a1615976b33ff7a7c8e229c13 "create-3d-shape-gradient-in-ppt.py" >}}

The following is the 3D shape after applying the gradient effect.



{{< figure align=center src="images/Create-3D-Shape-Gradient-in-PowerPoint.png" alt="Create Gradient for 3D Shapes in PPT">}}


## Apply 3D Effects to an Image in PowerPoint in Python {#Apply-3D-Effect-to-an-Image-in-PowerPoint}

You can also apply 3D effects to the images in the PowerPoint presentations. The following are the steps to perform this operation in Python.

*   Create a new PPT using **Presentation** class.
*   Then, add a new rectangle shape using **add\_auto\_shape()** method.
*   Set **shape.fill\_format.fill\_type** to **FillType.PICTURE** and add image.
*   Apply 3D effects to shape using properties in **shape.three\_dformat**.
*   Save presentation using **Presentation.save(String, SaveFormat)** method.

The following are the steps to apply 3D effects to an image in PPT using Python.

{{< gist aspose-com-gists c320d27a1615976b33ff7a7c8e229c13 "create-3d-image-in-ppt.py" >}}

The following is the resultant image that we get after applying 3D effects.



{{< figure align=center src="images/Create-3D-Image-in-PowerPoint-PPT.png" alt="Apply 3D Effects to an Image in PowerPoint in Python">}}


## Get a Free License

You can get a [free temporary license][8] to use Aspose.Slides for Python via .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to apply 3D effects in PowerPoint presentations using Python. We have covered how to create 3D text or shapes and apply 3D effects to images in PPT or PPTX presentations. In case you want to explore more about Aspose.Slides for Python via .NET, you can visit the [documentation][9]. Also, you can post your queries to our [forum][10].

## See Also

*   [Create PowerPoint Files in Python][11]
*   [Convert PPTX to PDF in Python][12]
*   [Convert PPT to PNG in Python][13]
*   [PPT/PPTX to HTML in Python][14]




[1]: #API-to-Create-3D-Effects-in-PowerPoint
[2]: #Create-a-3D-Text-in-PowerPoint
[3]: #Create-a-3D-Shape-in-PowerPoint
[4]: #Set-Gradient-for-3D-Shapes
[5]: #Apply-3D-Effect-to-an-Image-in-PowerPoint
[6]: https://products.aspose.com/slides/python-net
[7]: https://pypi.org/project/aspose.slides/
[8]: https://purchase.aspose.com/temporary-license
[9]: https://docs.aspose.com/slides/python-net/
[10]: https://forum.aspose.com/
[11]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[12]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/
[13]: https://blog.aspose.com/2021/12/29/convert-ppt-to-png-in-python/
[14]: https://blog.aspose.com/2021/12/16/convert-ppt-to-html-in-python/




