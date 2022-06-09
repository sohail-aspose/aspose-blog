---
title: 'Split PowerPoint Presentations using C#'
seoTitle: "Split PowerPoint Presentations using C# | .NET PowerPoint API"
description: "Use .NET PowerPoint API to split PPTX/PPT presentations using C# or VB.NET. Split each slide in the presentation and save it as a separate file."
date: Fri, 03 Sep 2021 15:50:28 +0000
draft: false
url: /2021/09/03/split-powerpoint-presentations-using-csharp/
author: Usman Aziz
summary: 'In various cases, you may need to split the PowerPoint presentations into multiple files. For example, to split a presentation by each slide, even or odd slides, and so on. In this article, you will learn **how to split the PowerPoint PPTX/PPT presentations using C#**.'
tags: ['split powerpoint presentation csharp', 'split ppt presentation csharp', 'split pptx presentation csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Split-PowerPoint-Presentation.jpg" alt="Split PowerPoint Presentation C#">}}


In various cases, you may need to split the PowerPoint presentations into multiple files. For example, to split a presentation by each slide, even or odd slides, and so on. In this article, you will learn **how to split the PowerPoint PPTX/PPT presentations using C#**.

*   [.NET API to Split PowerPoint Presentations][1]
*   [Split a PowerPoint Presentation using C#][2]

## .NET API to Split PowerPoint Presentations {#NET-API-to-Split-PowerPoint-Presentations}

In order to split PPTX or PPT presentations, we will use [Aspose.Slides for .NET][3]. It is a presentation manipulation API that lets you create, modify and convert PowerPoint and OpenOffice presentations from within your .NET applications. You can either [download][4] the API or install it using [NuGet][5].

```
PM> Install-Package Aspose.Slides.NET
```

## Split a PowerPoint Presentation using C# {#Split-a-PowerPoint-Presentation}

The following are the steps to split a PowerPoint presentation using C#.

*   First, create an instance of the [Presentation][6] class to load the PowerPoint presentation.
*   Then, loop through each [ISlide][7] in [Presentation.Slides][8] collection.
*   In each iteration, perform the following steps:
    *   Create an instance of [Presentation][9] class.
    *   Remove the default slide using [Presentation.Slides\[0\].Remove()][10] method.
    *   Add the slide to the presentation using [Presentation.Slides.AddClone(ISlide)][11] method.
    *   Finally, save the presentation using [Presentation.Save(String, SaveFormat)][12] method.

The following code sample shows how to split a PowerPoint PPTX presentation.

{{< gist aspose-com-gists e100eb12855796c52c407ac2fa23eb10 "split-presentation.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for .NET without evaluation limitations by requesting a [temporary license][13].

## Online Demo

Try the [online presentation splitter][14], which is based on Aspose.Slides.

## Conclusion

In this article, you have learned how to split PowerPoint PPTX or PPT presentations using C#. You can customize the provided code sample to define your own splitting criteria. For example, you can split each slide in the presentation, all the even or odd slides, etc. You can simply install the API and integrate the provided code into your application. In addition, you can visit the [documentation][15] to explore other features of API. Also, you can feel free to let us know about your queries via our [forum][16].

## See Also

*   [Create MS PowerPoint Presentations in C#][17]
*   [Convert PowerPoint PPTX/PPT to PNG Images in C#][18]
*   [Set Slide Background in PowerPoint Presentations using C#][19]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using C#][20]
*   [Apply Animation to Text in PowerPoint using C#][21]




[1]: #NET-API-to-Split-PowerPoint-Presentations
[2]: #Split-a-PowerPoint-Presentation
[3]: https://products.aspose.com/slides/net
[4]: https://downloads.aspose.com/slides/net
[5]: https://www.nuget.org/packages/Aspose.Slides.NET
[6]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[7]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[8]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/slides
[9]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[10]: https://apireference.aspose.com/slides/net/aspose.slides/islide/methods/remove
[11]: https://apireference.aspose.com/slides/net/aspose.slides/islidecollection/methods/addclone
[12]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[13]: https://purchase.aspose.com/temporary-license
[14]: https://products.aspose.app/slides/splitter
[15]: https://docs.aspose.com/slides/net/developer-guide/
[16]: https://forum.aspose.com/
[17]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/
[18]: https://blog.aspose.com/2021/09/01/convert-powerpoint-to-png-in-csharp/
[19]: https://blog.aspose.com/2021/08/31/set-background-in-powerpoint-using-csharp/
[20]: https://blog.aspose.com/2021/08/30/generate-pptx-thumbnails-using-csharp/
[21]: https://blog.aspose.com/2021/08/20/apply-animation-to-text-in-powerpoint-using-csharp/




