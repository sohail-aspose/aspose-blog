---
title: 'Convert PPT to PNG in Python'
seoTitle: "Convert PPT to PNG in Python | Export PPTX PPT to PNG in Python"
description: "Use Python PowerPoint library to convert PPT or PPTX presentations to PNG in Python. Define your desired width and height for the converted PNG images."
date: Wed, 29 Dec 2021 16:52:59 +0000
draft: false
url: /2021/12/29/convert-ppt-to-png-in-python/
author: Usman Aziz
summary: 'Often, you may need to display the PowerPoint [PPTX][1] or [PPT][2] presentations in your Python applications. The easiest way to achieve this is the conversion of slides to [PNG][3] images. In this article, you will learn **how to convert PPT or PPTX to PNG images in Python**. Furthermore, we will discuss how to generate PNG images of custom scale or size programmatically.'
tags: ['Convert a PPT to PNG in Python', 'Custom Image Size in PPT to PNG Python', 'Image Scaling in PPTX to PNG Python', 'Python Library for PPT to PNG Conversion']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/PowerPoint-to-PNG-Image.jpg" alt="Convert PPT PPTX to PNG in Python">}}


Often, you may need to display the PowerPoint [PPTX][4] or [PPT][5] presentations in your Python applications. The easiest way to achieve this is the conversion of slides to [PNG][6] images. In this article, you will learn **how to convert PPT or PPTX to PNG images in Python**. Furthermore, we will discuss how to generate PNG images of custom scale or size programmatically.

*   [Python Library for PPT to PNG Conversion][7]
*   [Convert a PPT to PNG][8]
*   [Image Scaling in PPT to PNG][9]
*   [Custom Image Size in PPT to PNG][10]

**Info**: Using the API here, Aspose developed a free online [PPT to PNG][11] converter (that allows you to convert PowerPoint slide to PNG images) and [PNG to PPT][12] converter (that allows you to generate images based on slides in a presentation).

## Python Library to Convert PPT to PNG {#Python-Library-for-PPT-to-PNG-Conversion}

To convert the slides in PowerPoint presentations to PNG images, we will use [Aspose.Slides for Python via .NET][13]. It is a powerful Python library that lets you create and manipulate presentations seamlessly. Furthermore, it allows you to convert the presentations to other document and image formats. You can install the library from [PyPI][14] using the following pip command.

```
> pip install aspose.slides 
```

## Convert a PPT to PNG in Python {#Convert-a-PPT-to-PNG}

The following are the steps to convert a PPT file to PNG in Python.

*   Load the PPT file using [Presentation][15] class.
*   Start a loop to access each slide in the presentation.
*   Get reference of each [ISlide][16] from **Pesentation.slides** collection using index.
*   Convert slide to PNG using **ISlide.get\_thumbnail().save(string, ImageFormat.png)** method.

The following code sample shows how to convert a PPTX to PNG in Python.

{{< gist aspose-com-gists 1e1f217acbf403c0161746ff3e4f07d9 "ppt-to-png.py" >}}

## Image Scaling - Python PPTX to PNG {#Image-Scaling-in-PPTX-to-PNG}

In the previous section, we generated PNG images of default dimensions. However, in certain cases, you need to scale the images to the desired dimensions. You can achieve this by providing the X and Y values to the **get\_thumbnail()** method. The following are the steps to scale images in PPT to PNG conversion.

*   Load the PPTX file using [Presentation][17] class.
*   Create two variables to define X and Y values.
*   Start a loop to access each slide in the presentation.
*   Get reference of each [ISlide][18] from **Pesentation.slides** collection using index.
*   Convert slide to PNG using **ISlide.get\_thumbnail(scale\_x, scale\_y).save(string, ImageFormat.png)** method.

The following code sample generates PNG images from PPTX using custom dimensions in Python.

{{< gist aspose-com-gists 1e1f217acbf403c0161746ff3e4f07d9 "ppt-to-png-custom-scale.py" >}}

## Custom Image Size in PPTX to PNG Conversion {#Custom-Image-Size-in-PPTX-to-PNG}

You can also customize PPT to PNG conversion to generate images of desired width and height. The following are the steps to convert a PPT to PNG with custom image size in Python.

*   Load the PPT file using [Presentation][19] class.
*   Create a **Size** object containing width and height of the image.
*   Start a loop to access each slide in the presentation.
*   Get reference of each [ISlide][20] from **Pesentation.slides** collection using index.
*   Convert slide to PNG using **ISlide.get\_thumbnail(Size).save(string, ImageFormat.png)** method.

The following code sample shows how to convert a PPTX to PNG with custom image size in Python.

{{< gist aspose-com-gists 1e1f217acbf403c0161746ff3e4f07d9 "ppt-to-png-custom-size.py" >}}

## Get a Free License

You can use Aspose.Slides for Python via .NET without evaluation limitations by getting a [temporary license][21].

## Conclusion

PPT to PNG conversion could be useful in various scenarios such as when creating a PowerPoint slideshow. In this article, you have learned how to convert PPT or PPTX to PNG in Python. Furthermore, we have also covered how to scale the resultant images or generate images of desired width and height. You can explore other features of Aspose.Slides for Python via .NET using the [documentation][22]. In case you would have any queries, contact us on our [forum][23].

## See Also

*   [Convert PPTX to PDF in Python][24]




[1]: https://docs.fileformat.com/presentation/pptx/
[2]: https://docs.fileformat.com/presentation/ppt/
[3]: https://docs.fileformat.com/image/png/
[4]: https://docs.fileformat.com/presentation/pptx/
[5]: https://docs.fileformat.com/presentation/ppt/
[6]: https://docs.fileformat.com/image/png/
[7]: #Python-Library-for-PPT-to-PNG-Conversion
[8]: #Convert-a-PPT-to-PNG
[9]: #Image-Scaling-in-PPTX-to-PNG
[10]: #Custom-Image-Size-in-PPTX-to-PNG
[11]: https://products.aspose.app/slides/conversion/ppt-to-png
[12]: https://products.aspose.app/slides/import/jpg-to-ppt
[13]: https://products.aspose.com/slides/python-net/
[14]: https://pypi.org/project/aspose.slides/
[15]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/presentation/
[16]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/islide/
[17]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/presentation/
[18]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/islide/
[19]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/presentation/
[20]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/islide/
[21]: https://purchase.aspose.com/temporary-license
[22]: https://docs.aspose.com/slides/python-net
[23]: https://forum.aspose.com/
[24]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/




