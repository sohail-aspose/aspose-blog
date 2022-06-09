---
title: 'Create and Manipulate Tables in PowerPoint using C#'
seoTitle: "C#: Create and Manipulate Tables in PowerPoint | .NET PowerPoint API"
description: "Use .NET PowerPoint API to create and manipulate tables in PowerPoint presentations using C#. Change formatting and aspect ratio of tables dynamically."
date: Mon, 23 Aug 2021 10:25:00 +0000
draft: false
url: /2021/08/23/create-tables-in-powerpoint-using-csharp/
author: Usman Aziz
summary: 'Tables are used to arrange the data in the form of rows and columns. Moreover, they organize and summarize the data so that it can be viewed and analyzed easily. MS PowerPoint also allows you to insert tables in the presentations. Accordingly, this article covers **how to create and manipulate tables in PowerPoint presentations using C#**.'
tags: ['Access a Table in PowerPoint Csharp', 'Create a Table in PowerPoint Presentation Csharp', 'Format Text in PowerPoint Tables Csharp', 'Lock Aspect Ratio of PowerPoint Tables Csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Create-Table-in-PowerPoint-1.jpg" alt="Create and Manipulate Tables in PowerPoint C#">}}


Tables are used to arrange the data in the form of rows and columns. Moreover, they organize and summarize the data so that it can be viewed and analyzed easily. MS PowerPoint also allows you to insert tables in the presentations. Accordingly, this article covers **how to create and manipulate tables in PowerPoint presentations using C#**.

*   [C# API to Create and Manipulate Tables in PowerPoint][1]
*   [Create a Table in PowerPoint Presentations][2]
*   [Access a Table in a Presentation][3]
*   [Format Text in PowerPoint Tables][4]
*   [Lock Aspect Ratio of the Tables][5]

## C# API to Create and Manipulate Tables in PowerPoint {#API-to-Create-and-Manipulate-Tables-in-PowerPoint}

To create and manipulate tables in PowerPoint presentations, we will use [Aspose.Slides for .NET][6]. The API lets you create, manipulate and convert PowerPoint and OpenOffice documents. You can [download][7] the API's DLL and add a reference to it in your project. Also, you can install it using [NuGet][8].

```
PM> Install-Package Aspose.Slides.NET
```

## Create a Table in PowerPoint Presentations using C# {#Create-a-Table-in-PowerPoint-Presentation}

Creating a table using Aspose.Slides for .NET is a piece of cake. The following steps show how to create a table in a PowerPoint presentation using C#.

*   First, create a new presentation or load an existing one using [Presentation][9] class.
*   Then, get reference of the desired slide into an [ISlide][10] object.
*   Define the width and height of columns and rows respectively in _double\[\]_ arrays.
*   Insert a new table in presentation using [ISlide.Shapes.AddTable()][11] method.
*   Get reference of the newly created table in an [ITable][12] object.
*   Create a loop to iterate through the rows of the table.
*   Create a nested loop to iterate through the cells of the table and in each iteration, perform the following operations.
    *   Set text of the cell using [ITable.Rows\[rowIndex\]\[cellIndex\].TextFrame.Text][13] property.
    *   Get reference of the cell's formatting into an [ICellFormat][14] object and set cell's border style, if required.
*   Finally, save the presentation using [Presentation.Save(String, SaveFormat)][15] method.

The following code sample shows how to create a table in a PowerPoint presentation.

{{< gist aspose-com-gists d128eb81b15aa2d87d6c08f68afc0078 "create-table.cs" >}}

The following screenshot shows the table that we have created using the above code.



{{< figure align=center src="images/Create-Table-in-PowerPoint.jpg" alt="Create Table in PowerPoint C#">}}


## Access a Table in a Presentation using C# {#Access-a-Table-in-a-Presentation-using-Java}

You can also access the tables in the existing PowerPoint presentations and manipulate them as required. The following are the steps to access the tables in a presentation.

*   First, load an existing presentation using [Presentation][16] class.
*   Then, get reference of the desired slide into an [ISlide][17] object.
*   Create an instance of [ITable][18] and initialize it with null.
*   Iterate through all [IShape][19] objects in [ISlide.Shapes][20] collection.
*   Filter the shapes of type [ITable][21].
*   Type cast the shape into _ITable_ and manipulate it as required.
*   Finally, save the presentation using [Presentation.Save(String, SaveFormat)][22] method.

The following code sample shows how to access tables in a PowerPoint presentation using C#.

{{< gist aspose-com-gists d128eb81b15aa2d87d6c08f68afc0078 "access-table.cs" >}}

## Format Text in PowerPoint Tables using C# {#Format-Text-in-PowerPoint-Tables-using-Java}

Aspose.Slides for .NET also allows you to set formatting of the tables quite easily, as demonstrated in the steps below.

*   First, load an existing presentation using [Presentation][23] class.
*   Then, get reference of the desired slide into an [ISlide][24] object.
*   Retreive the reference of the desired table from slide into an [ITable][25] object.
*   Set formatting using [PortionFormat][26], [ParagraphFormat][27], and [TextFrameFormat][28] classes.
*   Assign formatting to the table using _ITable.setTextFormat()_ methods.
*   Finally, save the presentation using [Presentation.Save(String, SaveFormat)][29] method.

The following code sample shows how to set the formatting of the table in PowerPoint using C#.

{{< gist aspose-com-gists d128eb81b15aa2d87d6c08f68afc0078 "format-table.cs" >}}

## Lock Aspect Ratio of Tables in PowerPoint using C# {#Lock-the-Aspect-Ratio-of-the-Tables}

You can also lock the aspect ratio of the tables in PowerPoint presentations using C#. The following are the steps to achieve this.

*   First, load an existing presentation using [Presentation][30] class.
*   Then, get reference of the desired slide into an [ISlide][31] object.
*   Create a table or retrieve the reference of an existing table into an [ITable][32] object.
*   Set [ITable.ShapeLock.AspectRatioLocked][33] property to _!ITable.ShapeLock.AspectRatioLocked_ to lock the aspect ratio.
*   Finally, save the presentation using [Presentation.Save(String, SaveFormat)][34] method.

The following code sample shows how to lock the aspect ratio of the table in PowerPoint presentations.

{{< gist aspose-com-gists d128eb81b15aa2d87d6c08f68afc0078 "lock-aspect-ratio.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for .NET without evaluation limitations by getting a free [temporary license][35].

## Conclusion

In this article, you have learned how to create tables in PowerPoint presentations using C#. Moreover, you have seen how to access and manipulate existing tables in the PowerPoint presentations programmatically. In addition, you can visit the [documentation][36] to explore more about Aspose.Slides for .NET. Also, you can ask your questions via our [forum][37].

## See Also

*   [Convert PowerPoint PPTX/PPT to PNG Images in C#][38]
*   [Set Slide Background in PowerPoint Presentations using C#][39]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using C#][40]
*   [Apply Animation to Text in PowerPoint using C#][41]
*   [Split PowerPoint Presentations using C#][42]




[1]: #API-to-Create-and-Manipulate-Tables-in-PowerPoint
[2]: #Create-a-Table-in-PowerPoint-Presentation
[3]: #Access-a-Table-in-a-Presentation-using-Java
[4]: #Format-Text-in-PowerPoint-Tables-using-Java
[5]: #Lock-the-Aspect-Ratio-of-the-Tables
[6]: https://products.aspose.com/slides/net
[7]: https://downloads.aspose.com/slides/net
[8]: https://www.nuget.org/packages/Aspose.Slides.Net
[9]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[10]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[11]: https://apireference.aspose.com/slides/net/aspose.slides/ishapecollection/methods/addtable
[12]: https://apireference.aspose.com/slides/net/aspose.slides/itable
[13]: https://apireference.aspose.com/slides/net/aspose.slides/itextframe/properties/text
[14]: https://apireference.aspose.com/slides/net/aspose.slides/icellformat
[15]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[16]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[17]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[18]: https://apireference.aspose.com/slides/net/aspose.slides/itable
[19]: https://apireference.aspose.com/slides/net/aspose.slides/ishape
[20]: https://apireference.aspose.com/slides/net/aspose.slides/ibaseslide/properties/shapes
[21]: https://apireference.aspose.com/slides/net/aspose.slides/itable
[22]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[23]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[24]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[25]: https://apireference.aspose.com/slides/net/aspose.slides/itable
[26]: https://apireference.aspose.com/slides/net/aspose.slides/portionformat
[27]: https://apireference.aspose.com/slides/net/aspose.slides/paragraphformat
[28]: https://apireference.aspose.com/slides/net/aspose.slides/textframeformat
[29]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[30]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[31]: https://apireference.aspose.com/slides/net/aspose.slides/islide
[32]: https://apireference.aspose.com/slides/net/aspose.slides/itable
[33]: https://apireference.aspose.com/slides/net/aspose.slides/igraphicalobjectlock/properties/aspectratiolocked
[34]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[35]: https://purchase.aspose.com/temporary-license
[36]: https://docs.aspose.com/slides/net
[37]: https://forum.aspose.com/
[38]: https://blog.aspose.com/2021/09/01/convert-powerpoint-to-png-in-csharp/
[39]: https://blog.aspose.com/2021/08/31/set-background-in-powerpoint-using-csharp/
[40]: https://blog.aspose.com/2021/08/30/generate-pptx-thumbnails-using-csharp/
[41]: https://blog.aspose.com/2021/08/20/apply-animation-to-text-in-powerpoint-using-csharp/
[42]: https://blog.aspose.com/2021/09/03/split-powerpoint-presentations-using-csharp/





