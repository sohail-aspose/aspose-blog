---
title: 'Convert PowerPoint PPTX/PPT to TIFF using C#'
seoTitle: "Convert PowerPoint PPTX/PPT to TIFF using C# | Customize Size or Pixel"
description: "Use .NET PowerPoint API to convert PowerPoint PPTX or PPT to TIFF using C#. Customize the image size and pixel format in PPTX/PPT to TIFF conversion."
date: Wed, 11 Aug 2021 18:36:00 +0000
draft: false
url: /2021/08/11/convert-powerpoint-to-tiff-using-csharp/
author: Usman Aziz
summary: 'PowerPoint to TIFF conversion could be useful in various scenarios, such as, for printing, fax, etc. In order to perform this conversion programmatically, this article covers **how to convert PowerPoint PPTX/PPT to TIFF using C#**. Furthermore, you will learn how to customize the size and pixel format of the resultant TIFF images.'
tags: ['powerpoint to tiff csharp', 'ppt to tiff csharp', 'pptx to tiff csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/PowerPoint-to-TIFF.jpg" alt="PowerPoint to TIFF C#">}}


PowerPoint to [TIFF][1] conversion could be useful in various scenarios, such as, for printing, fax, etc. In order to perform this conversion programmatically, this article covers **how to convert PowerPoint PPTX/PPT to TIFF using C#**. Furthermore, you will learn how to customize the size and pixel format of the resultant TIFF images.

*   [C# PowerPoint to TIFF Converter][2]
*   [Convert PowerPoint to TIFF][3]
*   [Convert PowerPoint to TIFF with Custom Image Size][4]
*   [PPTX to TIFF with Custom Pixel Format][5]

TIP: You may want to check out **Aspose FREE online [PowerPoint to Poster Converter][6].**

## C# PowerPoint to TIFF Converter {#PowerPoint-to-TIFF-Converter}

In order to convert the PowerPoint presentations, we will use [Aspose.Slides for .NET][7]. The API is designed to create, manipulate and convert presentation documents from within the .NET applications. You can either [download][8] the API or install it using [NuGet][9].

```
PM> Install-Package Aspose.Slides.NET 
```

## Convert PowerPoint PPTX to TIFF using C# {#Convert-PowerPoint-to-TIFF}

The following are the steps to convert a PowerPoint PPTX/PPT to TIFF using C#.

*   Load the PowerPoint presentation using [Presentation][10] class.
*   Convert PPTX to TIFF using [Presentation.Save(string, SaveFormat.Tiff)][11] method.

The following code sample shows how to convert a PowerPoint PPTX file to TIFF.

{{< gist aspose-com-gists 5c21d384f432926aa70f16160966467b "powerpoint-to-tiff.cs" >}}

## C# Convert PowerPoint to TIFF with Custom Image Size {#Convert-PowerPoint-to-TIFF-with-Custom-Image-Size}

Aspose.Slides for .NET also allows you to customize the size of the resultant image in PowerPoint to TIFF conversion. The following are the steps to achieve this.

*   Load the PowerPoint presentation using [Presentation][12] class.
*   Create an instance of [TiffOptions][13] class.
*   Set image size using [TiffOptions.ImageSize][14] property.
*   Convert PPTX to TIFF using [Presentation.Save(string, SaveFormat.Tiff)][15] method.

The following code sample shows how to convert PPTX to TIFF with custom image size.

{{< gist aspose-com-gists 5c21d384f432926aa70f16160966467b "powerpoint-to-tiff-image-size.cs" >}}

## Convert PowerPoint to TIFF with Custom Pixel Format {#PPTX-to-TIFF-with-Custom-Pixel-Format}

The following are the steps to customize the pixel format in PPTX to TIFF conversion using C#.

*   Load the PowerPoint presentation using [Presentation][16] class.
*   Create an instance of [TiffOptions][17] class.
*   Set pixel format to desired [format][18] using [TiffOptions.PixelFormat][19] property.
*   Convert PPTX to TIFF using [Presentation.Save(string, SaveFormat.Tiff)][20] method.

The following code sample shows how to customize pixel format in PPTX to TIFF conversion.

{{< gist aspose-com-gists 5c21d384f432926aa70f16160966467b "powerpoint-to-tiff-pixel-format.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for .NET without evaluation limitations by requesting a [temporary license][21].

## Conclusion

In this article, you have learned how to convert PowerPoint PPTX/PPT to TIFF using C#. Furthermore, you have seen how to customize the size and pixel format of the resultant TIFF images. You can visit the [documentation][22] to explore other features of Aspose.Slides for .NET. In addition, you can feel free to let us know about your queries via our [forum][23].

## See Also

*   [Create MS PowerPoint Presentations in C#][24]




[1]: https://docs.fileformat.com/image/tiff/
[2]: #PowerPoint-to-TIFF-Converter
[3]: #Convert-PowerPoint-to-TIFF
[4]: #Convert-PowerPoint-to-TIFF-with-Custom-Image-Size
[5]: #PPTX-to-TIFF-with-Custom-Pixel-Format
[6]: https://products.aspose.app/slides/conversion/convert-ppt-to-poster-online
[7]: https://products.aspose.com/slides/net
[8]: https://downloads.aspose.com/slides/net
[9]: https://www.nuget.org/packages/Aspose.Slides.Net
[10]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[11]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[12]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[13]: https://apireference.aspose.com/slides/net/aspose.slides.export/tiffoptions
[14]: https://apireference.aspose.com/slides/net/aspose.slides.export/tiffoptions/properties/imagesize
[15]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[16]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[17]: https://apireference.aspose.com/slides/net/aspose.slides.export/tiffoptions
[18]: https://apireference.aspose.com/slides/net/aspose.slides.export/imagepixelformat
[19]: https://apireference.aspose.com/slides/net/aspose.slides.export/tiffoptions/properties/pixelformat
[20]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[21]: https://purchase.aspose.com/temporary-license
[22]: https://docs.aspose.com/slides/net/developer-guide/
[23]: https://forum.aspose.com/
[24]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/





