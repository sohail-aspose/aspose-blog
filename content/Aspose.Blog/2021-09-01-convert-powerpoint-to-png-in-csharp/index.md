---
title: 'Convert PowerPoint PPTX/PPT to PNG Images in C#'
seoTitle: "Convert PowerPoint to PNG in C# | PPTX to PNG, PPT to PNG | .NET API"
description: "Convert PowerPoint to PNG images in C#. Convert PPT to PNG or PPTX to PNG. Create your online PPT(X) to PNG converter in ASP.NET or any .NET application."
date: Wed, 01 Sep 2021 15:18:30 +0000
draft: false
url: /2021/09/01/convert-powerpoint-to-png-in-csharp/
author: Usman Aziz
summary: 'In certain cases, you may need to convert the slides in PowerPoint presentations to images. For example, to embed presentations in your web or desktop applications, to generate thumbnails, etc. [PNG][1] is one of the most popular image formats which uses lossless compression. Therefore, in this article, you will learn **how to convert slides in PowerPoint PPTX or PPT to PNG images using C#**.'
tags: ['powerpoint to png csharp', 'ppt to png csharp', 'pptx to png csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/PowerPoint-to-PNG-Image.jpg" alt="">}}


In certain cases, you may need to convert the slides in PowerPoint presentations to images. For example, to embed presentations in your web or desktop applications, to generate thumbnails, etc. [PNG][2] is one of the most popular image formats which uses lossless compression. Therefore, in this article, you will learn **how to convert slides in PowerPoint PPTX or PPT to PNG images using C#**.

*   [.NET API for PowerPoint to PNG Conversion][3]
*   [Convert PowerPoint PPTX or PPT to PNG][4]

## C# API for PowerPoint to PNG Conversion {#API-for-PowerPoint-to-PNG-Conversion}

In order to convert the PPTX or PPT presentations to PNG, we will use [Aspose.Slides for .NET][5]. It is a feature-rich API that lets you create, modify and convert PowerPoint and OpenOffice presentations using C#. You can either [download][6] the API or install it using [NuGet][7].

```
PM> Install-Package Aspose.Slides.NET 
```

## Convert PowerPoint PPTX or PPT to PNG in C# {#Convert-PowerPoint-PPTX-or-PPT-to-PNG}

The following are the steps to convert slides in a PowerPoint PPTX to PNG images using C#.

1.  First, create an instance of the [Presentation][8] class to load the presentation.
2.  Loop through each [ISlide][9] in [Presentation.Slides][10] collection.
3.  Define the dimensions of the resultant PNG image.
4.  Generate image of the each slide using [ISlide.GetThumbnail(float ScaleX, float ScaleY)][11] method and get the reference of image into a [Bitmap][12] object.
5.  Finally, save image as PNG using [Bitmap.Save(String, System.Drawing.Imaging.ImageFormat.Png)][13] method.

The following code sample shows how to convert a PowerPoint PPTX to PNG.

{{< gist aspose-com-gists adf0d42992442cb65f4882048b80d343 "powerpoint-to-png.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for .NET without evaluation limitations by requesting a [temporary license][14].

## Online Demo

Try the [online PowerPoint to PNG converter][15], which is based on Aspose.Slides.

## Conclusion

In this article, you have learned how to convert slides in PowerPoint PPTX or PPT to PNG using C#. You can simply install the API and use the provided code in your .NET applications. In addition, you can visit the [documentation][16] to explore other features of API. Also, you can feel free to let us know about your queries via our [forum][17].

## See Also

*   [Create MS PowerPoint Presentations in C#][18]




[1]: https://docs.fileformat.com/image/png/
[2]: https://docs.fileformat.com/image/png/
[3]: #API-for-PowerPoint-to-PNG-Conversion
[4]: #Convert-PowerPoint-PPTX-or-PPT-to-PNG
[5]: https://products.aspose.com/slides/net
[6]: https://downloads.aspose.com/slides/net
[7]: https://www.nuget.org/packages/Aspose.Slides.NET
[8]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[9]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[10]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/slides
[11]: https://apireference.aspose.com/slides/net/aspose.slides.islide/getthumbnail/methods/9
[12]: https://docs.microsoft.com/en-us/dotnet/api/system.drawing.bitmap
[13]: https://docs.microsoft.com/en-us/dotnet/api/system.drawing.image.save?view=net-5.0#System_Drawing_Image_Save_System_String_System_Drawing_Imaging_ImageFormat_
[14]: https://purchase.aspose.com/temporary-license
[15]: https://products.aspose.app/slides/conversion/pptx-to-png
[16]: https://docs.aspose.com/slides/net/developer-guide/
[17]: https://forum.aspose.com/
[18]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/




