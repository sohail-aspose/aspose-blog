---
title: 'Convert PowerPoint PPT/PPTX to JPG Images in C#'
seoTitle: ""
description: ""
date: Fri, 07 Feb 2020 13:38:22 +0000
draft: false
url: /2020/02/07/convert-powerpoint-ppt-pptx-to-jpg-images-in-csharp-net/
author: Usman Aziz
summary: ''
tags: ['Convert PPT to JPG', 'Convert PPTX to JPG', 'Convert PowerPoint Slides to Images', 'Convert PowerPoint to Image in Csharp', 'PowerPoint to JPG']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/PowerPoint-to-Image-in-C.png" alt="Convert PowerPoint to Image">}}


There could be various scenarios when you need to **convert PowerPoint PPT or PPTX to JPG** images. For example, you may need to slide show the PPT/PPTX presentation in read-only mode within your application or you may want to generate the thumbnail for every slide of the PowerPoint presentation and etc. In order to automate **PowerPoint to JPG** conversion, I'll show you how to **convert PPT or PPTX slides to JPG images** programmatically in C# .NET.

**TIP:**

You may want to check out Aspose free [PowerPoint to JPG][1] or [PPTX to JPG][2] converter.

## Converting PPT or PPTX to JPG Images in C#

In order to convert PPT(X) to JPG images, we'll use [Aspose.Slides for .NET][3] which is a complete .NET package for PowerPoint automation. The API provides high-quality conversion of PowerPoint presentations to various file formats including JPG.

You can either download and reference the API's [DLL][4] or install the package using NuGet Package Manager or Package Manager Console.

### Using NuGet Package Manager



{{< figure align=center src="images/Aspose.Slides-NPM.png" alt="PPT to JPG in C#">}}


### Using the Package Manager Console```
PM> Install-Package Aspose.Slides
```

## Convert PowerPoint PPT to JPG in C#

The following are the steps to convert PPT to JPG using _Aspose.Slides for .NET_.

*   Create an instance of [Presentation][5] class and initialize it with a PowerPoint presentation's path.
*   Use [ISlide][6] interface to access the PPT slides from [Presentation.Slides][7] collection.
*   Get slide's thumbnail into [Bitmap][8] object using [ISlide.GetThumbnail(float scaleX, float scaleY)][9] method.
*   Save PPT slide as JPG image using [Image.Save(string filename, ImageFormat format)][10] method.

The following code sample shows how to convert PPT to JPG images in C#.

{{< gist aspose-com-gists ea7de1097bd23deee0a6d59674d5f465 "Convert-PPT-to-JPG.cs" >}}

### PowerPoint Presentation



{{< figure align=center src="images/Presentation.png" alt="PowerPoint PPTX to JPG in C#">}}


### Converted JPG Images



{{< figure align=center src="images/PPT-to-JPG-in-C.png" alt="PPT PPTX to JPG in C#">}}


## Convert PowerPoint PPTX to JPG with Customized Dimensions in C#

You may also customize the dimensions of the JPG images as per your requirements. The following code sample shows how to define _ScaleX_ and _ScaleY_ values while converting PPTX to JPG in C#.

{{< gist aspose-com-gists ea7de1097bd23deee0a6d59674d5f465 "Convert-PPT-to-JPG-Customized-Scaling.cs" >}}

## Get a Free Temporary License for Aspose.Slides for .NET

You can get a [free temporary license][11] for _Aspose.Slides for .NET_ to avoid the trial limitations.

## See Also

*   [Convert PowerPoint PPT/PPTX to PDF][12]




[1]: https://products.aspose.app/slides/conversion/ppt-to-jpg
[2]: https://products.aspose.app/slides/conversion/pptx-to-jpg
[3]: https://products.aspose.com/slides/net
[4]: https://downloads.aspose.com/slides/net
[5]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[6]: https://apireference.aspose.com/net/slides/aspose.slides/islide
[7]: https://apireference.aspose.com/net/slides/aspose.slides/presentation/properties/slides
[8]: https://docs.microsoft.com/en-us/dotnet/api/system.drawing.bitmap?view=netframework-4.8
[9]: https://apireference.aspose.com/net/slides/aspose.slides.islide/getthumbnail/methods/6
[10]: https://docs.microsoft.com/en-us/dotnet/api/system.drawing.image.save?view=netframework-4.8
[11]: https://purchase.aspose.com/temporary-license
[12]: https://blog.aspose.com/2019/12/31/convert-powerpoint-ppt-pptx-to-pdf-in-java-using-aspose-slides/





