---
title: 'Convert PowerPoint Presentations to SVG in C#'
seoTitle: "C# Convert PowerPoint to SVG | PPTX PPT Slides to SVG in C#"
description: "Use .NET PowerPoint API to convert slides in PowerPoint PPTX/PPT to SVG using C# or VB.NET. Create your PowerPoint viewer in ASP.NET."
date: Tue, 17 Aug 2021 16:03:34 +0000
draft: false
url: /2021/08/17/convert-powerpoint-slides-to-svg-in-csharp/
author: Usman Aziz
summary: 'PowerPoint to [SVG][1] conversion is often used to embed the content of the slides in web or desktop applications. Various online PowerPoint viewers also convert the presentations to SVG for slideshow. In accordance with that, this article covers **how to convert PowerPoint PPTX/PPT presentations to SVG format using C#**.'
tags: ['PPT to SVG Csharp', 'PPTX to SVG Csharp', 'PowerPoint to SVG Csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/PowerPoint-to-SVG.jpg" alt="PowerPoint to SVG C#">}}


PowerPoint to [SVG][2] conversion is often used to embed the content of the slides in web or desktop applications. Various online PowerPoint viewers also convert the presentations to SVG for slideshow. In accordance with that, this article covers **how to convert PowerPoint PPTX/PPT presentations to SVG format using C#**.

*   [PowerPoint to SVG Converter][3]
*   [Convert PPTX/PPT to SVG in C#][4]

## C# PowerPoint Presentation to SVG Converter {#PowerPoint-Presentation-to-SVG-Converter}

[Aspose.Slides for .NET][5] is designed to create and manipulate PowerPoint and OpenOffice presentations from within .NET applications. In addition, the API allows you to convert presentation documents to other formats such as SVG. You can either [download][6] the API or install it using [NuGet][7].

```
PM> Install-Package Aspose.Slides.NET
```

## Convert PPTX/PPT Presentations to SVG in C# {#Convert-PPTX-PPT-to-SVG}

The following are the steps to convert a PowerPoint PPTX/PPT presentation to SVG using C#.

*   First, create an instance of [Presentation][8] class to load the presentation.
*   Loop through the slides in [Presentation.Slides][9] collection.
*   Get the reference of each slide in [ISlide][10] object.
*   Write slide into a [MemoryStream][11] object using [ISlide.WriteAsSvg()][12] method.
*   Create a [Stream][13] object for resultant SVG file.
*   Write SVG data from [MemoryStream][14] object to SVG file's stream.
*   Finally, close the stream.

The following code sample shows how to convert PowerPoint PPTX/PPT to SVG.

{{< gist aspose-com-gists df9a0ef94c2a4183f353cecfde38238f "powerpoint-to-svg.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for .NET without evaluation limitations by requesting a [temporary license][15].

## Online Demo

Try the [online PowerPoint to SVG converter][16], which is based on Aspose.Slides.

## Conclusion

The slides in PowerPoint presentations are often converted to SVG for presentation viewers. For such use cases, this article covered how to convert PowerPoint presentations to SVG using C#. You can also visit the [documentation][17] to explore other features of Aspose.Slides for .NET. Also, you can feel free to let us know about your queries via our [forum][18].

## See Also

*   [Create MS PowerPoint Presentations in C#][19]




[1]: https://docs.fileformat.com/page-description-language/svg/
[2]: https://docs.fileformat.com/page-description-language/svg/
[3]: #PowerPoint-Presentation-to-SVG-Converter
[4]: #Convert-PPTX-PPT-to-SVG
[5]: https://products.aspose.com/slides/net
[6]: https://downloads.aspose.com/slides/net
[7]: https://www.nuget.org/packages/Aspose.Slides
[8]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[9]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/slides
[10]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[11]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream
[12]: https://apireference.aspose.com/slides/net/aspose.slides/islide/methods/writeassvg
[13]: https://docs.microsoft.com/en-us/dotnet/api/system.io.stream
[14]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream
[15]: https://purchase.aspose.com/temporary-license
[16]: https://products.aspose.app/slides/conversion/ppt-to-svg
[17]: https://docs.aspose.com/slides/net/developer-guide/
[18]: https://forum.aspose.com/
[19]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/





