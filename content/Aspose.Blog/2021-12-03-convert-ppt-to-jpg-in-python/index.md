---
title: 'Convert PPT to JPG in Python'
seoTitle: "Convert PPT to JPG in Python | Generate PPT Thumbnails in Python"
description: "Use Python PowerPoint library to convert PPT slides to JPG images in Python. Generate thumbnails of PPT having custom dimensions, notes, and comments."
date: Fri, 03 Dec 2021 13:18:00 +0000
draft: false
url: /2021/12/03/convert-ppt-to-jpg-in-python/
author: Usman Aziz
summary: 'While working with PowerPoint presentations in your Python applications, you may need to generate thumbnails for a [PPT][1]. For example, while creating a slideshow or a presentation manipulation tool. In this article, you will learn **how to generate thumbnails by converting a PPT to [JPG][2] images in Python**. We will also cover how to generate JPG images having custom dimensions and render slide notes and comments.'
tags: ['Convert PPT to JPG', 'Convert a PPT to JPG in Python', 'Export PPT to JPG Images in Python', 'Generate PPT Thumbnails in Python', 'Python PPT to JPG Converter']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Convert-PPT-to-JPG.png" alt="Convert PPT to JPG in Python">}}


While working with PowerPoint presentations in your Python applications, you may need to generate thumbnails for a [PPT][3]. For example, while creating a slideshow or a presentation manipulation tool. In this article, you will learn **how to generate thumbnails by converting a PPT to [JPG][4] images in Python**. We will also cover how to generate JPG images having custom dimensions and render slide notes and comments.

*   [Python PPT to JPG Converter][5]
*   [Convert a PPT to JPG][6]
*   [Customize Dimensions of Resultant JPG][7]
*   [Include Notes and Comments in JPG Images][8]

**TIP**: You may want to check out Aspose FREE [PowerPoint to JPG][9] converter.

## Python PPT to JPG Converter {#Python-PPT-to-JPG-Converter}

To convert PowerPoint presentations to JPG images, we will utilize [Aspose.Slides for Python via .NET][10]. It is a powerful library to implement presentation manipulation features in Python. Using the library, you can create, modify and convert the presentations seamlessly. Use the following pip command to install the library from [PyPI][11].

```
> pip install aspose.slides
```

## Convert a PPT to JPG in Python {#Convert-a-PPT-to-JPG}

The following are the steps to convert a PPT presentation to JPG images in Python.

*   First, load the presentation file using [Presentation][12] class.
*   Then, iterate through the slides using **Pesentation.slides** collection.
    *   Get reference of each [ISlide][13] in the collection using slide's index.
    *   Finally, use **ISlide.get\_thumbnail().save(string, ImageFormat.jpeg)** method to convert a slide to JPG image.

The following code sample shows how to convert a PowerPoint PPTX to JPG in Python.

{{< gist aspose-com-gists 27740be4bf35d27c47921c5c425fa725 "ppt-to-jpg.py" >}}

The following screenshot shows the resultant JPG image of first slide in the presentation.



{{< figure align=center src="images/PPT-to-JPG.png" alt="Convert PowerPoint PPT to JPG in Python" caption="Resultant JPG Image">}}


## PPT to JPG - Customize Image Dimensions {#Cutomize-Dimensions-of-Resultant-JPG}

You can also customize the dimensions of the resultant JPG images by providing width and height. Also, you can scale the images as per your requirements. The following steps demonstrate how to convert PPT to JPG with customized dimensions and scaling.

*   First, load the presentation file using [Presentation][14] class.
*   Create two variables to set width and height of JPG images.
*   Set X and Y scaling of the images using the specified width and height.
*   Iterate through the slides using **Pesentation.slides** collection.
    *   Get reference of each [ISlide][15] from the collection using slide's index.
    *   Convert slide to JPG using **ISlide.get\_thumbnail(scaleX, scaleY).save(string, ImageFormat.jpeg)** method.

The following code sample shows how to generate PPT thumbnails with customized scaling and dimensions in Python.

{{< gist aspose-com-gists 27740be4bf35d27c47921c5c425fa725 "ppt-to-jpg-custom-dimensions.py" >}}

## Include Notes and Comments - Python PPT to JPG {#Include-Notes-and-Comments-in-JPG-Images}

MS PowerPoint also allows you to write comments and notes for each slide in the presentation. By default, the comments and notes are not rendered in PPT to JPG conversion. However, you can include them in the resultant JPG images following the below steps.

*   First, load the presentation file using [Presentation][16] class.
*   Create a **Bitmap** object by specifying width and height of resultant images.
*   Create an object of [RenderingOptions][17] class.
*   Specify position for notes using **RenderingOptions.notes\_comments\_layouting.notes\_position** property.
*   To include comments, use **RenderingOptions.notes\_comments\_layouting.comments\_position** property.
*   Iterate through the slides in **Pesentation.slides** collection.
    
    *   Generate graphics object from Bitmap using **Graphics.from\_image(Bitmap)** method.
    *   Render the slide to graphics using **Presentation.slides\[index\].render\_to\_graphics(RenderingOptions, graphics**) method.
    
    *   Save slide as JPG using **Bitmap.save(string, ImageFormat.jpeg)** method.

The following code sample shows how to render notes and comments in PPT to JPG conversion.

{{< gist aspose-com-gists 27740be4bf35d27c47921c5c425fa725 "ppt-to-jpg-notes-comments.py" >}}

The following screenshot shows the resultant JPG image that contains slide notes and comments.



{{< figure align=center src="images/PPT-to-JPG-with-Comments-and-Notes.jpg" alt="Convert a PPT to JPG with Comments and Notes in Python" caption="PPT to JPG with Slide Notes and Comments">}}


## Get a Free License

You can use Aspose.Slides for Python via .NET without evaluation limitations by getting a [temporary license][18].

## Conclusion

In this article, you have learned how to convert PowerPoint PPT or PPTX to JPG images in Python. In addition, you have seen how to generate JPG images with custom dimensions and scaling. We have also covered how to include slide notes and comments in PPT to JPG conversion. Aspose.Slides for Python via .NET also provides a wide range of features that you can explore using the [documentation][19]. In case you would have any questions, contact us on our [forum][20].

## See Also

*   [Convert PPTX to PDF in Python][21]
*   [Create PowerPoint Presentations in Python][22]
*   [Convert PPT to PNG in Python][23]




[1]: https://docs.fileformat.com/presentation/ppt/
[2]: https://docs.fileformat.com/image/jpeg/
[3]: https://docs.fileformat.com/presentation/ppt/
[4]: https://docs.fileformat.com/image/jpeg/
[5]: #Python-PPT-to-JPG-Converter
[6]: #Convert-a-PPT-to-JPG
[7]: #Cutomize-Dimensions-of-Resultant-JPG
[8]: #Include-Notes-and-Comments-in-JPG-Images
[9]: https://products.aspose.app/slides/conversion/ppt-to-jpg
[10]: https://products.aspose.com/slides/python-net/
[11]: https://pypi.org/project/aspose.slides/
[12]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/presentation/
[13]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/islide/
[14]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/presentation/
[15]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/islide/
[16]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/presentation/
[17]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides.export/renderingoptions/
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/slides/python-net
[20]: https://forum.aspose.com/
[21]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/
[22]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[23]: https://blog.aspose.com/2021/12/29/convert-ppt-to-png-in-python/




