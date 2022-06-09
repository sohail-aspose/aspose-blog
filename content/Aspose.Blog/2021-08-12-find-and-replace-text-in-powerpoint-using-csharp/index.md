---
title: 'Find and Replace Text in PowerPoint PPTX/PPT using C#'
seoTitle: "C# Find and Replace Text in PowerPoint PPTX PPT | .NET PowerPoint API"
description: "Use .NET PowerPoint API to find and replace text in PowerPoint presentations using C# .NET. Find and replace text in PPTX or PPT presentations."
date: Thu, 12 Aug 2021 19:11:00 +0000
draft: false
url: /2021/08/12/find-and-replace-text-in-powerpoint-using-csharp/
author: Usman Aziz
summary: 'Finding and replacing text is often used to update the content in PowerPoint presentations. However, in order to perform this operation for a batch of presentations, you need automation. Accordingly, this article covers **how to find and replace text in PowerPoint PPTX/PPT programmatically using C#**.'
tags: ['Search and replace text in powerpoint csharp', 'find and replace text in powerpoint csharp', 'find and replace text in ppt csharp', 'find and replace text in pptx csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Find-and-Replace-Text-in-PowerPoint.jpg" alt="C# FInd and Replace Text in PowerPoint">}}


Finding and replacing text is often used to update the content in PowerPoint presentations. However, in order to perform this operation for a batch of presentations, you need automation. Accordingly, this article covers **how to find and replace text in PowerPoint PPTX/PPT programmatically using C#**.

*   [API to Find and Replace Text in PowerPoint][1]
*   [Find and Replace Text in PPTX using C#][2]

## C# API to Find and Replace Text in PowerPoint {#API-to-Find-and-Replace-Text-in-PowerPoint}

In order to find and replace text in PowerPoint presentations, we'll use [Aspose.Slides for .NET][3]. It is a feature-rich API that is designed to create and manipulate PowerPoint presentations from within .NET applications. You can either [download][4] the API or install it using [NuGet][5].

```
PM> Install-Package Aspose.Slides.NET
```

## Find and Replace Text in PowerPoint PPTX using C# {#Find-and-Replace-Text-in-PPTX}

The following are the steps to find and replace text in a PPTX presentation using C#.

*   Load the PowerPoint presentation using [Presentation][6] class.
*   Loop through each [Slide][7] in the presentation.
*   In each iteration, get text frames in an [ITextFrame][8] array.
*   Loop through array of ITextFrame and in each iteration, perform the following operations:
    *   Loop through the [ParagraphCollection][9] in each text frame.
    *   Access the [PortionCollection][10] in each [Paragraph][11].
    *   Check if [Portion.Text][12] contains the search string.
    *   If yes, find the position of the search string and replace it by setting [Portion.Text][13] property.
*   Save the updated presentation using [Presentation.Save(string, SaveFormat)][14] method.

The following code sample shows how to find and replace text in a PowerPoint presentation.

{{< gist aspose-com-gists d3e06dfe06c9cebddb252bc1a2f30f52 "find-replace-text-in-PowerPoint.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for .NET without evaluation limitations by requesting a [temporary license][15].

## Conclusion

The feature of finding and replacing text in PowerPoint presentations is used in various scenarios. In order to automate this operation, the article covered how to find and replace text in PowerPoint presentations programmatically using C#. You can simply install the API in your application and integrate the provided code sample. In addition, you can visit the [documentation][16] to explore other features of Aspose.Slides for .NET. Also, you can feel free to let us know about your queries via our [forum][17].

## See Also

*   [Create MS PowerPoint Presentations in C#][18]




[1]: #API-to-Find-and-Replace-Text-in-PowerPoint
[2]: #Find-and-Replace-Text-in-PPTX
[3]: https://products.aspose.com/slides/net
[4]: https://downloads.aspose.com/slides/net
[5]: https://www.nuget.org/packages/Aspose.Slides.Net
[6]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[7]: https://apireference.aspose.com/slides/net/aspose.slides/slide
[8]: https://apireference.aspose.com/slides/net/aspose.slides/itextframe
[9]: https://apireference.aspose.com/slides/net/aspose.slides/paragraphcollection
[10]: https://apireference.aspose.com/slides/net/aspose.slides/portioncollection
[11]: https://apireference.aspose.com/slides/net/aspose.slides/paragraph
[12]: https://apireference.aspose.com/slides/net/aspose.slides/portion/properties/text
[13]: https://apireference.aspose.com/slides/net/aspose.slides/portion/properties/text
[14]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[15]: https://purchase.aspose.com/temporary-license
[16]: https://docs.aspose.com/slides/net/developer-guide/
[17]: https://forum.aspose.com/
[18]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/





