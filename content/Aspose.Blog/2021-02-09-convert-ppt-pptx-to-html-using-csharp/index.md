---
title: 'Convert PowerPoint Files to HTML using C#'
seoTitle: "Convert PowerPoint to HTML in C# | C# PPT PPTX to HTML"
description: "Use .NET PowerPoint API to convert PPT or PPTX files to HTML using C#. Include or exclude hidden slides in PowerPoint to HTML conversion in C#."
date: Tue, 09 Feb 2021 03:27:00 +0000
draft: false
url: /2021/02/09/convert-ppt-pptx-to-html-using-csharp/
author: Usman Aziz
summary: 'In various scenarios, MS PowerPoint presentations are converted into images or HTML files. For example, when you need to embed presentation slides on a webpage or display them within a desktop application. For such cases, this article provides you a step by step guide of **how to convert PowerPoint PPT/PPTX files to HTML using C#**. Furthermore, you will learn how to include or exclude the hidden slides of a presentation in the converted HTML.'
tags: ['powerpoint to html converter', 'powerpoint to html csharp', 'ppt to html csharp', 'pptx to html csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/PPTX-to-HTML-1.jpg" alt="PPTX to HTML C#">}}


In various scenarios, MS PowerPoint presentations are converted into images or [HTML][1] files. For example, when you need to embed presentation slides on a webpage or display them within a desktop application. For such cases, this article provides you a step by step guide of **how to convert PowerPoint [PPT][2] or [PPTX][3] files to HTML using C#**. Furthermore, you will learn how to include or exclude the hidden slides of a presentation in the converted HTML.

*   [C# PowerPoint to HTML Converter API][4]
*   [Convert PowerPoint PPTX to HTML in C#][5]
*   [PPT/PPTX to HTML Conversion with Hidden Slides][6]
*   [Get a Free API License][7]

## C# PowerPoint to HTML Converter API {#CSharp-PowerPoint-to-HTML-Converter-API}

[Aspose.Slides for .NET][8] is a presentation manipulation API that lets you create and process PowerPoint presentations from within your .NET applications. Along with other PowerPoint automation features, The API allows you to convert PPT/PPTX presentations to other formats including HTML. You can either [download][9] the API's DLL or install it using [NuGet][10].

```
PM> Install-Package Aspose.Slides.NET
```

## Convert PowerPoint PPTX to HTML in C# {#Convert-PowerPoint-PPTX-to-HTML-in-CSharp}

The following are the steps to convert a PowerPoint PPTX file to HTML using Aspose.Slides for .NET.

*   Load the PowerPoint presentation using [Presentation][11] class.
*   Create an instance of [HtmlOptions][12] class.
*   Convert PPTX to HTML using [Presentation.Save(String, HtmlOptions)][13] method.

The following code sample shows how to convert a PowerPoint PPTX to HTML using C#.

{{< gist aspose-com-gists 8c0a42b70e108edd4a67e1f3913cba94 "pptx-to-html.cs" >}}

### PowerPoint Presentation



{{< figure align=center src="images/pptx.jpg" alt="PPTX File">}}


### Converted HTML



{{< figure align=center src="images/pptx-to-html.jpg" alt="PPTX to HTML C#">}}


## C# PPT/PPTX to HTML Conversion with Hidden Slides {#PPT-PPTX-to-HTML-Conversion-with-Hidden-Slides}

PowerPoint presentations may also include hidden slides. By default, the hidden slides are excluded in conversion to HTML. However, you can configure the API to include the hidden slides as well. The following are the steps to perform this operation.

*   Load the PowerPoint presentation using [Presentation][14] class.
*   Create an instance of [HtmlOptions][15] class.
*   Set [HtmlOptions.ShowHiddenSlides][16] property to _true_.
*   Convert PPTX to HTML using [Presentation.Save(String, HtmlOptions)][17] method.

The following code sample shows how to include hidden slides in PPTX to HTML conversion in C#.

{{< gist aspose-com-gists 8c0a42b70e108edd4a67e1f3913cba94 "pptx-to-html-hidden-slides.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [get a free temporary license][18] in order to try the API without evaluation limitations.

## Conclusion

PowerPoint to HTML conversion is adopted in various scenarios. In accordance with that, in this article, you have learned how to convert PowerPoint PPT/PPTX files to HTML using C#. Furthermore, you have seen how to include the hidden slides in PPTX to HTML conversion. You can explore more about Aspose.Slides for .NET using the [documentation][19].

## See Also

*   [Create MS PowerPoint Presentations in C#][20]




[1]: https://docs.fileformat.com/web/html/
[2]: https://docs.fileformat.com/presentation/ppt/
[3]: https://docs.fileformat.com/presentation/pptx/
[4]: #CSharp-PowerPoint-to-HTML-Converter-API
[5]: #Convert-PowerPoint-PPTX-to-HTML-in-CSharp
[6]: #PPT-PPTX-to-HTML-Conversion-with-Hidden-Slides
[7]: #Get-a-Free-API-License
[8]: https://products.aspose.com/slides/net
[9]: https://downloads.aspose.com/slides/net
[10]: https://www.nuget.org/packages/Aspose.Slides.Net
[11]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[12]: https://apireference.aspose.com/slides/net/aspose.slides.export/htmloptions
[13]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/4
[14]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[15]: https://apireference.aspose.com/slides/net/aspose.slides.export/htmloptions
[16]: https://apireference.aspose.com/slides/net/aspose.slides.export/htmloptions/properties/showhiddenslides
[17]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/4
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/slides/net
[20]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/





