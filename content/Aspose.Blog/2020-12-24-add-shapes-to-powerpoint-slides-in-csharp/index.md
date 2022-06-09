---
title: 'Add or Remove Shapes in PowerPoint Slides using C#'
seoTitle: ""
description: ""
date: Thu, 24 Dec 2020 10:19:00 +0000
draft: false
url: /2020/12/24/add-shapes-to-powerpoint-slides-in-csharp/
author: Usman Aziz
summary: 'Shapes are a fine way of making your PowerPoint presentations more elaborative and appealing. PowerPoint provides a wide range of shapes that you can add to your presentation slides i.e. ellipses, lines, rectangles, connectors, and so on. In order to automate this feature, this article covers **how to add, clone, and remove shapes in PowerPoint slides programmatically using C#**.'
tags: ['add shape in powerpoint slides csharp', 'clone shape in powerpoint slides csharp', 'manipulate powerpoint shapes using csharp', 'remove shape in powerpoint slides csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Work-with-Shapes-in-Slides-in-C-1024x578.jpg" alt="Work with Shapes in Slides in C#.jpg">}}


Shapes are a fine way of making your PowerPoint presentations more elaborative and appealing. PowerPoint provides a wide range of shapes that you can add to your presentation slides i.e. ellipses, lines, rectangles, connectors, and so on. In order to automate this feature, this article covers **how to add, clone, and remove shapes in PowerPoint slides programmatically using C#**.

*   [C# API to Work with PowerPoint Shapes][1]
*   [Types of PowerPoint Shapes][2]
*   [Add Shape to PowerPoint Slides][3]
*   [Add Connector to Shapes in PowerPoint Slides][4]
*   [Clone a Shape in PowerPoint Slides][5]
*   [Remove Shapes from PowerPoint Slides][6]

## C# API to Work with PowerPoint Shapes {#CSharp-API-to-Create-Shapes-in-PowerPoint-Slides}

[Aspose.Slides for .NET][7] is a C# API which is designed to work with PowerPoint presentations from within the .NET applications. Along with other presentation manipulation features, the API provides easy ways of working with shapes in PowerPoint slides. You can either download API's [DLL][8] or install it via [NuGet][9].

```
Install-Package Aspose.Slides.NET
```

## PowerPoint Shapes {#Types-of-PowerPoint-Shapes}

Aspose.Slides for .NET supports a wide range of shape types you can add to PowerPoint slides. The most commonly used shapes include:

*   [Rectangle][10]
*   [Connector][11]
*   [Ellipse][12]
*   [Line][13]
*   [and etc.][14]

## Add a Shape to PowerPoint Slides using C# {#Add-Shape-to-PowerPoint-Slides-using-CSharp}

In order to add a shape i.e. ellipse, line, rectangle, etc., Aspose.Slides provides [IShapeCollection.AddAutoShape(ShapeType, Single, Single, Single, Single)][15] method. The [ShapeType][16] enum lets you specify the type of shape you want to add. The following are the steps to add a shape to a PowerPoint slide.

*   Create an instance of [Presentation][17] class to create a new presentation or load an existing one.
*   Obtain the reference of a slide using [Presentation.Slides\[index\]][18] into [ISlide][19] object.
*   Add an Ellipse (or any other shape) using [IShapeCollection.AddAutoShape(ShapeType, Single, Single, Single, Single)][20] method exposed by [IShapes][21] object.
*   Save the PPTX file using [Presentation.Save(String, SaveFormat)][22] method.

The following code sample shows how to add a shape into a PowerPoint slide using C#.

{{< gist aspose-com-gists ecd09cd095a7e1c2455ea53f54161b3e "add-shape.cs" >}}

## Add Connector to Connect PowerPoint Shapes in C# {#Add-Connector-to-Shapes-in-PowerPoint-Slides-using-CSharp}

A connector is a line that is used to connect shapes in order to join them. A connector can be a straight or a curved line. Let's see how to add a connector between two shapes in a PowerPoint slide.

1.  Create an instance of the [Presentation][23] class to create a new presentation.
2.  Obtain the reference of a slide using [Presentation.Slides\[index\]][24] into [ISlide][25] object.
3.  Add two shapes just like you have added in the previous example and get their references in [IAutoShape][26] objects.
4.  Create a new [IConnector][27] object using [IShapeCollection.AddConnector(ShapeType, Single, Single, Single, Single)][28] method.
5.  Join the shapes using [IConnector.StartShapeConnectedTo][29] and [IConnector.EndShapeConnectedTo][30] properties.
6.  Call [IConnector.Reroute()][31] method to create the shortest automatic connection path.
7.  Save the PPTX file using [Presentation.Save(String, SaveFormat)][32] method.

The following code sample shows how to connect shapes in a PowerPoint slide using C#.

{{< gist aspose-com-gists ecd09cd095a7e1c2455ea53f54161b3e "add-connector.cs" >}}

## Clone Shapes in PowerPoint Slides using C# {#Clone-a-Shape-in-PowerPoint-Slides}

You can also clone shapes from one PowerPoint slide to another using Aspose.Slides for .NET. The following are the steps to perform this operation.

1.  Create an instance of the [Presentation][33] class.
2.  Obtain the reference of a slide using [Presentation.Slides\[index\]][34] into [ISlide][35] object.
3.  Access the source slide shapes using [ISlide.Shapes][36] collection.
4.  Access the destination slide shapes using [ISlide.Shapes][37] collection.
5.  Clone shapes from the source slide shape collection to destination slide using [IShapeCollection.AddClone(ISlide)][38] method.
6.  Save the updated presentation file.

The following code sample shows how to clone shapes within PowerPoint slides using C#.

{{< gist aspose-com-gists ecd09cd095a7e1c2455ea53f54161b3e "clone-shape.cs" >}}

## Remove Shapes from PowerPoint Slides using C# {#Remove-Shape-from-PowerPoint-Slides}

The following are the steps to remove shapes from a PowerPoint slide.

1.  Create an instance of the [Presentation][39] class to load the PPTX file.
2.  Access the desired slide from [Presentation.Slides\[index\]][40] into [ISlide][41] object.
3.  Find the shape with a specific [IShape.AlternativeText][42].
4.  Remove the shape using [ISlide.Shapes.Remove(IShape)][43] method.
5.  Save the updated presentation file.

The following code sample shows how to remove shapes from a PowerPoint slide using C#.

{{< gist aspose-com-gists ecd09cd095a7e1c2455ea53f54161b3e "remove-shape.cs" >}}

## Conclusion

MS PowerPoint lets you use various types of shapes in order to make your slides more elaborative. You can use ellipses, rectangles, lines, etc. to draw your shapes and connectors to join them. With the help of steps and code samples, this article covered how to add, clone, and remove shapes in PowerPoint slides programmatically using C#. In case you would like to explore more about the API, you can visit the [documentation][44].

## See Also

*   [Create MS PowerPoint Presentations in C#][45]




[1]: #CSharp-API-to-Create-Shapes-in-PowerPoint-Slides
[2]: #Types-of-PowerPoint-Shapes
[3]: #Add-Shape-to-PowerPoint-Slides-using-CSharp
[4]: #Add-Connector-to-Shapes-in-PowerPoint-Slides-using-CSharp
[5]: #Clone-a-Shape-in-PowerPoint-Slides
[6]: #Remove-Shape-from-PowerPoint-Slides
[7]: https://products.aspose.com/slides/net
[8]: https://downloads.aspose.com/slides/net
[9]: https://www.nuget.org/packages/Aspose.Slides.Net
[10]: https://docs.aspose.com/slides/net/rectangle/
[11]: https://docs.aspose.com/slides/net/connector/
[12]: https://docs.aspose.com/slides/net/ellipse/
[13]: https://docs.aspose.com/slides/net/line/
[14]: https://apireference.aspose.com/slides/net/aspose.slides/shapetype
[15]: https://apireference.aspose.com/slides/net/aspose.slides/ishapecollection/methods/addautoshape
[16]: https://apireference.aspose.com/slides/net/aspose.slides/shapetype
[17]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[18]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/slides
[19]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[20]: https://apireference.aspose.com/slides/net/aspose.slides/ishapecollection/methods/addautoshape
[21]: https://apireference.aspose.com/slides/net/aspose.slides/ishape
[22]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/4
[23]: http://www.aspose.com/api/net/slides/aspose.slides/presentation
[24]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/slides
[25]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[26]: https://apireference.aspose.com/slides/net/aspose.slides/iautoshape
[27]: https://apireference.aspose.com/slides/net/aspose.slides/iconnector
[28]: https://apireference.aspose.com/slides/net/aspose.slides/ishapecollection/methods/addconnector
[29]: https://apireference.aspose.com/slides/net/aspose.slides/iconnector/properties/startshapeconnectedto
[30]: https://apireference.aspose.com/slides/net/aspose.slides/iconnector/properties/endshapeconnectedto
[31]: https://apireference.aspose.com/slides/net/aspose.slides/iconnector/methods/reroute
[32]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/4
[33]: http://www.aspose.com/api/net/slides/aspose.slides/presentation
[34]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/slides
[35]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[36]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/slides
[37]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/slides
[38]: https://apireference.aspose.com/slides/net/aspose.slides/islidecollection/methods/addclone
[39]: http://www.aspose.com/api/net/slides/aspose.slides/presentation
[40]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/slides
[41]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[42]: https://apireference.aspose.com/slides/net/aspose.slides/ishape/properties/alternativetext
[43]: https://apireference.aspose.com/slides/net/aspose.slides/ishapecollection/methods/remove
[44]: https://docs.aspose.com/slides/net/
[45]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/





