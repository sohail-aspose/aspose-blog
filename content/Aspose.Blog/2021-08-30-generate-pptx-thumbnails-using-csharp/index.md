---
title: 'Generate Thumbnails for PowerPoint PPTX or PPT using C#'
seoTitle: "Generate Thumbnails of PPTX PPT in C# .NET | Aspose PowerPoint API"
description: "Use .NET PowerPoint API to generate thumbnails of PPTX or PPT presentations using C# or VB.NET. Generate thumbnails with desired dimensions."
date: Mon, 30 Aug 2021 23:59:00 +0000
draft: false
url: /2021/08/30/generate-pptx-thumbnails-using-csharp/
author: Usman Aziz
summary: "[Thumbnails][1] are commonly used to create small-sized versions of the larger images. They make it easier to look at or scroll through the list of images. MS PowerPoint also provides you the thumbnails of the slides in a presentation. Using slides' thumbnails, you can easily go through the presentation and navigate to a particular slide. In this article, you will learn **how to generate thumbnails of PowerPoint PPTX or PPT using C#**. This could be useful in scenarios such as when you need to create your own web or desktop-based PowerPoint viewer."
tags: ['generate powerpoint thumbnail in csharp', 'generate thumbnails for ppt csharp', 'generate thumbnails for pptx csharp', 'ppt to thumbnail in csharp', 'pptx to thumbnail in csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Generate-PPTX-Thumbnails.jpg" alt="generate PPTX thumbnails in C#">}}


[Thumbnails][2] are commonly used to create small-sized versions of the larger images. They make it easier to look at or scroll through the list of images. MS PowerPoint also provides you the thumbnails of the slides in a presentation. Using slides' thumbnails, you can easily go through the presentation and navigate to a particular slide. In this article, you will learn **how to generate thumbnails of PowerPoint PPTX or PPT using C#**. This could be useful in scenarios such as when you need to create your own web or desktop-based PowerPoint viewer.

*   [.NET API to Generate Thumbnails for PowerPoint PPTX/PPT][3]
*   [Generate Thumbnails for PPTX/PPT using C#][4]
*   [Generate Thumbnails with User-Defined Dimensions][5]

## .NET API to Generate Thumbnails for PowerPoint PPTX/PPT {#API-to-Generate-Thumbnails-for-PowerPoint-PPTX-PPT}

In order to generate thumbnails for PPTX or PPT presentations, we will use [Aspose.Slides for .NET][6]. It is a powerful API that lets you create and manipulate PowerPoint and OpenOffice documents. In addition, it allows you to convert presentations to other file formats. You can either [download][7] the API or install it using [NuGet][8].

```
PM> Install-Package Aspose.Slides.NET
```

## Generate Thumbnails for PPTX or PPT using C# {#Generate-Thumbnails-for-PPTX-PPT}

The following are the steps to generate thumbnails of a PPTX presentation using C#.

1.  First, create an instance of the [Presentation][9] class to load the presentation.
2.  Loop through each [ISlide][10] in [Presentation.Slides][11] collection.
3.  Generate thumbnail of the each slide using [ISlide.GetThumbnail(1f, 1f)][12] method and get the reference of thumbnail into a [Bitmap][13] object.
4.  Finally, save the thumbnail into your desired image format using [Bitmap.Save(String, System.Drawing.Imaging.ImageFormat)][14] method.

The following code sample shows how to generate thumbnails of a PPTX presentation using C#.

{{< gist aspose-com-gists 303d1ecc4588599fd3bb67700f7e3b7e "generate-pptx-thumbnail.cs" >}}

## Generate Thumbnails with User-Defined Dimensions {#Generate-Thumbnails-with-User-Defined-Dimensions}

You can also customize the dimensions of the thumbnails according to your requirement. This can be achieved using [Presentation.SlideSize.Size.Width][15] and [Presentation.SlideSize.Size.Height][16] properties. The following are the steps to perform this operation.

1.  First, create an instance of the [Presentation][17] class to load the presentation.
2.  Then, set the desired dimensions of the thumbnails and scale the values using [Width][18] and [Height][19] properties.
3.  Loop through each [ISlide][20] in [Presentation.Slides][21] collection.
4.  Generate thumbnail of the each slide using [ISlide.GetThumbnail(Single, Single)][22] method and get the reference of thumbnail into a [Bitmap][23] object.
5.  Finally, save the thumbnail into your desired image format using [Bitmap.Save(String, System.Drawing.Imaging.ImageFormat)][24] method.

The following code sample shows how to generate thumbnails of a PPTX with customized dimensions.

{{< gist aspose-com-gists 303d1ecc4588599fd3bb67700f7e3b7e "generate-pptx-thumbnail-custom-dimension.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for .NET without evaluation limitations by requesting a [temporary license][25].

## Conclusion

In this article, you have learned how to generate thumbnails of PowerPoint PPTX or PPT using C#. Furthermore, you have seen how to generate thumbnails with desired dimensions. In addition, you can visit the [documentation][26] to explore other features of API. Also, you can feel free to let us know about your queries via our [forum][27].

## See Also

*   [Create MS PowerPoint Presentations in C#][28]




[1]: https://en.wikipedia.org/wiki/Thumbnail
[2]: https://en.wikipedia.org/wiki/Thumbnail
[3]: #API-to-Generate-Thumbnails-for-PowerPoint-PPTX-PPT
[4]: #Generate-Thumbnails-for-PPTX-PPT
[5]: #Generate-Thumbnails-with-User-Defined-Dimensions
[6]: https://products.aspose.com/slides/net/
[7]: https://downloads.aspose.com/slides/net/
[8]: https://www.nuget.org/packages/Aspose.Slides.NET
[9]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[10]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[11]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/slides
[12]: https://apireference.aspose.com/slides/net/aspose.slides.islide/getthumbnail/methods/9
[13]: https://docs.microsoft.com/en-us/dotnet/api/system.drawing.bitmap
[14]: https://docs.microsoft.com/en-us/dotnet/api/system.drawing.image.save?view=net-5.0#System_Drawing_Image_Save_System_String_System_Drawing_Imaging_ImageFormat_
[15]: https://docs.microsoft.com/en-gb/dotnet/api/system.drawing.sizef.width?view=net-5.0#System_Drawing_SizeF_Width
[16]: https://docs.microsoft.com/en-gb/dotnet/api/system.drawing.sizef.height?view=net-5.0#System_Drawing_SizeF_Height
[17]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[18]: https://docs.microsoft.com/en-gb/dotnet/api/system.drawing.sizef.width?view=net-5.0#System_Drawing_SizeF_Width
[19]: https://docs.microsoft.com/en-gb/dotnet/api/system.drawing.sizef.height?view=net-5.0#System_Drawing_SizeF_Height
[20]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[21]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/slides
[22]: https://apireference.aspose.com/slides/net/aspose.slides.islide/getthumbnail/methods/9
[23]: https://docs.microsoft.com/en-us/dotnet/api/system.drawing.bitmap
[24]: https://docs.microsoft.com/en-us/dotnet/api/system.drawing.image.save?view=net-5.0#System_Drawing_Image_Save_System_String_System_Drawing_Imaging_ImageFormat_
[25]: https://purchase.aspose.com/temporary-license
[26]: https://docs.aspose.com/slides/net/developer-guide/
[27]: https://forum.aspose.com/
[28]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/





