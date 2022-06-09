---
title: 'Set Slide Background in PowerPoint Presentations using C#'
seoTitle: "C# Set Slide Background in PowerPoint PPTX PPT | .NET PowerPoint API"
description: "Use .NET PowerPoint API to set the slide background color in PowerPoint presentations using C# or VB.NET. Download source code."
date: Tue, 31 Aug 2021 23:59:00 +0000
draft: false
url: /2021/08/31/set-background-in-powerpoint-using-csharp/
author: Usman Aziz
summary: 'In this article, you will learn **how to set the background of slides in PowerPoint presentations programmatically using C#**. Particularly, the article will cover how to set the background of normal slides as well as the master slide.'
tags: ['Gradient as Slide Background Color Csharp', 'Set Background Color of Master Slide Csharp', 'Set Background Color of Normal Slides Csharp', 'Set Image as Slide Background Csharp']
categories: ['Aspose.Slides Product Family']
---

In this article, you will learn **how to set the background of slides in PowerPoint presentations programmatically using C#**. Particularly, the article will cover how to set the background of normal slides as well as the master slide.

*   [.NET API to Set Slide Background in PowerPoint][1]
*   [Set Background Color of Normal Slides][2]
*   [Set Background Color of Master Slide][3]
*   [Gradient as Slide Background Color][4]
*   [Set Image as Slide Background][5]

## C# API to Set Slide Background in PowerPoint {#API-to-Set-Slide-Background-in-PowerPoint}

In order to set or change the slides' background in PowerPoint presentations, we will use [Aspose.Slides for .NET][6]. The API is designed to create, manipulate and convert PowerPoint and OpenOffice presentations. You can either [download][7] the API or install it using [NuGet][8].

```
PM> Install-Package Aspose.Slides.NET
```

## Set Background Color of Normal Slides in C# {#Set-Background-Color-of-Normal-Slides}

The following are the steps to set the background color of the normal slides in a PowerPoint presentation using C#.

*   First, load the PowerPoint presentation using [Presentation][9] class.
*   Then, set the background of the desired slide by specifying its index using [Background][10] property, e.g. background type, color, fill type, etc.
*   Finally, save the updated presentation using [Presentation.Save(String, SaveFormat)][11] method.

The following code sample shows how to set the background of a slide in a PowerPoint presentation.

{{< gist aspose-com-gists c06df204f6d0031eaee4451f9f1e798b "set-slide-background.cs" >}}

Below is the screenshot of the slide before setting the background.



{{< figure align=center src="images/Set-PowerPoint-Background.jpg" alt="PowerPoint Presentation">}}


The following is the PowerPoint slide after setting the background.



{{< figure align=center src="images/Set-PPTX-Background.jpg" alt="Set Background of Slide in C#">}}


## Set Background Color of Master Slide in C# {#Set-Background-Color-of-Master-Slide}

You can also set the background of the master slide that will affect all the slides in the presentation. The following are the steps to change the background color of the master slide.

*   First, load the PowerPoint presentation using [Presentation][12] class.
*   Then, set the background of the master slide using [Presentation.Masters\[index\].Background][13] property.
*   Finally, save the updated presentation using [Presentation.Save(String, SaveFormat)][14] method.

The following code sample shows how to change the background of the master slide in PowerPoint.

{{< gist aspose-com-gists c06df204f6d0031eaee4451f9f1e798b "set-master-slide-background.cs" >}}

## Set Gradient Background Color of Slides {#Gradient-as-Slide-Background-Color}

You can also set the gradient background color of the slides using Aspose.Slides for .NET, as demonstrated in the steps below.

*   First, load the PowerPoint presentation using [Presentation][15] class.
*   Set [Presentation.Slides\[index\].Background.FillFormat.FillType][16] property to [FillType.Gradient][17].
*   Set [Presentation.Slides\[index\].Background.FillFormat.GradientFormat.TileFlip][18] property to [TileFlip.FlipBoth][19].
*   Finally, save the updated presentation using [Presentation.Save(String, SaveFormat)][20] method.

The following code sample shows how to set the gradient background color of the slides in PowerPoint.

{{< gist aspose-com-gists c06df204f6d0031eaee4451f9f1e798b "set-slide-gradient-background.cs" >}}

The following screenshot shows the gradient background of the slide.



{{< figure align=center src="images/Set-PowerPoint-Gradient-Background.jpg" alt="Set Gradient Background of Slide in C#">}}


## Set Image as Slide Background using C# {#Set-Image-as-Slide-Background}

The following are the steps to set an image as a slide background using C#.

*   First, load the PowerPoint presentation using [Presentation][21] class.
*   Set the background settings of the desired slide by specifying its index using [Background][22] property, e.g. background type, color, fill type, etc.
*   Load the image into a [System.Drawing.Image][23] object.
*   Add image to the presentation collection using [Presentation.Images.AddImage(Image)][24] and get its reference into an [IPPImage][25] object.
*   Set image as background using [Presentation.Slides\[index\].Background.FillFormat.PictureFillFormat.Picture.Image][26] property.
*   Finally, save the updated presentation using [Presentation.Save(String, SaveFormat)][27] method.

The following code sample shows how to set an image as the background of slides in a PowerPoint presentation.

{{< gist aspose-com-gists c06df204f6d0031eaee4451f9f1e798b "set-slide-image-background.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for .NET without evaluation limitations by requesting a [temporary license][28].

## Conclusion

In this article, you have learned how to set the background of slides in PowerPoint PPTX or PPT using C#. Furthermore, you have seen how to set gradient or image background of the PowerPoint presentations. You can visit the [documentation][29] to explore other features of Aspose.Slides for .NET. Also, you can feel free to let us know about your queries via our [forum][30].

## See Also

*   [Create MS PowerPoint Presentations in C#][31]




[1]: #API-to-Set-Slide-Background-in-PowerPoint
[2]: #Set-Background-Color-of-Normal-Slides
[3]: #Set-Background-Color-of-Master-Slide
[4]: #Gradient-as-Slide-Background-Color
[5]: #Set-Image-as-Slide-Background
[6]: https://products.aspose.com/slides/net/
[7]: https://downloads.aspose.com/slides/net/
[8]: https://www.nuget.org/packages/Aspose.Slides.NET
[9]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[10]: https://apireference.aspose.com/slides/net/aspose.slides/ibackground
[11]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[12]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[13]: https://apireference.aspose.com/slides/net/aspose.slides/ibaseslide/properties/background
[14]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[15]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[16]: https://apireference.aspose.com/slides/net/aspose.slides/ifillformat/properties/filltype
[17]: https://apireference.aspose.com/slides/net/aspose.slides/filltype
[18]: https://apireference.aspose.com/slides/net/aspose.slides/igradientformat/properties/tileflip
[19]: https://apireference.aspose.com/slides/net/aspose.slides/tileflip
[20]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[21]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[22]: https://apireference.aspose.com/slides/net/aspose.slides/ibackground
[23]: https://docs.microsoft.com/en-us/dotnet/api/system.drawing.image
[24]: https://apireference.aspose.com/slides/net/aspose.slides.iimagecollection/addimage/methods/3
[25]: https://apireference.aspose.com/slides/net/aspose.slides/ippimage
[26]: https://apireference.aspose.com/slides/net/aspose.slides/islidespicture/properties/image
[27]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[28]: https://purchase.aspose.com/temporary-license
[29]: https://docs.aspose.com/slides/net/developer-guide/
[30]: https://forum.aspose.com/
[31]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/





