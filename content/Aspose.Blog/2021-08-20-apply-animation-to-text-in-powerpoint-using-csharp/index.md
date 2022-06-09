---
title: 'Apply Animation to Text in PowerPoint using C#'
seoTitle: "Apply Animation to Text in PowerPoint using C# | Get Animation Effect"
description: "Use .NET PowerPoint API to apply animation effects to text in PowerPoint presentations in C# or VB.NET. Get the animations effects from the text."
date: Fri, 20 Aug 2021 23:45:00 +0000
draft: false
url: /2021/08/20/apply-animation-to-text-in-powerpoint-using-csharp/
author: Usman Aziz
summary: 'Animated text in PowerPoint presentations is used to draw the attention of the audience. Moreover, it brings life to the content of the presentations. You can apply animation effects to text, shapes, and the slides. In this article, you will learn **how to apply animation to the text in PowerPoint using C#**.'
tags: ['Add animation in PowerPoint CSharp', 'Apply Animation to Text in PowerPoint Csharp', 'Get Animation Effects from a Text in PowerPoint csharp']
categories: ['Aspose.Slides Product Family']
---

Animated text in PowerPoint presentations is used to draw the attention of the audience. Moreover, it brings life to the content of the presentations. You can apply animation effects to text, shapes, and the slides. In this article, you will learn **how to apply animation to the text in PowerPoint using C#**.

*   [API to Apply Animation to Text in PowerPoint][1]
*   [Apply Animation to Text in PowerPoint][2]
*   [Get Animation Effects from a Text in PowerPoint][3]

## API to Apply Animation to Text in PowerPoint {#API-to-Apply-Animation-to-Text-in-PowerPoint}

To apply animation to the text in PowerPoint presentations, we will use [Aspose.Slides for .NET][4]. It is a feature-rich and easy-to-use API for creating and manipulating PowerPoint and OpenOffice presentations. You can either [download][5] the API or install it using [NuGet][6].

```
PM> Install-Package Aspose.Slides.NET
```

## Apply Animation to Text in PowerPoint using C# {#Apply-Animation-to-Text-in-PowerPoint}

Aspose.Slides for .NET provides the support of over 150 animation effects including Bounce, PathFootball, Zoom, etc. Moreover, it also provides specific animation effects such as OLEObjectShow and OLEObjectOpen. All the supported animation effects are listed in [EffectType][7] enumeration.

The following are the steps to apply animation to text in a PowerPoint presentation using C#.

*   First, load the presentation using [Presentation][8] class.
*   Select the desired paragraph in an [IParagraph][9] object from the desired slide.
*   Apply animation effect to the text using [Presentation.Slides\[index\].Timeline.MainSequence.AddEffect()][10] method.
*   Finally, save the presentation using [Presentation.Save(String, SaveFormat)][11] method.

The following code sample shows how to apply an animation effect to text in a PowerPoint presentation.

{{< gist aspose-com-gists 8f5af8ca6f64c4af2dc29674b5fb0e97 "apply-text-animation.cs" >}}

## Get Animation Effects from a Text in PowerPoint {#Get-Animation-Effects-from-a-Text-in-PowerPoint}

You can also get information about the animation effect which is applied to a particular text. This can be useful when you need to apply the same effect to another text in the presentation.

The following are the steps to get information about the animation effect applied to a text.

*   First, load the presentation using [Presentation][12] class.
*   Get sequence of the desired slide in [ISequence][13] object.
*   Access the shape from the selected slide in an [IAutoShape][14] object.
*   Loop through each IParagraph in [IAutoShape.TextFrame.Paragraphs][15] collection.
*   Finally, get the effects in an IEffect array using [ISequence.GetEffectsByParagraph(iParagraph)][16] method.

The following code sample shows how to get the information about a text's animation effect.

{{< gist aspose-com-gists 8f5af8ca6f64c4af2dc29674b5fb0e97 "get-text-animation.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for .NET without evaluation limitations by requesting a [temporary license][17].

## Conclusion

In this article, you have learned how to apply animation effects on text in PowerPoint presentations using C#. Furthermore, you have also seen how to get animation effects from a text in a PowerPoint presentation. In order to explore other features of Aspose.Slides for .NET, you can visit the [documentation][18]. Also, you can feel free to let us know about your queries via our [forum][19].

## See Also

*   [Create MS PowerPoint Presentations in C#][20]




[1]: #API-to-Apply-Animation-to-Text-in-PowerPoint
[2]: #Apply-Animation-to-Text-in-PowerPoint
[3]: #Get-Animation-Effects-from-a-Text-in-PowerPoint
[4]: https://products.aspose.com/slides/net
[5]: https://downloads.aspose.com/slides/net
[6]: https://www.nuget.org/packages/Aspose.Slides.Net
[7]: https://apireference.aspose.com/net/slides/aspose.slides.animation/effecttype
[8]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[9]: https://apireference.aspose.com/slides/net/aspose.slides/iparagraph
[10]: https://apireference.aspose.com/slides/net/aspose.slides.animation/sequence/methods/addeffect/index
[11]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[12]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[13]: https://apireference.aspose.com/net/slides/aspose.slides.animation/isequence
[14]: https://apireference.aspose.com/slides/net/aspose.slides/iautoshape
[15]: https://apireference.aspose.com/slides/net/aspose.slides/itextframe/properties/paragraphs
[16]: https://apireference.aspose.com/slides/net/aspose.slides.animation/isequence/methods/geteffectsbyparagraph
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/slides/net/developer-guide/
[19]: https://forum.aspose.com/
[20]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/





