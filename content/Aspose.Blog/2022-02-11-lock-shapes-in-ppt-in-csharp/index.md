---
title: 'Lock and Unlock Shapes in PowerPoint PPT in C#'
date: Fri, 11 Feb 2022 14:09:23 +0000
draft: false
url: /2022/02/11/lock-shapes-in-ppt-in-csharp/
author: 'Usman Aziz'
summary: "The protection of digital documents is a common concern these days. You don't want any unauthorized person to change the content of your documents. Therefore, it becomes inevitable to use effective protection mechanisms. Accordingly, in this article, we will show you how to protect PPT/PPTX presentations from within your .NET applications. We will accomplish that by **locking the shapes in a PowerPoint [PPT](https://docs.fileformat.com/presentation/ppt) or [PPTX](https://docs.fileformat.com/presentation/pptx/) in C#**."
tags: ['CSharp API to Lock Shapes in PowerPoint PPT', 'Lock PowerPoint PPT Shapes in Csharp', 'Unlock Shapes in PowerPoint PPT in Csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Protect-PowerPoint-Files.jpg" alt="Lock unlock shapes in PowerPoint PPT in C#">}}


The protection of digital documents is a common concern these days. You don't want any unauthorized person to change the content of your documents. Therefore, it becomes inevitable to use effective protection mechanisms. Accordingly, in this article, we will show you how to protect PPT/PPTX presentations from within your .NET applications. We will accomplish that by **locking the shapes in a PowerPoint [PPT](https://docs.fileformat.com/presentation/ppt) or [PPTX](https://docs.fileformat.com/presentation/pptx/) in C#**.

*   [C# API to Lock Shapes in PowerPoint PPT](#API-to-Lock-PowerPoint-Presentations)
*   [Lock PowerPoint PPT Shapes in C#](#Lock-a-PowerPoint-Presentation)
*   [Unlock Shapes in PowerPoint PPT](#Remove-Protection-from-PowerPoint-PPT)

## C# .NET API to Lock Shapes in PowerPoint PPT {#API-to-Lock-PowerPoint-Presentations}

To lock and unlock PowerPoint presentations, we will use [Aspose.Slides for .NET](https://products.aspose.com/slides/net). The API provides a range of features to create and manipulate PowerPoint presentations. You can either [download](https://downloads.aspose.com/slides/net) API’s DLL or install it using [NuGet](https://www.nuget.org/packages/Aspose.Slides.Net).

```
PM> Install-Package Aspose.Slides.NET
```

## Lock Shapes in PowerPoint PPT in C# {#Lock-a-PowerPoint-Presentation}

A PowerPoint presentation may contain a variety of elements such as text, images, audio, etc. Aspose.Slides for .NET takes each element as a Shape or an abject derived from Shape. So, to protect the content of the presentations, we need to lock all their shapes. Aspose.Slides provides appropriate locks for the following types of shapes.

*   Auto Shape
*   Group Shape
*   Connector
*   Picture Frame

The following steps show how to lock shapes in a PowerPoint PPT in C#.

*   First, load the PPT/PPTX file using **Presentation** class.
*   Then, get slides in the presentation using **Presentation.Slides** property.
*   For each slide, access its shapes using **ISlide.Shapes** collection.
*   For each shape in the collection, perform the following steps:
    *   Check type of the shape.
    *   Use appropriate lock according to type of the shape.
*   Finally, save the presentation using **Presentation.Save(string, SaveFormat)** method.

The following code sample shows how to lock shapes in a PowerPoint PPTX using C#.

\[gist id="345dbabceedbf2feda6da683b6cca6e2" file="lock-ppt-shapes.cs"\]

## Unlock PowerPoint Presentations in C# {#Remove-Protection-from-PowerPoint-PPT}

To unlock the shapes and make them editable, you will need to turn off the locks. Please note that if you have locked the shapes using Aspose.Slides for .NET then you will have to use the same API for unlocking. Unlocking is done by disabling the shape locks and setting their values to false.

The following code sample shows how to unlock shapes in a PPTX file in C#.

\[gist id="345dbabceedbf2feda6da683b6cca6e2" file="unlock-ppt-shapes.cs"\]

## Get a Free License

Use Aspose.Slides for .NET without evaluation limitations by getting a [free temporary license](https://purchase.aspose.com/temporary-license).

## Conclusion

In this article, you have learned how to lock shapes in PowerPoint PPT/PPTX in C#. Furthermore, you have seen how to unprotect the presentations by unlocking their shapes programmatically. Apart from that, you can explore more about Aspose.Slides for .NET by visiting the [documentation](https://docs.aspose.com/slides/net). Also, you can post your queries to our [forum](https://forum.aspose.com/).

## See Also

*   [Create MS PowerPoint Presentations in C#](https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/)
*   [Add or Remove Shapes in PowerPoint Slides using C#](https://blog.aspose.com/2020/12/24/add-shapes-to-powerpoint-slides-in-csharp/)
*   [Extract Images from PowerPoint PPT in C#](https://blog.aspose.com/2022/01/13/extract-images-from-ppt-in-csharp-net/)



