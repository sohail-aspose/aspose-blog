---
title: 'Create Thumbnails for PPT Slides in Python'
date: Fri, 28 Jan 2022 07:21:47 +0000
draft: false
url: /2022/01/28/create-thumbnails-for-ppt-in-python/
author: ''Usman Aziz''
summary: '[Thumbnails][1] are small-sized images that make it easier to look at or scroll through the list of images. They are also used in MS PowerPoint to list the slides and navigate in a PPT. While creating a PPT viewer application, you may need to generate thumbnail images for the slides. To accomplish that, this article covers **how to create thumbnails for [PPTX][2] or [PPT][3] slides programmatically in Python**.'
tags: ['Create PPT Viewer in Python', 'Create Thumbnails for PPT Slides in Python', 'Generate Thumbnails for PPT Slides Show in Python', 'Python Library to Create Thumbnails for PPT Slides']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Create-PPT-Thumbnails.png" alt="Create Thumbnails for PPT Slides in Python">}}


[Thumbnails][4] are small-sized images that make it easier to look at or scroll through the list of images. They are also used in MS PowerPoint to list the slides and navigate in a PPT. While creating a PPT viewer application, you may need to generate thumbnail images for the slides. To accomplish that, this article covers **how to create thumbnails for [PPTX][5] or [PPT][6] slides programmatically in Python**.

*   [Python Library to Create Thumbnails for PPT Slides][7]
*   [Create Thumbnails for PPTX/PPT Slides][8]
*   [Create Thumbnails with User-Defined Dimensions][9]

## Python Library to Create Thumbnails for PPT Slides {#API-to-Generate-Thumbnails-for-PowerPoint-PPTX-PPT}

To create thumbnails for slides in PPTX or PPT presentations, we will use [Aspose.Slides for Python via .NET][10]. The library provides a bunch of features to create and manipulate PowerPoint presentations. Moreover, it lets you convert the presentations to other formats. You can install the library in your applications from [PyPI][11] using the following command.

```
> pip install aspose.slides
```

## Create Thumbnails for PPT Slides in Python {#Generate-Thumbnails-for-PPTX-PPT}

The following are the steps to create thumbnails for a presentation in Python.

1.  First, load the presentation file using **Presentation** class.
2.  Loop through each **ISlide** in **Presentation.slides** collection.
3.  Create thumbnail of the each slide using **ISlide.get\_thumbnail(scale\_x, scale\_y)** method and get the reference of thumbnail into a **Bitmap** object.
4.  Finally, save the thumbnail into your desired image format using **Bitmap.save(String, ImageFormat)** method.

The following code sample shows how to create thumbnails for slides in a PPTX presentation in Python.

{{< gist aspose-com-gists ca731f8fd76b67fc56580bd84d112665 "create-ppt-thumbnail.py" >}}

## Create PPT Thumbnails with Custom Dimensions {#Generate-Thumbnails-with-User-Defined-Dimensions}

Often, you may need to create thumbnails of customized dimensions. This can be achieved using **Presentation.slide\_size.size.width** and **Presentation.slide\_size.size.height** properties. The following are the steps to create thumbnails of custom dimensions.

1.  First, create an instance of the **Presentation **class to load the presentation.
2.  Then, specify desired values of width and height.
3.  Get scaled values of the X and Y.
4.  Loop through each **ISlide** in **Presentation.slides** collection.
5.  Generate thumbnail of the each slide using **ISlide.get\_thumbnail(X, Y)** method and get the reference of thumbnail into a **Bitmap** object.
6.  Finally, save the thumbnail into your desired image format using **Bitmap.save(string, ImageFormat)** method.

The following code sample shows how to create thumbnails of a PPTX with customized dimensions.

{{< gist aspose-com-gists ca731f8fd76b67fc56580bd84d112665 "create-ppt-thumbnail-custom-dimension.py" >}}

## Get a Free License {#Get-a-Free-API-License}

You can use Aspose.Slides for Python via .NET without evaluation limitations by requesting a [temporary license][12].

## Conclusion

In this article, you have learned how to create thumbnails of PPT slides in Python. Moreover, you have seen how to use custom dimensions to scale the PPT thumbnail images. In addition, you can visit the [documentation][13] to explore other features of Aspose.Slides for Python. Also, you can let us know about your queries via our [forum][14].

## See Also

*   [Create PowerPoint Files in Python][15]
*   [Convert PPTX to PDF in Python][16]
*   [Convert PPT to PNG in Python][17]
*   [PPT/PPTX to HTML in Python][18]




[1]: https://en.wikipedia.org/wiki/Thumbnail
[2]: https://docs.fileformat.com/presentation/pptx/
[3]: https://docs.fileformat.com/presentation/ppt/
[4]: https://en.wikipedia.org/wiki/Thumbnail
[5]: https://docs.fileformat.com/presentation/pptx/
[6]: https://docs.fileformat.com/presentation/ppt/
[7]: #API-to-Generate-Thumbnails-for-PowerPoint-PPTX-PPT
[8]: #Generate-Thumbnails-for-PPTX-PPT
[9]: #Generate-Thumbnails-with-User-Defined-Dimensions
[10]: https://products.aspose.com/slides/python-net
[11]: https://pypi.org/project/aspose.slides/
[12]: https://purchase.aspose.com/temporary-license
[13]: https://docs.aspose.com/slides/python-net
[14]: https://forum.aspose.com/
[15]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[16]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/
[17]: https://blog.aspose.com/2021/12/29/convert-ppt-to-png-in-python/
[18]: https://blog.aspose.com/2021/12/16/convert-ppt-to-html-in-python/




