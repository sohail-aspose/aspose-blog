---
title: 'Create SmartArt in PowerPoint Presentations using C#'
seoTitle: "Create SmartArt in PowerPoint Presentations using C# | Source Code"
description: "Use .NET PowerPoint API to create SmartArt shapes in PowerPoint presentations using C# or VB.NET. Access and modify SmartArt in PowerPoint."
date: Wed, 22 Sep 2021 15:14:34 +0000
draft: false
url: /2021/09/22/create-smartart-in-powerpoint-using-csharp/
author: Usman Aziz
summary: 'SmartArt in presentations is used to provide the information in visual form. Sometimes, it is opted to make the simple text more appealing. Whereas, in other cases, it is used to demonstrate flow diagrams, processes, relationships between different entities, etc. In this article, you will learn **how to create SmartArt in PowerPoint presentations programmatically using C#**.'
tags: ['Access a SmartArt Shape in PowerPoint Csharp', 'Change SmartArt Shape Style in PowerPoint Csharp', 'Create a SmartArt Shape in PowerPoint Csharp', 'NET API to Create SmartArt in PowerPoint']
categories: ['Aspose.Slides Product Family']
---

SmartArt in presentations is used to provide the information in visual form. Sometimes, it is opted to make the simple text more appealing. Whereas, in other cases, it is used to demonstrate flow diagrams, processes, relationships between different entities, etc. In this article, you will learn **how to create SmartArt in PowerPoint presentations programmatically using C#**.

*   [.NET API to Create SmartArt in PowerPoint][1]
*   [Create a SmartArt Shape in PowerPoint][2]
*   [Access a SmartArt Shape in PowerPoint][3]
*   [Change SmartArt Shape's Style][4]

## .NET API to Create SmartArt in PowerPoint {#API-to-Create-SmartArt-in-PowerPoint}

To work with SmartArt in PowerPoint presentations, we will use [Aspose.Slides for .NET][5]. It is a powerful class library to create and manipulate PowerPoint and OpenOffice presentations. You can either install the API via [NuGet][6] or [download][7] its DLL.

```
PM> Install-Package Aspose.Slides.NET
```

## Create a SmartArt Shape in PowerPoint using C# {#Create-a-SmartArt-Shape-in-PowerPoint}

Aspose.Slides for .NET provides the easiest way to create the SmartArt shapes in the presentations. For demonstration, let's create a SmartArt shape from scratch in a PowerPoint presentation using C#.

*   Create a new presentation or load an existing one using [Presentation][8] class.
*   Get reference of the desired slide into an [ISlide][9] object.
*   Create a SmartArt using [ISlide.Shapes.AddSmartArt()][10] method.
*   Save the updated presentation using [Presentation.Save(String, SaveFormat)][11] method.

The following code sample shows how to create a SmartArt shape in a PowerPoint presentation.

{{< gist aspose-com-gists f69856d5e985b8c77904c541dd1b33f5 "create-smartart.cs" >}}

The following screenshot shows the output of the above code sample.



{{< figure align=center src="images/Create-SmartArt.jpg" alt="Create SmartArt in PowerPoint C#">}}


## Access a SmartArt Shape in PowerPoint using C# {#Access-a-SmartArt-Shape-in-PowerPoint}

You can also access the SmartArt shapes in the existing PowerPoint presentations. Once accessed, you can modify them as required. The following are the steps to access the SmartArt shapes in PowerPoint presentations using C#.

*   Create a new presentation or load an existing one using [Presentation][12] class.
*   Get reference of the desired slide into an [ISlide][13] object.
*   Loop through the shapes in the slide using [ISlide.Shapes][14] collection.
*   If the shape is of type [ISmartArt][15], then get its reference into an [ISmartArt][16] object.
*   If required, filter the SmartArt shapes of a specific layout using [ISmartArt.Layout][17] property.

The following code sample shows how to access SmartArt shapes in PowerPoint presentations.

{{< gist aspose-com-gists f69856d5e985b8c77904c541dd1b33f5 "access-smartart.cs" >}}

## Change SmartArt Shape's Style using C# {#Change-SmartArt-Shape-Style}

Once you have accessed a SmartArt shape, you can change its style as well. The following steps demonstrate how to change the style of the SmartArt shapes in a PowerPoint presentation using C#.

*   Create a new presentation or load an existing one using [Presentation][18] class.
*   Get reference of the desired slide into an [ISlide][19] object.
*   Loop through the shapes in the slide using [ISlide.Shapes][20] collection.
*   If the shape is of type [ISmartArt][21], then get its reference into an [ISmartArt][22] object.
*   Change the desired style, i.e. [ISmartArt.ColorStyle][23], [ISmartArt.QuickStyle][24], etc.
*   Save the updated presentation using [Presentation.Save(String, SaveFormat)][25] method.

The following code sample shows how to change the style of the SmartArt shapes in PowerPoint presentations.

{{< gist aspose-com-gists f69856d5e985b8c77904c541dd1b33f5 "change-smartart.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

Get a free [temporary license][26] to use Aspose.Slides for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to create SmartArt in PowerPoint presentations using C#. Moreover, you have seen how to access the SmartArt shapes and change their styles programmatically. You can explore the [documentation][27] to learn more about Aspose.Slides for .NET. In addition, you can ask your questions via our [forum][28].

## See Also

*   [Convert PowerPoint PPTX/PPT to PNG Images in C#][29]
*   [Set Slide Background in PowerPoint Presentations using C#][30]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using C#][31]
*   [Apply Animation to Text in PowerPoint using C#][32]
*   [Split PowerPoint Presentations using C#][33]




[1]: #API-to-Create-SmartArt-in-PowerPoint
[2]: #Create-a-SmartArt-Shape-in-PowerPoint
[3]: #Access-a-SmartArt-Shape-in-PowerPoint
[4]: #Change-SmartArt-Shape-Style
[5]: https://products.aspose.com/slides/net
[6]: https://www.nuget.org/packages/Aspose.Slides.NET
[7]: https://downloads.aspose.com/slides/net
[8]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[9]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[10]: https://apireference.aspose.com/slides/net/aspose.slides/ishapecollection/methods/addsmartart
[11]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[12]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[13]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[14]: https://apireference.aspose.com/slides/net/aspose.slides/ibaseslide/properties/shapes
[15]: https://apireference.aspose.com/slides/net/aspose.slides.smartart/ismartart
[16]: https://apireference.aspose.com/slides/net/aspose.slides.smartart/ismartart
[17]: https://apireference.aspose.com/slides/net/aspose.slides.smartart/ismartart/properties/layout
[18]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[19]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[20]: https://apireference.aspose.com/slides/net/aspose.slides/ibaseslide/properties/shapes
[21]: https://apireference.aspose.com/slides/net/aspose.slides.smartart/ismartart
[22]: https://apireference.aspose.com/slides/net/aspose.slides.smartart/ismartart
[23]: https://apireference.aspose.com/slides/net/aspose.slides.smartart/ismartart/properties/colorstyle
[24]: https://apireference.aspose.com/slides/net/aspose.slides.smartart/ismartart/properties/quickstyle
[25]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[26]: https://purchase.aspose.com/temporary-license
[27]: https://docs.aspose.com/slides/net/developer-guide/
[28]: https://forum.aspose.com/
[29]: https://blog.aspose.com/2021/09/01/convert-powerpoint-to-png-in-csharp/
[30]: https://blog.aspose.com/2021/08/31/set-background-in-powerpoint-using-csharp/
[31]: https://blog.aspose.com/2021/08/30/generate-pptx-thumbnails-using-csharp/
[32]: https://blog.aspose.com/2021/08/20/apply-animation-to-text-in-powerpoint-using-csharp/
[33]: https://blog.aspose.com/2021/09/03/split-powerpoint-presentations-using-csharp/




