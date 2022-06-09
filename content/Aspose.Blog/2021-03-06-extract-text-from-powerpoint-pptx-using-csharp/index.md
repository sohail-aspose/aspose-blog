---
title: 'Extract Text from PowerPoint Files using C#'
seoTitle: "Extract Text From PowerPoint PPTX/PPT in C# | Extract Text from Slides"
description: "Use .NET PowerPoint API to extract text from PowerPoint PPTX/PPT presentations in C#. Extract text from a specific slide of from the whole presentation."
date: Sat, 06 Mar 2021 18:10:17 +0000
draft: false
url: /2021/03/06/extract-text-from-powerpoint-pptx-using-csharp/
author: Usman Aziz
summary: 'You may often need to extract text from the PowerPoint slides in order to perform text analysis. On the other hand, you may want to extract and save the text in a file or database for further processing. In accordance with that, this article covers **how to extract text from PowerPoint presentations using C#**. Particularly, you will learn how to extract text from a specific slide or whole presentation.'
tags: ['API to Extract Text From PowerPoint PPTX', 'Extract Text from PowerPoint Presentation csharp', 'Extract Text from a PowerPoint Slide csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Extract-Text-from-PowerPoint.jpg" alt="Extract Text from PowerPoint C#">}}


You may often need to extract text from the PowerPoint slides in order to perform text analysis. On the other hand, you may want to extract and save the text in a file or database for further processing. In accordance with that, this article covers **how to extract text from PowerPoint presentations using C#**. Particularly, you will learn how to extract text from a specific slide or whole presentation.

*   [API to Extract Text from PowerPoint PPTX][1]
*   [Extract Text from a PowerPoint Slide][2]
*   [Extract Text from a PowerPoint Presentation][3]
*   [Get a Free API License][4]

## C# API to Extract Text from PowerPoint PPTX {#CSharp-API-to-Extract-Text-From-PowerPoint-PPTX}

In order to manipulate PowerPoint presentations, Aspose offers [Aspose.Slides for .NET][5]. The said API is designed to implement PowerPoint automation features in .NET applications. It also provides some simple ways of extracting text from the PPTX presentations. You can either [download][6] the API or get it installed using [NuGet][7].

```
PM> Install-Package Aspose.Slides.NET
```

## Extract Text from a PowerPoint Slide in C# {#Extract-Text-from-a-PowerPoint-Slide-in-CSharp}

The following are the steps to extract text from a slide in a PowerPoint presentation.

*   Load the presentation using [Presentation][8] class.
*   Get all the text frames from a slide into [ITextFrame][9] array using [SlideUtil.GetAllTextBoxes()][10] method.
*   Loop through each [ITextFrame][11] and access its text using [ITextFrame.Paragraphs][12] property.
*   Retrieve and print text from each [Portion][13] of the paragraph.

The following code sample shows how to extract text from a PowerPoint slide using C#.

{{< gist aspose-com-gists fa06076425f4fd9b9ed20591f404b529 "extract-text-from-slide.cs" >}}

## Extract Text from PowerPoint Presentation in C# {#Extract-Text-from-PowerPoint-Presentation-in-CSharp}

You can also extract text from the whole PowerPoint presentation using Aspose.Slides for .NET. The following are the steps to perform this operation.

*   Load the presentation using [Presentation][14] class.
*   Get all the text frames in presentation using [SlideUtil.GetAllTextFrames()][15] method.
*   Loop through each [ITextFrame][16] and access its [Paragraphs][17].
*   Access the portions of the paragraphs and print their text.

The following code sample shows how to extract text from a PowerPoint presentation.

{{< gist aspose-com-gists fa06076425f4fd9b9ed20591f404b529 "extract-text-from-presentation.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

In case you want to try the API without evaluation limitations, you can [get a free temporary license][18].

## Conclusion

In this article, you have learned how to extract text from PowerPoint presentations. Particularly, you have seen how to extract text from a specific slide or the whole presentation using C#. You can explore more about Aspose.Slides for .NET using [documentation][19]. In case you would have any queries or confusion, inform us via our [forum][20].

## See Also

*   [Convert PowerPoint PPT or PPTX to PDF using C#][21]




[1]: #CSharp-API-to-Extract-Text-From-PowerPoint-PPTX
[2]: #Extract-Text-from-a-PowerPoint-Slide-in-CSharp
[3]: #Extract-Text-from-PowerPoint-Presentation-in-CSharp
[4]: #Get-a-Free-API-License
[5]: https://products.aspose.com/slides/net
[6]: https://downloads.aspose.com/slides/net
[7]: https://www.nuget.org/packages/Aspose.Slides.Net
[8]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[9]: https://apireference.aspose.com/slides/net/aspose.slides/itextframe
[10]: https://apireference.aspose.com/slides/net/aspose.slides.util/slideutil/methods/getalltextboxes
[11]: https://apireference.aspose.com/slides/net/aspose.slides/itextframe
[12]: https://apireference.aspose.com/slides/net/aspose.slides/itextframe/properties/paragraphs
[13]: https://apireference.aspose.com/slides/net/aspose.slides/portion
[14]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[15]: https://apireference.aspose.com/slides/net/aspose.slides.util/slideutil/methods/getalltextframes
[16]: https://apireference.aspose.com/slides/net/aspose.slides/itextframe
[17]: https://apireference.aspose.com/slides/net/aspose.slides/itextframe/properties/paragraphs
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/slides/net/
[20]: https://forum.aspose.com/
[21]: https://blog.aspose.com/2020/02/12/convert-powerpoint-ppt-pptx-to-pdf-in-csharp-net/





