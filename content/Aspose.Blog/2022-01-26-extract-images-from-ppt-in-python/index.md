---
title: 'Extract Images from PowerPoint Presentations in Python'
date: Wed, 26 Jan 2022 15:13:19 +0000
draft: false
url: /2022/01/26/extract-images-from-ppt-in-python/
author: 'Usman Aziz'
summary: 'Images are an effective way of communication that makes the content lively. This is the reason the images are widely adopted in web pages, documents, presentations, etc. MS PowerPoint presentations are usually built up with less text and more graphical objects and images. Therefore, when processing the presentations programmatically, you may need to extract images along with the text. To accomplish that, this article covers **how to extract images from [PPT][1] or [PPTX][2] presentations in Python**.'
tags: ['Python Library to Extract Images from Presentations', 'extract images from ppt in python', 'extract images from presentations in python', 'python image extractor for powerpoint']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Extract-Images-from-Presentations.png" alt="Extract Images from PowerPoint Presentations in Python">}}


Images are an effective way of communication that makes the content lively. This is the reason the images are widely adopted in web pages, documents, presentations, etc. MS PowerPoint presentations are usually built up with less text and more graphical objects and images. Therefore, when processing the presentations programmatically, you may need to extract images along with the text. To accomplish that, this article covers **how to extract images from [PPT][3] or [PPTX][4] presentations in Python**.

*   [Python Library to Extract Images from Presentations][5]
*   [Extract Images from a PPTX Presentation in Python][6]
*   [Extract Images from Shapes][7]
*   [Image Extraction from Slide Background][8]

**Info**: Aspose provides PowerPoint to images converters—[PPT to JPG][9] and [PPT to PNG][10]—that allow you to generate images based on slides in a presentation.

## Python Library to Extract Images from Presentations {#Python-Library-to-Extract-Images-from-Presentations}

To extract images from PowerPoint presentations, we will use [Aspose.Slides for Python via .NET][11]. It is a powerful Python library that is designed to create presentations from scratch. Moreover, it allows you to convert and manipulate the existing presentations seamlessly. You can install it from [PyPI][12] using the following pip command.

```
> pip install aspose.slides
```

## Extract Images from a PowerPoint PPT in Python {#Extract-Images-from-a-PPTX-Presentation-in-Python}

The following are the steps to extract images from a PowerPoint presentation in Python.

*   Load the presentation using **Presentation** class.
*   Loop through the images in presentation using **Presentation.images** collection.
*   Save each image as a file.

The following code sample shows how to extract images from a PPTX file in Python.

{{< gist aspose-com-gists c9c009285fd63669928ec5523dacd3f4 "extract-images.py" >}}

## Extract Images from Shapes in a PPT {#Extract-Images-from-Shapes}

In certain cases, you may need to extract images only from the shapes in a presentation. So let's see how to extract images from shapes in a PPT in Python.

*   First, load the presentation using **Presentation** class.
*   Then, loop through the slides of presentation using **Presentation.slides** collection.
*   For each slide, access its shapes using **ISlide.shapes** collection.
*   For each shape in the collection, perform the following steps:
    *   If the shape is an auto shape and its fill type is picture then extract image using **IShape.fill\_format.picture\_fill\_format.picture.image** property.
    *   If the shape is a picture frame then extract image using **IShape.picture\_format.picture.image** property.
    *   Finally, save the image as a file.

The following code sample shows how to extract images from shapes in a PPT presentation using Python.

{{< gist aspose-com-gists c9c009285fd63669928ec5523dacd3f4 "extract-image-from-shape.py" >}}

## Extract Images from Slide Backgrounds in a PPT {#Image-Extraction-from-Slide-Background}

Another scenario could be extracting the images that are used as slide backgrounds. The following are the steps to extract images only from slide backgrounds in a PPT presentation.

*   First, load the presentation using **Presentation** class.
*   Then, loop through the slides of presentation using **Presentation.slides** collection.
*   For each slide, perform the following steps:
    *   Check if slide has a background image using **ISlide.background.fill\_format.fill\_type** property.
    *   If the background has picture then extract image using **ISlide.background.fill\_format.picture\_fill\_format.picture.image** property.
    *   Check if the layout slide has background image using **ISlide.layout\_slide.background.fill\_format.fill\_type** property.
    *   If background is filled with a picture then extract it using **ISlide.layout\_slide.background.fill\_format.picture\_fill\_format.picture.image** property.
    *   Finally, save the extracted image as a file.

The following code sample shows how to extract images from slide backgrounds in a PPT in Python.

{{< gist aspose-com-gists c9c009285fd63669928ec5523dacd3f4 "extract-image-from-background.py" >}}

Both of the above code samples use a method **get\_image\_format**, which returns the appropriate image format for the provided type. The implementation of that method is provided below.

{{< gist aspose-com-gists c9c009285fd63669928ec5523dacd3f4 "get-image-format.py" >}}

## Get a Free License

You can get a [free temporary license][13] to use Aspose.Slides for Python via .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to extract images from PowerPoint presentations in Python. We have also covered the extraction of images from shapes and slide backgrounds separately. Besides, you can explore more about Aspose.Slides for Python by visiting the [documentation][14]. Also, you can ask your questions via our [forum][15].

## See Also

*   [Create PowerPoint Files in Python][16]
*   [Convert PPTX to PDF in Python][17]
*   [Convert PPT to PNG in Python][18]
*   [PPT/PPTX to HTML in Python][19]




[1]: https://docs.fileformat.com/presentation/ppt/
[2]: https://docs.fileformat.com/presentation/pptx/
[3]: https://docs.fileformat.com/presentation/ppt/
[4]: https://docs.fileformat.com/presentation/pptx/
[5]: #Python-Library-to-Extract-Images-from-Presentations
[6]: #Extract-Images-from-a-PPTX-Presentation-in-Python
[7]: #Extract-Images-from-Shapes
[8]: #Image-Extraction-from-Slide-Background
[9]: https://products.aspose.app/slides/conversion/ppt-to-jpg
[10]: https://products.aspose.app/slides/conversion/ppt-to-png
[11]: https://products.aspose.com/slides/python-net
[12]: https://pypi.org/project/aspose.slides/
[13]: https://purchase.aspose.com/temporary-license
[14]: https://docs.aspose.com/slides/python-net
[15]: https://forum.aspose.com/
[16]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[17]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/
[18]: https://blog.aspose.com/2021/12/29/convert-ppt-to-png-in-python/
[19]: https://blog.aspose.com/2021/12/16/convert-ppt-to-html-in-python/




