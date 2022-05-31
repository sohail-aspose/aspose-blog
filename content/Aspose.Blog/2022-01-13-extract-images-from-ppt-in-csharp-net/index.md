---
title: 'Extract Images from PowerPoint PPT in C#'
date: Thu, 13 Jan 2022 12:01:00 +0000
draft: false
url: /2022/01/13/extract-images-from-ppt-in-csharp-net/
author: 'Usman Aziz'
summary: 'While processing the PowerPoint presentations in a .NET application, you may need to extract content from the PPT slides. The content could be in the form of text and images. In the [previous post][1], we have covered text extraction from PowerPoint slides. In this article, we will show you **how to extract images from PowerPoint [PPT][2] or [PPTX][3] in C#**.'
tags: ['extract images from powerpoint in csharp', 'extract images from ppt backgrounds in csharp', 'extract images from ppt in csharp', 'extract images from pptx in csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Extract-Images-from-Presentations.png" alt="Extract Images from PowerPoint PPT in C#">}}


While processing the PowerPoint presentations in a .NET application, you may need to extract content from the PPT slides. The content could be in the form of text and images. In the [previous post][4], we have covered text extraction from PowerPoint slides. In this article, we will show you **how to extract images from PowerPoint [PPT][5] or [PPTX][6] in C#**.

*   [.NET API to Extract Images from Presentations][7]
*   [Extract Images from a PPTX Presentation in C#][8]
*   [Extract Images from Shapes][9]
*   [Image Extraction from Slide Background][10]

## C# .NET API to Extract Images from PowerPoint PPT {#Library-to-Extract-Images-from-Presentations}

For extracting images from PowerPoint PPT/PPTX, we will use [Aspose.Slides for .NET][11]. It is a feature-rich .NET API that allows you to create new presentations and manipulate the existing ones seamlessly. You can either [download][12] API’s DLL or install it using [NuGet][13].

```
PM> Install-Package Aspose.Slides.NET
```

## Extract Images from a PowerPoint PPT in C# {#Extract-Images-from-a-PPTX-Presentation-in-Python}

The following are the steps to extract all the images in a PPT presentation in C#.

*   First, use [Presentation][14] class to load the PPT/PPTX file.
*   Then, loop through all the images in the presentation using [Presentation.Images][15] collection.
*   Finally, get type and format of each image and save it.

The following code sample shows how to extract images from a PowerPoint PPT in C#.

{{< gist aspose-com-gists e38c11d0c0dc6fec2334dc1faf13babc "extract-ppt-images.cs" >}}

## Extract Images from Shapes in a PPT {#Extract-Images-from-Shapes}

In various cases, you may need to extract images from the shape objects only. This can be achieved by following the steps below.

*   First, use [Presentation][16] class to load the presentation file.
*   Then, use [Presentation.Slides][17] collection to loop through slides.
*   For each slide, access its shapes using [ISlide.Shapes][18] collection.
*   Perform the following steps for each shape in the collection:
    *   If the shape is an auto shape and it is filled with a picture then extract image using [IShape.FillFormat.PictureFillFormat.Picture.Image][19] property.
    *   If the shape is a picture frame then extract image using [IPictureFrame.PictureFormat.Picture.Image][20] property.
    *   Finally, save the image as a file.

The following code sample shows how to extract images from shapes in a PPT using C#.

{{< gist aspose-com-gists e38c11d0c0dc6fec2334dc1faf13babc "extract-ppt-shape-images.cs" >}}

## Extract Images from Slide Backgrounds in C# {#Image-Extraction-from-Slide-Background}

Another possible scenario could be extracting images that are used only as slide backgrounds. The following steps show how to extract slide background images in C#.

*   First, load the PPT/PPTX file using [Presentation][21] class.
*   Then, loop through the slides in the presentation using [Presentation.Slides][22] collection.
*   For each slide, perform the following steps:
    *   Check if slide has a background image using [ISlide.Background.FillFormat.FillType][23] property.
    *   If the background has picture then extract image using [Background.FillFormat.PictureFillFormat.Picture.Image][24] property.
    *   Check if the layout slide has background image using [LayoutSlide.Background.FillFormat.FillType][25] property.
    *   If layout slide's background is filled with a picture then extract it using [ISlide.LayoutSlide.Background.FillFormat.PictureFillFormat.Picture.Image][26] property.
    *   Finally, save the extracted image as a file.

The following code sample shows how to extract images from slide backgrounds in a PPT in C#.

{{< gist aspose-com-gists e38c11d0c0dc6fec2334dc1faf13babc "extract-ppt-background-images.cs" >}}

We have used the method **GetImageFormat** in all of the above code snippets. This method returns the appropriate image format for the provided type. The implementation of this method is given below.

{{< gist aspose-com-gists e38c11d0c0dc6fec2334dc1faf13babc "get-image-format.cs" >}}

## Get a Free License

You can get a [free temporary license][27] to use Aspose.Slides for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to extract images from PowerPoint PPT/PPTX in C#. With the help of code samples, we have demonstrated how to extract images from shapes and slide backgrounds. You can explore more about Aspose.Slides for .NET by visiting the [documentation][28]. Also, you can ask your questions via our [forum][29].

## See Also

*   [Create MS PowerPoint Presentations in C#][30]
*   [Add or Remove Shapes in PowerPoint Slides using C#][31]




[1]: https://blog.aspose.com/2021/03/06/extract-text-from-powerpoint-pptx-using-csharp/
[2]: https://docs.fileformat.com/presentation/ppt
[3]: https://docs.fileformat.com/presentation/pptx
[4]: https://blog.aspose.com/2021/03/06/extract-text-from-powerpoint-pptx-using-csharp/
[5]: https://docs.fileformat.com/presentation/ppt
[6]: https://docs.fileformat.com/presentation/pptx
[7]: #Library-to-Extract-Images-from-Presentations
[8]: #Extract-Images-from-a-PPTX-Presentation-in-Python
[9]: #Extract-Images-from-Shapes
[10]: #Image-Extraction-from-Slide-Background
[11]: https://products.aspose.com/slides/net
[12]: https://downloads.aspose.com/slides/net
[13]: https://www.nuget.org/packages/Aspose.Slides.Net
[14]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[15]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/images
[16]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[17]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/slides
[18]: https://apireference.aspose.com/slides/net/aspose.slides/ibaseslide/properties/shapes
[19]: https://apireference.aspose.com/slides/net/aspose.slides/islidespicture/properties/image
[20]: https://apireference.aspose.com/slides/net/aspose.slides/islidespicture/properties/image
[21]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[22]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/slides
[23]: https://apireference.aspose.com/slides/net/aspose.slides/ifillformat/properties/filltype
[24]: https://apireference.aspose.com/slides/net/aspose.slides/islidespicture/properties/image
[25]: https://apireference.aspose.com/slides/net/aspose.slides/ifillformat/properties/filltype
[26]: https://apireference.aspose.com/slides/net/aspose.slides/islidespicture/properties/image
[27]: https://purchase.aspose.com/temporary-license
[28]: https://docs.aspose.com/slides/net
[29]: https://forum.aspose.com/
[30]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/
[31]: https://blog.aspose.com/2020/12/24/add-shapes-to-powerpoint-slides-in-csharp/




