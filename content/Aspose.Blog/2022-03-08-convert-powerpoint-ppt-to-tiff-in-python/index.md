---
title: 'Convert PowerPoint PPT/PPTX to TIFF in Python'
date: Tue, 08 Mar 2022 11:00:34 +0000
draft: false
url: /2022/03/08/convert-powerpoint-ppt-to-tiff-in-python/
author: ''Usman Aziz''
summary: '[TIFF][1] is a popular format that is used for the conversion of PowerPoint presentations to image format. This conversion could be useful for generating thumbnails of the PPT slides. In this article, you will learn **how to convert PowerPoint PPT or PPTX to TIFF using Python**. Furthermore, you will learn how to customize PPT to TIFF conversion using different options.'
tags: ['Convert PPT to TIFF in Python', 'Convert PPTX to TIFF in Python', 'Generate PPT Thumbnails in Python', 'Python PowerPoint to TIFF Converter']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/PowerPoint-to-TIFF.jpg" alt="PowerPoint PPT to TIFF in Python">}}


[TIFF][2] is a popular format that is used for the conversion of PowerPoint presentations to image format. This conversion could be useful for generating thumbnails of the PPT slides. In this article, you will learn **how to convert PowerPoint PPT or PPTX to TIFF using Python**. Furthermore, you will learn how to customize PPT to TIFF conversion using different options.

*   [Python PowerPoint to TIFF Converter][3]
*   [Convert PowerPoint PPT to TIFF][4]
*   [Convert PPT to TIFF with Hidden Slides][5]
*   [PowerPoint to TIFF with Custom Image Size][6]
*   [PPT to TIFF with Custom Pixel Format][7]

## Python PowerPoint PPT to TIFF Converter {#PowerPoint-to-TIFF-Converter}

[Aspose.Slides for Python][8] provides high fidelity conversion of PowerPoint presentations to various popular image and document formats. We will use this library to convert our PPT/PPTX presentations to TIFF format. You can install the library from [PyPI][9] using the following command.

```
> pip install aspose.slides
```

## Convert PowerPoint PPTX to TIFF in Python {#Convert-PowerPoint-to-TIFF}

The conversion of PowerPoint PPT/PPTX to TIFF can be done in a couple of lines of code using Aspose.Slides for Python, as demonstrated below.

*   Load the PowerPoint PPT/PPTX using **Presentation** class.
*   Save presentation as TIFF using **Presentation.save(string, SaveFormat.TIFF)** method.

The following code sample shows how to convert a PowerPoint PPTX file to TIFF in Python.

{{< gist aspose-com-gists 1fa402fc19dcf41f6a169d63cabee21d "powerpoint-to-tiff.py" >}}

## Convert PPT to TIFF with Hidden Slides in Python {#Convert-PPT-to-TIFF-with-Hidden-Slides-in-Python}

Often, the PowerPoint presentations contain hidden slides, which are not included in PPT to TIFF conversion by default. However, you can enable the rendering of hidden slides as demonstrated below.

*   First, load the PowerPoint PPT/PPTX using **Presentation** class.
*   Then, create an instance of **TiffOptions** class.
*   Set **TiffOptions.show\_hidden\_slides** property to **True**.
*   Save presentation as TIFF using **Presentation.save(string, SaveFormat.TIFF, TiffOptions)** method.

The following code sample shows how to include hidden slides in PPT to TIFF conversion.

{{< gist aspose-com-gists 1fa402fc19dcf41f6a169d63cabee21d "powerpoint-to-tiff-hidden-slides.py" >}}

## PPT to TIFF - Customize Compression and Image Size {#Convert-PowerPoint-to-TIFF-with-Custom-Image-Size}

You can also customize the size of resultant TIFF images during the conversion. Moreover, you can change the default compression type of the converted TIFF image. The following steps show how to set compression type and image size in PowerPoint PPT to TIFF conversion.

*   First, load the PowerPoint PPT/PPTX using **Presentation** class.
*   Then, create an instance of **TiffOptions** class.
*   Set image dimensions using **TiffOptions.image\_size** property.
*   Set compression type using **TiffOptions.compression\_type** property.
*   Convert PPT to TIFF using **Presentation.save(string, SaveFormat.TIFF, TiffOptions)** method.

The following code sample shows how to convert PPTX to TIFF with custom image size and compression.

{{< gist aspose-com-gists 1fa402fc19dcf41f6a169d63cabee21d "powerpoint-to-tiff-image-size.py" >}}

## Python PowerPoint to TIFF with Custom Pixel Format {#PPTX-to-TIFF-with-Custom-Pixel-Format}

Aspose.Slides for Python also allows you to set the pixel format of the resultant TIFF image. This can be achieved by following the steps below.

*   Load the PPT/PPTX presentation using **Presentation** class.
*   Create an instance of **TiffOptions** class.
*   Set [desired pixel format][10] using **TiffOptions.pixel\_format** property.
*   Convert presentation to TIFF using **Presentation.save(string, SaveFormat.TIFF, TiffOptions)** method.

The following code sample shows how to customize pixel format in PPT to TIFF conversion using Python.

{{< gist aspose-com-gists 1fa402fc19dcf41f6a169d63cabee21d "powerpoint-to-tiff-pixel-format.py" >}}

## Get a Free License {#Get-a-Free-API-License}

You can use Aspose.Slides for Python without evaluation limitations by requesting a [temporary license][11].

## Conclusion

In this article, you have learned how to convert PowerPoint PPT to TIFF in Python. Furthermore, you have seen how to customize the image size, include hidden slides, set compression type, and define the pixel format of the resultant TIFF. Besides, you can visit the [documentation][12] to explore other features of Aspose.Slides for Python. Also, you can post your questions or queries to our [forum][13].

## See Also

*   [Create PowerPoint Files in Python][14]
*   [Add Watermark in PowerPoint PPT in Python][15]
*   [Apply 3D Effects in PowerPoint PPT using Python][16]




[1]: https://docs.fileformat.com/image/tiff/
[2]: https://docs.fileformat.com/image/tiff/
[3]: #PowerPoint-to-TIFF-Converter
[4]: #Convert-PowerPoint-to-TIFF
[5]: #Convert-PPT-to-TIFF-with-Hidden-Slides-in-Python
[6]: #Convert-PowerPoint-to-TIFF-with-Custom-Image-Size
[7]: #PPTX-to-TIFF-with-Custom-Pixel-Format
[8]: https://products.aspose.com/slides/python-net
[9]: https://pypi.org/project/aspose.slides/
[10]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides.export/imagepixelformat/
[11]: https://purchase.aspose.com/temporary-license
[12]: https://docs.aspose.com/slides/python-net
[13]: https://forum.aspose.com/
[14]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[15]: https://blog.aspose.com/2022/02/09/add-watermark-to-powerpoint-ppt-in-python/
[16]: https://blog.aspose.com/2022/01/08/create-three-d-effects-in-ppt-python/




