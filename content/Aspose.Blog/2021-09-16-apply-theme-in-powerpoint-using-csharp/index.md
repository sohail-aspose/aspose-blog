---
title: 'Apply Theme in PowerPoint Presentations using C#'
seoTitle: "Apply Theme in PowerPoint Presentations using C# | .NET API"
description: "Use .NET PowerPoint API to apply theme in PowerPoint presentations using C# or VB.NET. Set font, background color, style programmatically."
date: Thu, 16 Sep 2021 15:56:57 +0000
draft: false
url: /2021/09/16/apply-theme-in-powerpoint-using-csharp/
author: Usman Aziz
summary: 'PowerPoint provides a wide range of themes that you can apply in the presentations. In addition, you can define your own custom themes as per your requirements. In this article, you will learn how to work with themes of PowerPoint presentations dynamically, Particularly, the article will cover **how to apply themes in the PowerPoint presentations programmatically using C#**.'
tags: ['Apply Theme to a PowerPoint Presentation in Csharp', 'Change Theme Background Style in Presentation csharp', 'Set Theme Color in the Presentation csharp', 'Set Theme Font in the Presentation csharp']
categories: ['Aspose.Slides Product Family']
---

PowerPoint provides a wide range of themes that you can apply in the presentations. In addition, you can define your own custom themes as per your requirements. In this article, you will learn how to work with themes of PowerPoint presentations dynamically, Particularly, the article will cover **how to apply themes in the PowerPoint presentations programmatically using C#**.

*   [.NET API to Apply Themes in PowerPoint Presentations][1]
*   [Apply Theme to a PowerPoint Presentation in C#][2]
    *   [Set Theme Color in the Presentation][3]
    *   [Set Theme Font in the Presentation][4]
    *   [Change Theme Background Style in Presentation][5]

## .NET API to Apply Themes in PowerPoint Presentations {#API-to-Apply-Themes-in-PowerPoint-Presentations}

In order to apply themes in PowerPoint presentations, we will use [Aspose.Slides for .NET][6]. It is a powerful and feature-rich API to create and manipulate presentations from within .NET applications. You can either [download][7] the API or install it using [NuGet][8].

```
PM> Install-Package Aspose.Slides.NET
```

## Apply Theme in a PowerPoint Presentation using C# {#Apply-Theme-to-a-PowerPoint-Presentation}

A PowerPoint theme represents a set of colors, font size, font family, background style, etc. that you can apply to different elements. In the below sections, we will explicitly cover how to set theme color, font, and background in a PowerPoint presentation.

## Set Theme Color in PowerPoint Presentation using C# {#Set-Theme-Color-in-the-Presentation}

The following are the steps to set a theme color for a shape in PowerPoint presentation using C#.

*   First, load a presentation or create a new one using [Presentation][9] class.
*   Then, add a new shape to the presentation using [AddAutoShape()][10] method.
*   Set [IAutoShape.FillFormat.FillType][11] property.
*   Set [IAutoShape.FillFormat.SolidFillColor.SchemeColor][12] property to desired color.
*   Finally, save the presentation using [Presentation.Save(String, SaveFormat)][13] method.

The following code sample shows how to set a theme color in PowerPoint presentation using C#.

{{< gist aspose-com-gists 5a740f14f61859a0c6a5b59591e263ac "set-theme-color.cs" >}}

## Set Theme Font in the Presentation using C# {#Set-Theme-Font-in-the-Presentation}

Aspose.Slides provides special identifiers to set font from the font scheme. These identifiers are as follows:

*   “**+mn-lt**": Body Font Latin (Minor Latin Font)
*   “**+mj-lt**": Heading Font Latin (Major Latin Font)
*   “**+mn-ea**": Body Font East Asian (Minor East Asian Font)
*   “**+mj-ea**": Body Font East Asian (Minor East Asian Font)

The following are the steps to create an element with the text and assign the Latin font from the font scheme.

*   First, load a presentation or create a new one using [Presentation][14] class.
*   Then, add a new shape to the presentation using [AddAutoShape()][15] method.
*   Create a new [Paragraph][16] and add a [Portion][17] into it.
*   Set Latin font using [Portion.PortionFormat.LatinFont][18] property.
*   Finally, save the presentation using [Presentation.Save(String, SaveFormat)][19] method.

The following code sample shows how to set theme font in a PowerPoint presentation using C#.

{{< gist aspose-com-gists 5a740f14f61859a0c6a5b59591e263ac "set-theme-font.cs" >}}

## Change Theme Background Style in Presentation using C# {#Change-Theme-Background-Style-in-Presentation}

The presentation themes also contain the background styles that you can set in a PowerPoint presentation. The following are the steps to perform this operation.

*   First, load a presentation or create a new one using [Presentation][20] class.
*   Then, set the background style by assigning its index to [Presentation.Masters\[0\].Background.StyleIndex][21] property.
*   Finally, save the presentation using [Presentation.Save(String, SaveFormat)][22] method.

The following code sample shows how to set theme background style in a presentation.

{{< gist aspose-com-gists 5a740f14f61859a0c6a5b59591e263ac "set-theme-background.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for .NET without evaluation limitations by requesting a [temporary license][23].

## Conclusion

In this article, you have learned how to apply theme color, font and background style in PowerPoint presentations using C#. Moreover, you can install the API and integrate the provided code or customize it as per your requirements. In addition, you can visit the [documentation][24] to explore more about Aspose.Slides for .NET. Also, you can post your queries to our [forum][25].

## See Also

*   [Create SMS PowerPoint Presentations in C#][26]
*   [Convert PowerPoint PPTX/PPT to PNG Images in C#][27]
*   [Set Slide Background in PowerPoint Presentations using C#][28]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using C#][29]
*   [Apply Animation to Text in PowerPoint using C#][30]
*   [Split PowerPoint Presentations using C#][31]




[1]: #API-to-Apply-Themes-in-PowerPoint-Presentations
[2]: #Apply-Theme-to-a-PowerPoint-Presentation
[3]: #Set-Theme-Color-in-the-Presentation
[4]: #Set-Theme-Font-in-the-Presentation
[5]: #Change-Theme-Background-Style-in-Presentation
[6]: https://products.aspose.com/slides/net
[7]: https://downloads.aspose.com/slides/net
[8]: https://nuget.org/packages/Aspose.Slides.Net
[9]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[10]: https://apireference.aspose.com/slides/net/aspose.slides/ishapecollection/methods/addautoshape
[11]: https://apireference.aspose.com/slides/net/aspose.slides/ifillformat/properties/filltype
[12]: https://apireference.aspose.com/slides/net/aspose.slides/icolorformat/properties/schemecolor
[13]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/4
[14]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[15]: https://apireference.aspose.com/slides/net/aspose.slides/ishapecollection/methods/addautoshape
[16]: https://apireference.aspose.com/slides/net/aspose.slides/paragraph
[17]: https://apireference.aspose.com/slides/net/aspose.slides/portion
[18]: https://apireference.aspose.com/slides/net/aspose.slides/ibaseportionformat/properties/latinfont
[19]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/4
[20]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[21]: https://apireference.aspose.com/slides/net/aspose.slides/ibackground/properties/styleindex
[22]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/4
[23]: https://purchase.aspose.com/temporary-license
[24]: https://docs.aspose.com/slides/net/developer-guide/
[25]: https://forum.aspose.com/
[26]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/
[27]: https://blog.aspose.com/2021/09/01/convert-powerpoint-to-png-in-csharp/
[28]: https://blog.aspose.com/2021/08/31/set-background-in-powerpoint-using-csharp/
[29]: https://blog.aspose.com/2021/08/30/generate-pptx-thumbnails-using-csharp/
[30]: https://blog.aspose.com/2021/08/20/apply-animation-to-text-in-powerpoint-using-csharp/
[31]: https://blog.aspose.com/2021/09/03/split-powerpoint-presentations-using-csharp/




