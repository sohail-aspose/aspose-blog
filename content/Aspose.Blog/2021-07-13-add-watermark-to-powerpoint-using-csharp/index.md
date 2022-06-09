---
title: 'Add Watermark to PowerPoint Slides using C#'
seoTitle: "Add Watermark to PowerPoint in C# | Add Text or Image Watermark"
description: "Use .NET PowerPoint API to add watermark to the PowerPoint presentations using C#. Add text or image watermarks to the slides seamlessly."
date: Tue, 13 Jul 2021 11:36:00 +0000
draft: false
url: /2021/07/13/add-watermark-to-powerpoint-using-csharp/
author: Usman Aziz
summary: "Watermarks are commonly used to specify the ownership or to prevent unauthorized usage of the documents. In this article, we'll demonstrate how to protect PowerPoint presentations by applying watermarks programmatically. Particularly, you will learn **how to add text or image watermark to PowerPoint slides using C#**."
tags: ['Add Image Watermark to PowerPoint Slides csharp', 'Add Text Watermark to PowerPoint Slides csharp', 'Add Watermark to PowerPoint Csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Add-Watermark-in-PowerPoint.jpg" alt="Add Watermark to PowerPoint C#">}}


Watermarks are commonly used to specify the ownership or to prevent unauthorized usage of the documents. Furthermore, they are also used to display the status of a document such as manuscript, draft, etc. In this article, we'll demonstrate how to protect PowerPoint presentations by applying watermarks programmatically. Particularly, you will learn **how to add text or image watermark to PowerPoint slides using C#**.

*   [C# API to Add Watermark to PowerPoint Slides][1]
*   [Add Text Watermark to PowerPoint Slides][2]
*   [Add Image Watermark to PowerPoint Slides][3]

**Info**: You may want to check out **Aspose.Slides free** [Add Watermark to PowerPoint][4] and [Remove Watermark from PowerPoint][5] online tools.

## C# API to Add Watermark to PowerPoint Slides {#API-to-Add-Watermark-to-PowerPoint-Slides}

In order to add watermarks to the PowerPoint slides, we'll use [Aspose.Slides for .NET][6]. It is a feature-rich API that lets you create presentation documents from within the .NET applications. Furthermore, it also allows you to manipulate the existing presentation files. You can either [download][7] the API or install it using [NuGet][8].

```
PM> Install-Package Aspose.Slides.NET
```

## Add Text Watermark to PowerPoint Slides in C# {#Add-Text-Watermark-to-PowerPoint-Slides}

The following are the steps to add a text watermark to the PowerPoint slides using C#.

*   First, load the PowerPoint presentation using the [Presentation][9] class.
*   Get reference of the slide to which you want to add the watermark in [ISlide][10] object.
*   Calculate the position of the watermark.
*   Add a new auto shape to the [Shapes][11] collection of the slide and get its reference in [IAutoShape][12] object.
*   Add text frame to the shape and set its text using [IAutoShape.AddTextFrame(string)][13] method.
*   Set font size, color and rotation angle of the watermark.
*   Lock watermark to avoid removal or modification.
*   Finally, save the updated PowerPoint file using [Presentation.Save(string, SaveFormat)][14] method.

The following code sample shows how to add a text watermark to the PowerPoint slides.

{{< gist aspose-com-gists ce0af01df1fa0f11a5387d9543c6f709 "add-watermark-to-PowerPoint.cs" >}}

### Output

The following is the screenshot of the PowerPoint slide after adding the watermark.



{{< figure align=center src="images/Add-Watermark-in-PowerPoint-Slide.jpg" alt="Add Watermark to PowerPoint Slides in C#">}}


## Add Image Watermark to PowerPoint Slides in C# {#Add-Image-Watermark-to-PowerPoint-Slides}

The following are the steps to add an image watermark to the PowerPoint slides in C#.

*   First, load the PowerPoint presentation using the [Presentation][15] class.
*   Get reference of the slide to which you want to add the watermark in [ISlide][16] object.
*   Calculate the position of the watermark.
*   Add image to the presentation and get its reference in [IPPImage][17] object.
*   Add a new auto shape to the [Shapes][18] collection of the slide and get its reference in [IAutoShape][19] object.
*   Set [IAutoShape.FillFormat.FillType][20] to FillType.Picture.
*   Set watermark image by assigning _IPPImage_ object to [IAutoShape.FillFormat.PictureFillFormat.Picture.Image][21] property.
*   Lock watermark to avoid removal or modification.
*   Finally, save the updated PowerPoint file using [Presentation.Save(string, SaveFormat)][22] method.

The following code sample shows how to add an image watermark to PowerPoint slides.

{{< gist aspose-com-gists ce0af01df1fa0f11a5387d9543c6f709 "add-image-watermark-to-PowerPoint.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for .NET without evaluation limitations by requesting a [temporary license][23].

## Conclusion

In this article, you have learned how to add a watermark to the PowerPoint slides using C#. The step-by-step guide and code samples have demonstrated how to add text and image watermarks to PowerPoint presentations. In addition, you can consult the [documentation][24] to explore other features of the API. Also, you can feel free to let us know about your queries via our [forum][25].

## See Also

*   [Create MS PowerPoint Presentations in C#][26]




[1]: #API-to-Add-Watermark-to-PowerPoint-Slides
[2]: #Add-Text-Watermark-to-PowerPoint-Slides
[3]: #Add-Image-Watermark-to-PowerPoint-Slides
[4]: https://products.aspose.app/slides/watermark
[5]: https://products.aspose.app/slides/watermark/remove-watermark
[6]: https://products.aspose.com/slides/net
[7]: https://downloads.aspose.com/slides/net
[8]: https://www.nuget.org/packages/Aspose.Slides.Net
[9]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[10]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[11]: https://apireference.aspose.com/slides/net/aspose.slides/ibaseslide/properties/shapes
[12]: https://apireference.aspose.com/slides/net/aspose.slides/autoshape
[13]: https://apireference.aspose.com/slides/net/aspose.slides/autoshape/methods/addtextframe
[14]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[15]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[16]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[17]: https://apireference.aspose.com/slides/net/aspose.slides/ippimage
[18]: https://apireference.aspose.com/slides/net/aspose.slides/ibaseslide/properties/shapes
[19]: https://apireference.aspose.com/slides/net/aspose.slides/autoshape
[20]: https://apireference.aspose.com/slides/net/aspose.slides/ifillformat/properties/filltype
[21]: https://apireference.aspose.com/slides/net/aspose.slides/islidespicture/properties/image
[22]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[23]: https://purchase.aspose.com/temporary-license
[24]: https://docs.aspose.com/slides/net/developer-guide/
[25]: https://forum.aspose.com/
[26]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/





