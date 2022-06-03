---
title: 'Apply 3D Effects in PowerPoint PPT using C#'
date: Mon, 24 Jan 2022 15:13:27 +0000
draft: false
url: /2022/01/24/create-three-d-effects-in-ppt-csharp-net/
author: ''Usman Aziz''
summary: '3D effects in PowerPoint presentations make the content more attractive. Using 3D text or shapes, you can enhance the interactivity and catch the attention of the audience. While working on the automation of PowerPoint from within .NET applications, you may need to add 3D effects to the presentations. To accomplish that, this article covers **how to apply the 3D effects in PowerPoint PPT in C#**.'
tags: ['Apply 3D Effects to an Image in PPT Csharp', 'Create a 3D Shape in PowerPoint in Csharp', 'Create a 3D Text in PowerPoint in Csharp', 'Dotnet API to Create 3D Effects in PowerPoint', 'Set Gradient for 3D Shapes in PPT in Csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Apply-3D-Effects-in-PowerPoint.psd_.png" alt="Apply 3D Effects in PowerPoint using C#">}}


3D effects in PowerPoint presentations make the content more attractive. Using 3D text or shapes, you can enhance the interactivity and catch the attention of the audience. While working on the automation of PowerPoint from within .NET applications, you may need to add 3D effects to the presentations. To accomplish that, this article covers **how to apply the 3D effects in PowerPoint PPT in C#**.

*   [.NET API to Create 3D Effects in PowerPoint][1]
*   [Create a 3D Text in PowerPoint in C#][2]
*   [Create a 3D Shape in PowerPoint in C#][3]
*   [Set Gradient for 3D Shapes][4]
*   [Apply 3D Effects to an Image in PowerPoint][5]

## .NET API to Apply 3D Effects in PowerPoint {#API-to-Create-3D-Effects-in-PowerPoint}

[Aspose.Slides for .NET][6] is an amazing API that provides a range of features to implement PowerPoint automation. Using the API, you can create and manipulate presentations seamlessly. We will use this API to apply 3D effects in the PowerPoint presentations. You can either [download][7] API's DLL or install it using [NuGet][8].

```
PM> Install-Package Aspose.Slides.NET 
```

## Create a 3D Text in PowerPoint in C# {#Create-a-3D-Text-in-PowerPoint}

The following are the steps to create a 3D text fragment in PowerPoint PPT using C#.

*   First, create a new PPT or load existing one using [Presentation][9] class.
*   Then, add a new rectangle shape using [AddAutoShape()][10] method.
*   Set shape's properties such as fill type, text, etc.
*   Get reference of the text inside shape into a [Portion][11] object.
*   Apply formatting to the text portion.
*   Get reference of the [TextFrame][12] inside shape.
*   Apply 3D effects using properties in [TextFrame.TextFrameFormat.ThreeDFormat][13].
*   Finally, save presentation using [Presentation.Save(String, SaveFormat)][14] method.

The following code sample shows how to create a 3D text in PowerPoint in C#.

{{< gist aspose-com-gists 9111ed69eeb4cf031293753aa445d405 "create-3d-text-in-ppt.cs" >}}

The following screenshot shows output of the code sample above.



{{< figure align=center src="images/Create-3D-Text-in-PPT.png" alt="Create a 3D Text in PowerPoint in C#">}}


## Create a 3D Shape in PowerPoint in C# {#Create-a-3D-Shape-in-PowerPoint}

Similar to text, you can apply 3D effects to the shapes in PowerPoint presentations. The following are the steps to create a 3D shape in PowerPoint in C#.

*   First, create a new PPT using [Presentation][15] class.
*   Add a new rectangle shape using [AddAutoShape()][16] method.
*   Set shape's text using [Shape.TextFrame.Text][17] property.
*   Apply 3D effects to shape using properties in [IAutoShape.ThreeDFormat][18].
*   Finally, save presentation using [Presentation.Save(String, SaveFormat)][19] method.

The following code sample shows how to apply 3D effects to shapes in PowerPoint using C#.

{{< gist aspose-com-gists 9111ed69eeb4cf031293753aa445d405 "create-3d-shape-in-ppt.cs" >}}

The following is the 3D shape that we get after executing this code.



{{< figure align=center src="images/Create-3D-Shape-in-PPT.png" alt="Create a 3D Shape in PowerPoint in C#">}}


## Create Gradient for 3D Shapes {#Set-Gradient-for-3D-Shapes}

You can also apply gradient effects to the shapes following the steps below.

*   First, create a new PPT using [Presentation][20] class.
*   Add a new rectangle shape using [AddAutoShape()][21] method.
*   Set shape's text using [Shape.TextFrame.Text][22] property.
*   Set [IAutoShape.FillFormat.FillType][23] to [FillType.Gradient][24] and set gradient colors.
*   Apply 3D effects to shape using properties in [IAutoShape.ThreeDFormat][25].
*   Finally, save presentation using [Presentation.Save(String, SaveFormat)][26] method.

The following code sample shows how to apply gradient effects to shapes in PowerPoint.

{{< gist aspose-com-gists 9111ed69eeb4cf031293753aa445d405 "create-3d-shape-gradient-in-ppt.cs" >}}

The following is the 3D shape after applying the gradient effect.



{{< figure align=center src="images/Create-3D-Shape-Gradient-in-PPT.png" alt="Create Gradient for 3D Shapes in PowerPoint">}}


## Apply 3D Effects to an Image in PowerPoint in C# {#Apply-3D-Effect-to-an-Image-in-PowerPoint}

Aspose.Slides for .NET also allows you to apply 3D effects to an image. The following are the steps to perform this operation in C#.

*   Create a new PPT using [Presentation][27] class.
*   Add a new rectangle shape using [AddAutoShape()][28] method.
*   Set [IAutoShape.FillFormat.FillType][29] to [FillType.Picture][30] and add image.
*   Apply 3D effects to shape using properties in [IAutoShape.ThreeDFormat][31].
*   Save presentation using [Presentation.Save(String, SaveFormat)][32] method.

The following are the steps to apply 3D effects to an image in PPT using C#.

{{< gist aspose-com-gists 9111ed69eeb4cf031293753aa445d405 "create-3d-image-in-ppt.cs" >}}

The following is the resultant image that we get after applying 3D effects.



{{< figure align=center src="images/Create-3D-Image-in-PPT.png" alt="Apply 3D Effects to an Image in PowerPoint in C#">}}


## Get a Free License

You can get a [free temporary license][33] to use Aspose.Slides for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to apply 3D effects in PowerPoint presentations using C#. We have covered how to create 3D text or shapes and apply 3D effects to images in PPT or PPTX presentations. In case you want to explore more about Aspose.Slides for .NET, you can visit the [documentation][34]. Also, you can post your queries to our [forum][35].

## See Also

*   [Create MS PowerPoint Presentations in C#][36]
*   [Add or Remove Shapes in PowerPoint Slides using C#][37]




[1]: #API-to-Create-3D-Effects-in-PowerPoint
[2]: #Create-a-3D-Text-in-PowerPoint
[3]: #Create-a-3D-Shape-in-PowerPoint
[4]: #Set-Gradient-for-3D-Shapes
[5]: #Apply-3D-Effect-to-an-Image-in-PowerPoint
[6]: https://products.aspose.com/slides/net
[7]: https://downloads.aspose.com/slides/net
[8]: https://www.nuget.org/packages/Aspose.Slides.Net
[9]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[10]: https://apireference.aspose.com/slides/net/aspose.slides/ishapecollection/methods/addautoshape
[11]: https://apireference.aspose.com/slides/net/aspose.slides/portion
[12]: https://apireference.aspose.com/slides/net/aspose.slides/textframe
[13]: https://apireference.aspose.com/slides/net/aspose.slides/itextframeformat/properties/threedformat
[14]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/4
[15]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[16]: https://apireference.aspose.com/slides/net/aspose.slides/ishapecollection/methods/addautoshape
[17]: https://apireference.aspose.com/slides/net/aspose.slides/itextframe/properties/text
[18]: https://apireference.aspose.com/slides/net/aspose.slides/ithreedformat
[19]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/4
[20]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[21]: https://apireference.aspose.com/slides/net/aspose.slides/ishapecollection/methods/addautoshape
[22]: https://apireference.aspose.com/slides/net/aspose.slides/itextframe/properties/text
[23]: https://apireference.aspose.com/slides/net/aspose.slides/ifillformat/properties/filltype
[24]: https://apireference.aspose.com/slides/net/aspose.slides/filltype
[25]: https://apireference.aspose.com/slides/net/aspose.slides/ithreedformat
[26]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/4
[27]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[28]: https://apireference.aspose.com/slides/net/aspose.slides/ishapecollection/methods/addautoshape
[29]: https://apireference.aspose.com/slides/net/aspose.slides/ifillformat/properties/filltype
[30]: https://apireference.aspose.com/slides/net/aspose.slides/filltype
[31]: https://apireference.aspose.com/slides/net/aspose.slides/ithreedformat
[32]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/4
[33]: https://purchase.aspose.com/temporary-license
[34]: https://docs.aspose.com/slides/net/
[35]: https://forum.aspose.com/
[36]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/
[37]: https://blog.aspose.com/2020/12/24/add-shapes-to-powerpoint-slides-in-csharp/




