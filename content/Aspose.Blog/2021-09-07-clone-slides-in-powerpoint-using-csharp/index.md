---
title: 'Clone Slides in PowerPoint Presentations using C#'
seoTitle: "Clone Slides in PowerPoint PPTX/PPT using C# | .NET Presentation API"
description: "Use .NET PowerPoint API to clone slides in PowerPoint PPTX PPT presentations using C# or VB.NET. Clone slides within or in another presentation."
date: Tue, 07 Sep 2021 16:10:17 +0000
draft: false
url: /2021/09/07/clone-slides-in-powerpoint-using-csharp/
author: Usman Aziz
summary: 'In certain cases, you may need to clone the slides in PowerPoint presentations. The cloning process makes the copy of a slide within or in another presentation without changing the original slide. In this article, you will learn how to automate slide cloning in PowerPoint presentations. Particularly, the article will cover **how to clone slides within a PowerPoint presentation or from one presentation to another using C#**.'
tags: ['clone slides in powerpoint csharp', 'clone slides in ppt csharp', 'clone slides in pptx csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Clone-Slides-in-PowerPoint.jpg" alt="Clone Slides in PowerPoint C#">}}


In certain cases, you may need to clone the slides in PowerPoint presentations. The cloning process makes the copy of a slide within or in another presentation without changing the original slide. In this article, you will learn how to automate slide cloning in PowerPoint presentations. Particularly, the article will cover **how to clone slides within a PowerPoint presentation or from one presentation to another using C#**.

*   [.NET API to Clone Slides in PowerPoint Presentations][1]
*   [Clone Slide within a PowerPoint Presentation][2]
    *   [Copy Slide at the End of Presentation][3]
    *   [Clone Slide to a Specific Position][4]
*   [Clone Slide into Another Presentation][5]
    *   [Copy Slide at the End of Another Presentation][6]
    *   [Clone Slide to a Specific Position of Another Presentation][7]

## .NET API to Clone Slides in PowerPoint Presentations {#API-to-Clone-Slides-in-PowerPoint-Presentations}

In order to clone slides in PPTX or PPT presentations, we will use [Aspose.Slides for .NET][8]. It is a presentation manipulation API that lets you create, modify and convert PowerPoint and OpenOffice presentations. You can either [download][9] the API or install it using [NuGet][10].

```
PM> Install-Package Aspose.Slides.NET
```

## Clone Slides within a PowerPoint Presentation in C# {#Clone-Slide-within-a-PowerPoint-Presentations}

You can clone a slide either at a specified location or at the end of the PowerPoint presentation. The following sections demonstrate each of the above-mentioned scenarios with code samples.

### Clone Slide at the End of Presentation {#Clone-Slide-at-the-End-of-Presentation}

The following are the steps to clone a slide at the end of a PowerPoint presentation using C#.

1.  First, load the PowerPoint presentation using [Presentation][11] class.
2.  Get reference of the slide collection using [Presentation.Slides][12] into an [ISlideCollection][13] object.
3.  Clone desired slide using [ISlideCollection.AddClone(ISlide)][14] method by specifying the slide to be cloned as a parameter.
4.  Finally, save the presentation using [Presentation.Save(String, SaveFormat)][15] method.

The following code sample shows how to clone a slide at the end of the PowerPoint presentation.

{{< gist aspose-com-gists cfb9b18a6c25c6e4501787e37300adab "clone-slide-at-end.cs" >}}

### Clone Slide to a Specific Position in Presentation {#Clone-Slide-to-a-Specific-Position}

The following are the steps to clone a slide at a specific position in the PowerPoint presentation using C#.

1.  Load the PowerPoint presentation using [Presentation][16] class.
2.  Get reference of the slide collection using [Presentation.Slides][17] into an [ISlideCollection][18] object.
3.  Clone desired slide using [ISlideCollection.InsertClone(Int32, ISlide)][19] method by specifying the destination index and slide to be cloned as parameters.
4.  Save the presentation using [Presentation.Save(String, SaveFormat)][20] method.

The following code sample shows how to clone a slide at a specific position in a PowerPoint presentation.

{{< gist aspose-com-gists cfb9b18a6c25c6e4501787e37300adab "clone-slide-at-index.cs" >}}

## Clone Slides into Another Presentation using C# {#Clone-Slide-into-Another-Presentation}

In this section, you will learn how to clone a slide from one presentation to another. The following subsections will cover the cloning of a slide at the end or at a specific position in the destination presentation.

### Clone Slide at the End of Another Presentation {#Copy-Clone-Slide-at-the-End-of-Another-Presentation}

The following are the steps to clone a slide at the end of another presentation using C#.

1.  Load the source PowerPoint presentation using [Presentation][21] class.
2.  Load the destination PowerPoint presentation using [Presentation][22] class.
3.  Get reference of the slide collection from destination presentation into an [ISlideCollection][23] object.
4.  Clone desired slide using [ISlideCollection.AddClone(ISlide)][24] method by specifying the slide to be cloned as a parameter.
5.  Save the destination presentation using [Presentation.Save(String, SaveFormat)][25] method.

The following code sample shows how to clone a slide from one presentation to another.

{{< gist aspose-com-gists cfb9b18a6c25c6e4501787e37300adab "clone-slide-other-presentation.cs" >}}

### Clone Slide to a Specific Position in Another Presentation {#Clone-Slide-to-a-Specific-Position-in-Another-Presentation}

The following are the steps to clone a slide at a specific location in another presentation using C#.

1.  Load the source PowerPoint presentation using [Presentation][26] class.
2.  Load the destination PowerPoint presentation using [Presentation][27] class.
3.  Get reference of the slide collection from destination presentation into an [ISlideCollection][28] object.
4.  Clone desired slide using [ISlideCollection.InsertClone(Int32, ISlide)][29] method by specifying the destination index and slide to be cloned as parameters.
5.  Save the destination presentation using [Presentation.Save(String, SaveFormat)][30] method.

The following code sample shows how to clone a slide into another PowerPoint presentation.

{{< gist aspose-com-gists cfb9b18a6c25c6e4501787e37300adab "clone-slide-at-index-other-presentation.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for .NET without evaluation limitations by requesting a [temporary license][31].

Tip: You may want to check out [Aspose FREE PowerPoint Splitter][32] used to split the slides in presentations and save them as separate files.

## Conclusion

In this article, you have learned how to clone slides in PowerPoint presentations using C#. The article explicitly covered the cloning of slides within a presentation or from one presentation to another. In addition, you can visit the [documentation][33] to explore other features of API. Also, you can feel free to let us know about your queries via our [forum][34].

## See Also

*   [Create MS PowerPoint Presentations in C#][35]
*   [Convert PowerPoint PPTX/PPT to PNG Images in C#][36]
*   [Set Slide Background in PowerPoint Presentations using C#][37]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using C#][38]
*   [Apply Animation to Text in PowerPoint using C#][39]
*   [Split PowerPoint Presentations using C#][40]




[1]: #API-to-Clone-Slides-in-PowerPoint-Presentations
[2]: #Clone-Slide-within-a-PowerPoint-Presentations
[3]: #Clone-Slide-at-the-End-of-Presentation
[4]: #Clone-Slide-to-a-Specific-Position
[5]: #Clone-Slide-into-Another-Presentation
[6]: #Copy-Clone-Slide-at-the-End-of-Another-Presentation
[7]: #Clone-Slide-to-a-Specific-Position-in-Another-Presentation
[8]: https://products.aspose.com/slides/net
[9]: https://downloads.aspose.com/slides/net
[10]: https://www.nuget.org/packages/Aspose.Slides.NET
[11]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[12]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/slides
[13]: https://apireference.aspose.com/net/slides/aspose.slides/islidecollection
[14]: https://apireference.aspose.com/net/slides/aspose.slides/islidecollection/methods/addclone/index
[15]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[16]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[17]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/slides
[18]: https://apireference.aspose.com/net/slides/aspose.slides/islidecollection
[19]: https://apireference.aspose.com/slides/net/aspose.slides/islidecollection/methods/insertclone
[20]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[21]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[22]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[23]: https://apireference.aspose.com/net/slides/aspose.slides/islidecollection
[24]: https://apireference.aspose.com/net/slides/aspose.slides/islidecollection/methods/addclone/index
[25]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[26]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[27]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[28]: https://apireference.aspose.com/net/slides/aspose.slides/islidecollection
[29]: https://apireference.aspose.com/slides/net/aspose.slides/islidecollection/methods/insertclone
[30]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[31]: https://purchase.aspose.com/temporary-license
[32]: https://products.aspose.app/slides/splitter
[33]: https://docs.aspose.com/slides/net/developer-guide/
[34]: https://forum.aspose.com/
[35]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/
[36]: https://blog.aspose.com/2021/09/01/convert-powerpoint-to-png-in-csharp/
[37]: https://blog.aspose.com/2021/08/31/set-background-in-powerpoint-using-csharp/
[38]: https://blog.aspose.com/2021/08/30/generate-pptx-thumbnails-using-csharp/
[39]: https://blog.aspose.com/2021/08/20/apply-animation-to-text-in-powerpoint-using-csharp/
[40]: https://blog.aspose.com/2021/09/03/split-powerpoint-presentations-using-csharp/




