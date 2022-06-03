---
title: 'Convert PowerPoint PPT to Animated GIF in Python'
date: Thu, 24 Feb 2022 14:28:09 +0000
draft: false
url: /2022/02/24/convert-ppt-to-gif-in-python/
author: 'Usman Aziz'
summary: 'In various cases, PowerPoint presentations are converted to other formats such as HTML, images, etc. It is usually done to avoid dependency on MS PowerPoint to view the presentations. In accordance with that, this article shows **how to convert a PowerPoint [PPT][1] or [PPTX][2] presentation to an animated [GIF][3] in Python**. Moreover, we will cover how to set frame size, the delay between slides, and frames per second programmatically.'
tags: ['Python PowerPoint to GIF Converter', 'convert powerpoint to gif in python', 'convert ppt to gif in python', 'convert pptx to gif in python']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Convert-PowerPoint-PPT-to-GIF.png" alt="Convert PowerPoint PPT to Animated GIF in Python">}}


In various cases, PowerPoint presentations are converted to other formats such as HTML, images, etc. It is usually done to avoid dependency on MS PowerPoint to view the presentations. In accordance with that, this article shows **how to convert a PowerPoint [PPT][4] or [PPTX][5] presentation to an animated [GIF][6] in Python**. Moreover, we will cover how to set frame size, the delay between slides, and frames per second programmatically.

*   [Python Library for PowerPoint to GIF Conversion][7]
*   [Convert a PowerPoint PPT to GIF in Python][8]
*   [Set Additional Options for PPT/PPTX to GIF Conversion][9]

**Info**: Aspose recently developed an online [Text to GIF][10] service that allows you to transform texts or messages into interesting animations.

## Python Library for PowerPoint PPT to GIF Conversion {#Library-for-PowerPoint-to-GIF-Conversion}

To convert PowerPoint presentations to animated GIF, we will use [Aspose.Slides for Python][11]. It is a powerful Python library that lets you create and manipulate presentations seamlessly. Furthermore, it provides high-quality conversion of PPT/PPTX to other popular formats. To use this library, you can install it from [PyPI][12] using the following command.

```
> pip install aspose.slides
```

## Convert a PowerPoint PPT to GIF in Python {#Convert-a-PowerPoint-PPT-to-GIF}

Aspose.Slides for Python converts the complete presentation to an animated GIF, which contains all the slides. The following are the simple steps to convert a PPT to GIF in Python.

*   Load the PPT/PPTX presentation using **Presentation** class.
*   Save the presentation as GIF using **Presentation.save(string, SaveFormat.GIF)** method.

The following code sample shows how to convert a PowerPoint PPTX file to an animated GIF in Python.

{{< gist aspose-com-gists f5069f87659431e7bf30e4679558880c "ppt-to-gif.py" >}}

## Set Additional Options - Python PPT to GIF {#Set-Additional-Options-for-PPT-PPTX-to-GIF-Conversion}

Aspose.Slides for Python also allows you to customize PPT to GIF conversion using different options. You can set the delay between slides, frame size of GIF, and the transition in frames per second. The following are the steps to achieve this.

*   Load the PPT/PPTX presentation using **Presentation** class.
*   Create an instance of **GifOptions** class.
*   Set desired options such as frame size.
*   Save the presentation as GIF using **Presentation.save(string, SaveFormat.GIF, GifOptions)** method.

The following code sample shows how to convert a PPT to an animated GIF with customized settings in Python.

{{< gist aspose-com-gists f5069f87659431e7bf30e4679558880c "ppt-to-gif-custom.py" >}}

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][13] to use Aspose.Slides for Python without evaluation limitations.

## Conclusion

In this article, you have learned how to convert PowerPoint PPT/PPTX presentations to animated GIF in Python. Furthermore, you have seen how to customize PowerPoint to GIF conversion using different options. Besides, you can explore more about Aspose.Slides for Python using the [documentation][14]. Also, you can feel free to let us know about your queries via our [forum][15].

## See Also

*   [Create PowerPoint Files in Python][16]
*   [Convert PPTX to PDF in Python][17]
*   [Convert PPT to PNG in Python][18]
*   [PPT/PPTX to HTML in Python][19]
*   [Add Watermark in PowerPoint PPT in Python][20]
*   [Apply 3D Effects in PowerPoint PPT using Python][21]




[1]: https://docs.fileformat.com/presentation/ppt/
[2]: https://docs.fileformat.com/presentation/pptx/
[3]: https://docs.fileformat.com/image/gif/
[4]: https://docs.fileformat.com/presentation/ppt/
[5]: https://docs.fileformat.com/presentation/pptx/
[6]: https://docs.fileformat.com/image/gif/
[7]: #Library-for-PowerPoint-to-GIF-Conversion
[8]: #Convert-a-PowerPoint-PPT-to-GIF
[9]: #Set-Additional-Options-for-PPT-PPTX-to-GIF-Conversion
[10]: https://products.aspose.app/slides/text-to-gif
[11]: https://products.aspose.com/slides/python-net
[12]: https://pypi.org/project/aspose.slides/
[13]: https://purchase.aspose.com/temporary-license
[14]: https://docs.aspose.com/slides/python-net/
[15]: https://forum.aspose.com/
[16]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[17]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/
[18]: https://blog.aspose.com/2021/12/29/convert-ppt-to-png-in-python/
[19]: https://blog.aspose.com/2021/12/16/convert-ppt-to-html-in-python/
[20]: https://blog.aspose.com/2022/02/09/add-watermark-to-powerpoint-ppt-in-python/
[21]: https://blog.aspose.com/2022/01/08/create-three-d-effects-in-ppt-python/




