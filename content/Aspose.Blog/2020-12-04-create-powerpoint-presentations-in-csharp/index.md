---
title: 'Create MS PowerPoint Presentations in C#'
seoTitle: ""
description: ""
date: Fri, 04 Dec 2020 11:55:47 +0000
draft: false
url: /2020/12/04/create-powerpoint-presentations-in-csharp/
author: Usman Aziz
summary: 'MS PowerPoint presentations allow you to create slide shows containing text, images, charts, animations, and other elements. Various additional formatting options let you make your presentations more appealing. In this post, you will come to know how to create such presentations programmatically. You will learn **how to create PPTX presentations having text, tables, images, and charts using C#**.'
tags: ['add slides in presentations csharp', 'add table in presentation in csharp', 'create presentations in csharp', 'update presentations in csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Create-PowerPoint-Presentation.jpg" alt="Create PowerPoint Presentations C#">}}


MS PowerPoint presentations allow you to create slide shows containing text, images, charts, animations, and other elements. Various additional formatting options let you make your presentations more appealing. In this post, you will come to know how to create such presentations programmatically. You will learn **how to create PPTX presentations having text, tables, images, and charts using C#**.

*   [C# PowerPoint API][1]
*   [Create a PowerPoint Presentation][2]
*   [Open an Existing PowerPoint Presentation][3]
*   [Add Slide to a Presentation][4]
*   [Add Text to Presentation's Slide][5]
*   [Create a Table in Presentation][6]
*   [Create a Chart in Presentation][7]
*   [Add an Image in Presentation][8]

## C# PowerPoint API - Free Download {#CSharp-PowerPoint-API}

[Aspose.Slides for .NET][9] is a presentation manipulation API that lets you create and manipulate PowerPoint documents from within your .NET applications. The API provides nearly all possible features required to implement basic as well as advanced PowerPoint automation features. You can either [download][10] the API or install it via [NuGet][11].

```
Install-Package Aspose.Slides.NET
```

## Create a PowerPoint Presentation in C# {#Create-a-PowerPoint-Presentation}

Let's start by creating an empty PowerPoint presentation using Aspose.Slides for .NET. The following are the steps to do so.

*   Create an instance of the [Presentation][12] class.
*   Save it as PPTX using [Presentation.Save(String, SaveFormat)][13] method.

The following code sample shows how to create a PowerPoint presentation in C#.

\[gist id="b1cad52e295795513abe7284bde7f7e7" file="create-presentation.cs"\]

## Open an Existing PowerPoint Presentation in C# {#Open-an-Existing-PowerPoint-Presentation}

You don't need to put extra efforts in order to open an existing PowerPoint presentation. Simply provide the path of the PPTX file to the constructor of the [Presentation][14] class and you are done. The following code sample shows how to open an existing PPTX presentation.

\[gist id="b1cad52e295795513abe7284bde7f7e7" file="open-presentation.cs"\]

## Add a Slide to Presentation in C# {#Add-Slide-to-a-Presentation}

Once you have created the presentation, you can start adding the slides to it. The following are the steps to add a slide in the presentation using Aspose.Slides for .NET.

*   Create an instance of the [Presentation][15] class.
*   Instantiate [ISlideCollection][16] class by setting a reference to the [Presentations.Slides][17] property.
*   Add an empty slide to the presentation using [Slide.AddEmptySlide(ILayoutSlide)][18] method exposed by [ISlideCollection][19] object
*   Save the presentation file using the [Presentation.Save(String, SaveFormat)][20] method.

The following code sample shows how to add a slide in a PowerPoint presentation using C#.

\[gist id="b1cad52e295795513abe7284bde7f7e7" file="add-slide.cs"\]

## Insert Text in a Slide using C# {#Add-Text-to-Presentation-Slide}

Now we can add content to the slides in the PowerPoint presentation. Let's first add a piece of text to the slide using the following steps.

*   Create a new presentation using the [Presentation][21] class.
*   Obtain the reference of the slide in the presentation.
*   Add an [IAutoShape][22] with [ShapeType][23] as Rectangle at a specified position of the slide.
*   Obtain the reference of that newly added _IAutoShape_ object.
*   Add a [TextFrame][24] to the _AutoShape_ containing the default text.
*   Save the presentation as a PPTX file.

The following code sample shows how to add text to slide in a presentation using C#.

\[gist id="b1cad52e295795513abe7284bde7f7e7" file="add-text.cs"\]

## Create Table in a Presentation using C# {#Create-Table-in-Presentation-using-CSharp}

Aspose.Slides for .NET provides an easy way to create a table in the presentation document. The following are the steps for it.

*   Create an instance of the [Presentation][25] class.
*   Obtain the reference of a slide by using its index.
*   Define arrays of columns with width and rows with height.
*   Add a table to the slide using [Slide.Shapes.AddTable()][26] method exposed by [IShapes][27] object and get the reference to the table in [ITable][28] instance.
*   Iterate through each cell to apply the formatting.
*   Add text to the cells using _Table.Rows\[\]\[\].TextFrame.Text_ property.
*   Save the presentation as a PPTX file.

The following code sample shows how to create table in a slide of PowerPoint presentation.

\[gist id="b1cad52e295795513abe7284bde7f7e7" file="create-table.cs"\]

## Create Chart in a Presentation using C# {#Create-Charts-in-Presentation}

The following are the steps to add a chart in PowerPoint presentation using C#.

*   Create an instance of the [Presentation][29] class.
*   Obtain the reference of a slide by index.
*   Add a chart with the desired type using [ISlide.Shapes.AddChart(ChartType, Single, Single, Single, Single)][30] method.
*   Add a chart title.
*   Access the chart data worksheet.
*   Clear all the default series and categories.
*   Add new series and categories.
*   Add new chart data for chart series.
*   Set fill color for chart series.
*   Add chart series labels.
*   Save the presentation as a PPTX file.

The following code sample shows how to add chart in a presentation using C#.

\[gist id="b1cad52e295795513abe7284bde7f7e7" file="create-chart.cs"\]

Learn more about the presentation charts [here][31].

## Add an Image in Presentation {#Add-an-Image-in-Presentation}

The following are the steps to add images in the presentation slide.

*   Create a new presentation using [Presentation][32] class.
*   Read SVG image using [File.ReadAllText(String path)][33] method.
*   Add image to slide using [Presentation.Slides\[0\].Shapes.AddPictureFrame(ShapeType shapeType, float x, float y,float width, float height, IPPImage image)][34] method.
*   Save the presentation.

The following code sample shows how to add image to a presentation in C#.

\[gist id="b1cad52e295795513abe7284bde7f7e7" file="add-image.cs"\]

**TIP**: Besides the creation of slides or presentations, Aspose.Slides provides [many features][35] that allow you to work with presentations. For example, using its own APIs, Aspose developed [a free online viewer for Microsoft PowerPoint Presentations][36].

## Conclusion

In this article, you have learned how to create PowerPoint presentations from scratch using C#. In addition, you have seen how to add slides, text, tables, images, and charts in new or existing PPTX presentations. You can learn more about the API using the [documentation][37].

## See Also

*   [Protect PowerPoint PPTX Presentations using C#][38]
*   [Create MS PowerPoint Presentations in ASP.NET][39]
*   [Convert PowerPoint PPTX/PPT to PNG Images in C#][40]
*   [Set Slide Background in PowerPoint Presentations using C#][41]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using C#][42]
*   [Apply Animation to Text in PowerPoint using C#][43]
*   [Split PowerPoint Presentations using C#][44]



[1]: #CSharp-PowerPoint-API
[2]: #Create-a-PowerPoint-Presentation
[3]: #Open-an-Existing-PowerPoint-Presentation
[4]: #Add-Slide-to-a-Presentation
[5]: #Add-Text-to-Presentation-Slide
[6]: #Create-Table-in-Presentation-using-CSharp
[7]: #Create-Charts-in-Presentation
[8]: #Add-an-Image-in-Presentation
[9]: https://products.aspose.com/slides/net
[10]: https://downloads.aspose.com/slides/net
[11]: https://www.nuget.org/packages/Aspose.Slides.Net
[12]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[13]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/4
[14]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[15]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[16]: https://apireference.aspose.com/net/slides/aspose.slides/islidecollection
[17]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/slides
[18]: https://apireference.aspose.com/slides/net/aspose.slides/islidecollection/methods/addemptyslide
[19]: https://apireference.aspose.com/slides/net/aspose.slides/islidecollection
[20]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/4
[21]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[22]: https://apireference.aspose.com/net/slides/aspose.slides/iautoshape
[23]: https://apireference.aspose.com/net/slides/aspose.slides/igeometryshape/properties/shapetype
[24]: https://apireference.aspose.com/slides/net/aspose.slides/textframe
[25]: http://www.aspose.com/api/net/slides/aspose.slides/presentation
[26]: https://apireference.aspose.com/slides/net/aspose.slides/ishapecollection/methods/addtable
[27]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[28]: https://apireference.aspose.com/slides/net/aspose.slides/itable
[29]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[30]: https://apireference.aspose.com/slides/net/aspose.slides/ishapecollection/methods/addchart
[31]: https://docs.aspose.com/slides/net/powerpoint-charts/
[32]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[33]: https://docs.microsoft.com/en-us/dotnet/api/system.io.file.readalltext?view=net-5.0#System_IO_File_ReadAllText_System_String_
[34]: https://apireference.aspose.com/slides/net/aspose.slides/ishapecollection/methods/addpictureframe
[35]: https://docs.aspose.com/slides/net/features-overview/
[36]: https://products.aspose.app/slides/viewer
[37]: https://docs.aspose.com/slides/net/
[38]: https://blog.aspose.com/2020/11/24/protect-powerpoint-pptx-presentations-using-csharp/
[39]: https://blog.aspose.com/2021/09/09/create-edit-powerpoint-files-in-asp-net/
[40]: https://blog.aspose.com/2021/09/01/convert-powerpoint-to-png-in-csharp/
[41]: https://blog.aspose.com/2021/08/31/set-background-in-powerpoint-using-csharp/
[42]: https://blog.aspose.com/2021/08/30/generate-pptx-thumbnails-using-csharp/
[43]: https://blog.aspose.com/2021/08/20/apply-animation-to-text-in-powerpoint-using-csharp/
[44]: https://blog.aspose.com/2021/09/03/split-powerpoint-presentations-using-csharp/





