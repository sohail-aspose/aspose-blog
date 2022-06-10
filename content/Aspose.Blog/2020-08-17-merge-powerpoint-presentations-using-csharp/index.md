---
title: 'Merge PowerPoint Presentations using C# or VB.NET'
seoTitle: "Merge PowerPoint Presentations using C# | Merge Multiple PPT/PPTX C#"
description: "Merge or combine PowerPoint PPT/PPTX presentations using C# or VB.NET. Merge all or selected slides from one PowerPoint presentation to other using C#."
date: Mon, 17 Aug 2020 15:22:06 +0000
draft: false
url: /2020/08/17/merge-powerpoint-presentations-using-csharp/
author: Usman Aziz
summary: ''
tags: ['combine multiple presentations in csharp', 'combine powerpoint presentations using csharp', 'merge powerpoint presentations using csharp', 'merge ppt using csharp', 'merge pptx using csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Merge-PowerPoint-files.jpg" alt="Merge PowerPoint files in C#">}}


Merging PowerPoint presentations can be useful in various scenarios such as combining content from multiple PPT/PPTX, merging parts of a single presentation created by two or more people, and etc. The manual way of copying/pasting the content may not be suitable when dealing with a number of presentations. Therefore, this article lets the .NET developers learn **how to merge PowerPoint presentations programmatically using C#**.

**TIP**: You may be interested in trying out a [web viewer app for presentations][1] developed with Aspose’s APIs.

*   [.NET PowerPoint Merger API][2]
*   [Merge PowerPoint Presentations using C#][3]
*   [Merge Particular Slides of PowerPoint Presentations using C#][4]
*   [Use Slide Master while Merging PowerPoint Presentations][5]

## .NET PowerPoint Merger API {#NET-PowerPoint-Merger-API}

[Aspose.Slides for .NET][6] is a feature-rich .NET PowerPoint API that lets you create and manipulate presentation documents. Along with that, it allows you to combine two or more PowerPoint presentations using C# or VB.NET. You can [download][7] the API's DLL or install it using [NuGet][8].

## Merge PowerPoint Presentations using C# {#Merge-PowerPoint-Presentations-using-CSharp}

In this section, you will learn how to clone and merge all the slides from one PowerPoint presentation to another. For this, you can simply clone the slides from the source presentation and add them at the end of the target presentation. The following are the steps to merge two presentations.

*   Create an object of [Presentation][9] class to load the target presentation file.
*   Create another [Presentation][10] object to load the source presentation from where you'll clone the slides.
*   Access the collection of slides from source presentation using [Presentation.Slides][11] property.
*   Loop through the slides collection and merge them into the target presentation using [Presentation.Slides.AddClone(ISlide)][12] method.
*   Save the merged presentation using [Presentation.Save(String, SaveFormat)][13] method.

The following code sample shows how to merge two PowerPoint presentations using C#.

{{< gist aspose-com-gists 02b8b90a3b1b53e565530346be710916 "merge-powerpoint-presentation.cs" >}}

### Target Presentation



{{< figure align=center src="images/merge-presentation1.jpg" alt="target powerpoint presentation">}}


### Source Presentation



{{< figure align=center src="images/merge-presentation2.jpg" alt="source powerpoint presentation to be merged">}}


### Merged Presentation



{{< figure align=center src="images/merged-presentation.jpg" alt="merge powerpoint presentation C#">}}


## Merge Particular Slides of PowerPoint Presentations using C# {#Merge-Particular-Slides-of-PowerPoint-Presentations-using-CSharp}

In the previous example, you have merged all the slides from the source PPTX file into the target PPTX. However, there might be the case when you need to merge only the selected slides. In such a case, you can specify the slides to be merged using the slide's index. The following are the steps to perform this operation.

*   Load the target presentation using the [Presentation][14] class.
*   Load the source presentation using the [Presentation][15] class.
*   Clone the desired slides using _presentation1.Slides.AddClone(presentation2.Slides\[int Index\])_ method.
*   Save the merged presentation as a new PPTX file.

The following code sample shows how to merge particular slides of presentations using C#.

{{< gist aspose-com-gists 02b8b90a3b1b53e565530346be710916 "merge-powerpoint-presentation-selected-slides.cs" >}}

### Merged Presentation



{{< figure align=center src="images/merged-presentation-selected-slides.jpg" alt="merged powerpoint presentation using C#">}}


## Use Slide Master while Merging PowerPoint Presentations {#Use-Slide-Master-while-Merging-PowerPoint-Presentations}

In both of the previous examples, you have merged the slides keeping the design and template of the source presentation. However, in certain cases, you may need to modify the layout of the slides in accordance with the target presentation. In such cases, you can use the overloaded [presentation1.Slides.AddClone(presentation2.Slides\[1\], presentation1.Masters\[0\], true)][16] method.

The following code sample shows how to merge the slides in PowerPoint presentation using the Slide Master in C#.

{{< gist aspose-com-gists 02b8b90a3b1b53e565530346be710916 "merge-powerpoint-presentation-slide-master.cs" >}}

### Merged Presentation



{{< figure align=center src="images/merged-presentation-slide-master.jpg" alt="combined powerpoint presentation using C#">}}


## Conclusion

In this article, you have learned how to **merge two or multiple PowerPoint presentations using C#**. You can port the C# code samples in order to merge presentations using VB.NET. In case you want to explore more about Aspose's .NET PowerPoint API, you can visit the [documentation][17].

## See Also

*   [Create ASP.NET PowerPoint Viewer][18]




[1]: https://products.aspose.app/slides/viewer
[2]: #NET-PowerPoint-Merger-API
[3]: #Merge-PowerPoint-Presentations-using-CSharp
[4]: #Merge-Particular-Slides-of-PowerPoint-Presentations-using-CSharp
[5]: #Use-Slide-Master-while-Merging-PowerPoint-Presentations
[6]: https://products.aspose.com/slides/net
[7]: https://downloads.aspose.com/slides/net
[8]: https://www.nuget.org/packages/Aspose.Slides.Net
[9]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[10]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[11]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/slides
[12]: https://apireference.aspose.com/slides/net/aspose.slides/islidecollection/methods/addclone
[13]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/4
[14]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[15]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[16]: https://apireference.aspose.com/net/slides/aspose.slides.islidecollection/addclone/methods/2
[17]: https://docs.aspose.com/slides/net/developer-guide/
[18]: https://blog.aspose.com/2020/02/23/asp-net-core-powerpoint-viewer-display-ppt-pptx-presentations/





