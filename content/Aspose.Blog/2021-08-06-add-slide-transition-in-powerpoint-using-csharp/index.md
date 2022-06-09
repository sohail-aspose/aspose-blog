---
title: 'Add Slide Transitions in PowerPoint Presentations using C#'
seoTitle: "Add Slide Transition in PowerPoint using C# | Add Morph Transition"
description: "Use .NET PowerPoint API to add slide transitions in PowerPoint presentations using C# or VB.NET. Set morph transition in PowerPoint programmatically."
date: Fri, 06 Aug 2021 14:30:00 +0000
draft: false
url: /2021/08/06/add-slide-transition-in-powerpoint-using-csharp/
author: Usman Aziz
summary: 'Slide transitions are the visual effects that appear when you move from one slide to another in PowerPoint presentations. Moreover, you can set transition sound, speed, duration, and other effects as per your choice. In this article, you will learn **how to add slide transitions in PowerPoint presentations programmatically using C#**.'
tags: ['Add Morph Slide Transition using Csharp', 'Add Slide Transition in PowerPoint Csharp', 'Add Slide Transition using Csharp', 'Dotnet PowerPoint API']
categories: ['Aspose.Slides Product Family']
---

Slide transitions are the visual effects that appear when you move from one slide to another in PowerPoint presentations. Moreover, you can set transition sound, speed, duration, and other effects as per your choice. In this article, you will learn **how to add slide transitions in PowerPoint presentations programmatically using C#**.

*   [.NET API to Add Slide Transitions in PowerPoint][1]
*   [Add Slide Transition using C#][2]
*   [Add Advanced Slide Transitions][3]
*   [Morph Transitions in PowerPoint][4]

## .NET API to Add Slide Transitions in PowerPoint {#API-to-Add-Slide-Transition-in-PowerPoint}

In order to add transitions to the slides in PowerPoint presentations, we will use [Aspose.Slides for .NET][5]. It is a .NET API to create and manipulate the PowerPoint and OpenOffice documents. You can either [download][6] the API or install it using [NuGet][7].

```
PM> Install-Package Aspose.Slides.NET 
```

## Add Slide Transition using C# {#Add-Slide-Transition}

The following are the steps to add slide transition in a PowerPoint presentation using C#.

1.  First, load the PowerPoint presentation using [Presentation][8] class.
2.  Then, set a slide transition type using [SlideShowTransition.Type][9] property and [TransitionType][10] enum.
3.  Finally, save the updated presentation using [Presentation.Save(String, SaveFormat)][11] method.

The following code sample shows how to set the transition of a slide in a PowePoint presentation.

{{< gist aspose-com-gists f122aab627a2b7b58544894c52d9935b "add-transition.cs" >}}

## Add Advanced Slide Transitions using C# {#Add-Advanced-Slide-Transition}

The following are the steps to set advanced slide transition options such as duration, sound, speed, etc.

1.  First, load the PowerPoint presentation using [Presentation][12] class.
2.  Set a slide transition type using [SlideShowTransition.Type][13] property and [TransitionType][14] enum.
3.  Set a advanced effects such as [SlideShowTransition.Sound][15], [SlideShowTransition.AdvanceAfterTime][16], etc. ([see list of effects][17].
4.  Finally, save the updated presentation using [Presentation.Save(String, SaveFormat)][18] method.

The following code sample shows how to set advanced slide transition options in a PowerPoint presentation.

{{< gist aspose-com-gists f122aab627a2b7b58544894c52d9935b "add-advance-transition.cs" >}}

## Set Morph Transition in PowerPoint using C# {#Morph-Transition-in-PowerPoint}

Using Aspose.Slides for .NET, you can also set the morph transitions, which are used to make smooth animations. The following morph transitions are supported by the API:

*   [ByObject][19]: Morph transition will be performed considering shapes as indivisible objects.
*   [ByWord][20]: Morph transition will be performed with transferring text by words where possible.
*   [ByChar][21]: Morph transition will be performed with transferring text by characters where possible.

The following are the steps to add morph transition in a PowerPoint presentation using C#.

1.  First, load the PowerPoint presentation using [Presentation][22] class.
2.  Set [SlideShowTransition.Type][23] property to [TransitionType.Morph][24].
3.  Set morph transition type using [((IMorphTransition)presentation.Slides\[0\].SlideShowTransition.Value).MorphType][25] property.
4.  Finally, save the updated presentation using [Presentation.Save(String, SaveFormat)][26] method.

The following code sample shows how to set morph transitions in a PowerPoint presentation.

{{< gist aspose-com-gists f122aab627a2b7b58544894c52d9935b "add-morph-transition.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for .NET without evaluation limitations by requesting a [temporary license][27].

## Conclusion

In this article, you have learned how to add slide transitions in PowerPoint presentations using C#. Moreover, you have seen how to set morph transitions in the slides programmatically. In addition, you can visit the [documentation][28] to explore other features of API. Also, you can feel free to let us know about your queries via our [forum][29].

## See Also

*   [Create MS PowerPoint Presentations in C#][30]
*   [Convert PowerPoint PPTX/PPT to PNG Images in C#][31]
*   [Set Slide Background in PowerPoint Presentations using C#][32]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using C#][33]
*   [Apply Animation to Text in PowerPoint using C#][34]




[1]: #API-to-Add-Slide-Transition-in-PowerPoint
[2]: #Add-Slide-Transition
[3]: #Add-Advanced-Slide-Transition
[4]: #Morph-Transition-in-PowerPoint
[5]: https://products.aspose.com/slides/net
[6]: https://downloads.aspose.com/slides/net
[7]: https://www.nuget.org/packages/Aspose.Slides.NET
[8]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[9]: https://apireference.aspose.com/slides/net/aspose.slides/islideshowtransition/properties/type
[10]: https://apireference.aspose.com/slides/net/aspose.slides.slideshow/transitiontype
[11]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[12]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[13]: https://apireference.aspose.com/slides/net/aspose.slides/islideshowtransition/properties/type
[14]: https://apireference.aspose.com/slides/net/aspose.slides.slideshow/transitiontype
[15]: https://apireference.aspose.com/slides/net/aspose.slides/islideshowtransition/properties/sound
[16]: https://apireference.aspose.com/slides/net/aspose.slides/islideshowtransition/properties/advanceaftertime
[17]: https://apireference.aspose.com/slides/net/aspose.slides/islideshowtransition)
[18]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[19]: https://apireference.aspose.com/slides/net/aspose.slides.slideshow/transitionmorphtype
[20]: https://apireference.aspose.com/slides/net/aspose.slides.slideshow/transitionmorphtype
[21]: https://apireference.aspose.com/slides/net/aspose.slides.slideshow/transitionmorphtype
[22]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[23]: https://apireference.aspose.com/slides/net/aspose.slides/islideshowtransition/properties/type
[24]: https://apireference.aspose.com/slides/net/aspose.slides.slideshow/transitiontype
[25]: https://apireference.aspose.com/slides/net/aspose.slides.slideshow/imorphtransition/properties/morphtype
[26]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[27]: https://purchase.aspose.com/temporary-license
[28]: https://docs.aspose.com/slides/net/developer-guide/
[29]: https://forum.aspose.com/
[30]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/
[31]: https://blog.aspose.com/2021/09/01/convert-powerpoint-to-png-in-csharp/
[32]: https://blog.aspose.com/2021/08/31/set-background-in-powerpoint-using-csharp/
[33]: https://blog.aspose.com/2021/08/30/generate-pptx-thumbnails-using-csharp/
[34]: https://blog.aspose.com/2021/08/20/apply-animation-to-text-in-powerpoint-using-csharp/





