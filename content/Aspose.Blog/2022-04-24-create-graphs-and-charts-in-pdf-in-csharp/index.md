---
title: 'Create Graphs and Charts in PDF in C#'
seoTitle: "Create Graphs and Charts in PDF in C# | Add Line, Rectangle, Circle, etc"
description: "Use .NET PDF API to create charts and graphs in PDF in C#. Add various graphical objects such as lines, arcs, circles, ellipses, rectangles and curves."
date: Sun, 24 Apr 2022 07:11:00 +0000
draft: false
url: /2022/04/24/create-graphs-and-charts-in-pdf-in-csharp/
author: Usman Aziz
summary: 'In a number of [PDF][1] documents, graphs and charts are used to visually represent the data or information. In some cases, charts used to graphically describe the flow of the activities or operations in a system such as flow charts, whereas, some are used to draw the data patterns. This article covers **how to create graphs and charts in PDF files programmatically in C#**. We will explicitly demonstrate how to create different graphical objects in a PDF file.'
tags: ['Create an Arc in PDF in Csharp', 'Create an Circle in PDF in Csharp', 'Create an Ellipse in PDF in Csharp', 'Create an Line in PDF in Csharp', 'Create an Rectangle in PDF in Csharp', 'DotNet API to Create Graphs and Charts in PDF']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Create-Graphs-and-Charts-in-PDF.png" alt="Create Graphs and Charts in PDF in C#">}}


In a number of [PDF][2] documents, graphs and charts are used to visually represent the data or information. In some cases, charts used to graphically describe the flow of the activities or operations in a system such as flow charts, whereas, some are used to draw the data patterns. This article covers **how to create graphs and charts in PDF files programmatically in C#**. We will explicitly demonstrate how to create different graphical objects in a PDF file.

*   [.NET API to Create Graphs and Charts in PDF][3]
*   [Create an Arc in PDF][4]
*   [Create a Circle in PDF][5]
*   [Add a Curve in PDF][6]
*   [Add a Line in PDF][7]
*   [Create a Rectangle in PDF][8]
*   [Create an Ellipse in PDF][9]

## C# .NET API to Create Graphs and Charts in PDF {#API-to-Create-Graphs-and-Charts-in-PDF}

We will use [Aspose.PDF for .NET][10] to create charts and graphs in PDF files. The API is designed to perform PDF generation and manipulation within the .NET applications. It allows you to create PDF files of simple and complex layouts seamlessly. You can [download][11] the API's binaries or install it using [NuGet][12].

```
PM> Install-Package Aspose.PDF
```

## Create an Arc in a PDF in C# {#Create-an-Arc-in-PDF}

The following are the steps to add an arc in PDF in C#.

1.  Create a new PDF or load an existing one using the **[Document][13]** class.
2.  Create a **[Graph][14]** object with dimensions.
3.  Set **[BorderInfo][15]** for graph object.
4.  Create an instance of **[Arc][16]** class and set its dimensions and other parameters.
5.  Add arc to the shapes collection of _Graph_ using **[Graph.Shapes.Add(Arc)][17]** method.
6.  Add graph to the page using **[Page.Paragraphs.Add(Graph)][18]** method.
7.  Save the PDF file using **[Document.Save(String)][19]** method.

The following code sample shows how to add arcs in a PDF in C#.

{{< gist aspose-com-gists 340243ea16f22cd56afbabc050e5b955 "create-arc-in-pdf.cs" >}}

The following are the arcs that we have generated using the above code sample.



{{< figure align=center src="images/Create-Arc-in-PDF.png" alt="Create an Arc in PDF in C#">}}


## Create a Circle in a PDF in C# {#Create-a-Circle-in-PDF}

The following are the steps to add a circle to a PDF file in C#.

1.  Create a new PDF or load an existing one using **[Document][20]** class.
2.  Create a **[Graph][21]** object with dimensions.
3.  Set ****[BorderInfo][22]**** for graph object.
4.  Create an instance of **[Circle][23]** class and set its dimensions.
5.  Add circle to the shapes collection of _Graph_ using **[Graph.Shapes.Add(Circle)][24]** method.
6.  Add graph to the page using **[Page.Paragraphs.Add(Graph)][25]** method.
7.  Save the PDF file using **[Document.Save(String)][26]** method.

The following code sample shows how to add a circle in PDF in C#.

{{< gist aspose-com-gists 340243ea16f22cd56afbabc050e5b955 "create-circle-in-pdf.cs" >}}

The following is the circle that we have generated using the above code sample.



{{< figure align=center src="images/Create-Circle-in-PDF.png" alt="Create a Circle in PDF in C#">}}


## Add a Curve in a PDF in C# {#Add-a-Curve-in-PDF}

The following are the steps to add a curve in a PDF file in C#.

1.  Create a new PDF or load an existing one using **[Document][27]** class.
2.  Create a **[Graph][28]** object with dimensions.
3.  Set ****[BorderInfo][29]**** for graph object.
4.  Create an instance of **[Curve][30]** class and set its dimensions.
5.  Add curve to the shapes collection of _Graph_ using **[Graph.Shapes.Add(Curve)][31]** method.
6.  Add graph to the page using **[Page.Paragraphs.Add(Graph)][32]** method.
7.  Save the PDF file using **[Document.Save(String)][33]** method.

The following code sample shows how to add curves to a PDF file in C#.

{{< gist aspose-com-gists 340243ea16f22cd56afbabc050e5b955 "create-curve-in-pdf.cs" >}}

The following are the curves that we have generated using the above code sample.



{{< figure align=center src="images/Create-Curves-in-PDF.png" alt="Add a Curve in PDF in C#">}}


## Add a Line in a PDF in C# {#Add-a-Line-in-PDF}

The following are the steps to add a line in a PDF using C#.

1.  Create a new PDF or load an existing one using **[Document][34]** class.
2.  Create a **[Graph][35]** object with dimensions.
3.  Set ****[BorderInfo][36]**** for graph object.
4.  Create an instance of **[Line][37]** class and set its dimensions.
5.  Set other properties of line such as style, width, etc.
6.  Add line to the shapes collection of _Graph_ using **[Graph.Shapes.Add(Line)][38]** method.
7.  Add graph to the page using **[Page.Paragraphs.Add(Graph)][39]** method.
8.  Save the PDF file using **[Document.Save(String)][40]** method.

The following code sample shows how to add lines in PDF in C#.

{{< gist aspose-com-gists 340243ea16f22cd56afbabc050e5b955 "create-line-in-pdf.cs" >}}

The following are the lines that we have created using the above code sample.



{{< figure align=center src="images/Create-Line-in-PDF.png" alt="Add a Line in PDF in C#">}}


## Create a Rectangle in PDF in C# {#Create-a-Rectangle-in-PDF}

Similar to other graphical objects, you can add a rectangle to the PDF. Also, you can fill the rectangle with a certain color, control Z-Order, add gradient color, etc. The following are the steps to create a rectangle in a PDF file in C#.

1.  Create a new PDF or load an existing one using **[Document][41]** class.
2.  Create a **[Graph][42]** object with dimensions.
3.  Set ****[BorderInfo][43]**** for graph object.
4.  Create an instance of **[Rectangle][44]** class and set its dimensions.
5.  Set other properties of the rectangle such as fill color, gradient, etc.
6.  Add rectangle to the shapes collection of _Graph_ using **[Graph.Shapes.Add(Rectangle)][45]** method.
7.  Add graph to the page using **[Page.Paragraphs.Add(Graph)][46]** method.
8.  Save the PDF file using **[Document.Save(String)][47]** method.

The following code sample shows how to add rectangles in PDF in C#.

{{< gist aspose-com-gists 340243ea16f22cd56afbabc050e5b955 "create-rectangle-in-pdf.cs" >}}

The following are the rectangles that we have created using the above code sample.



{{< figure align=center src="images/Create-Rectangle-in-PDF.png" alt="Create a Rectangle in PDF in C#">}}


## Create an Ellipse in PDF in C# {#Create-an-Ellipse-in-PDF}

Last but not the least, let's have a look at how to create an ellipse in PDF in C#.

1.  Create a new PDF or load an existing one using **[Document][48]** class.
2.  Create a **[Graph][49]** object with dimensions.
3.  Set ****[BorderInfo][50]**** for graph object.
4.  Create an instance of **[Ellipse][51]** class and set its dimensions.
5.  Set other properties of ellipse such as fill color, etc.
6.  Add ellipse to the shapes collection of _Graph_ using **[Graph.Shapes.Add(Ellipse)][52]** method.
7.  Add graph to the page using **[Page.Paragraphs.Add(Graph)][53]** method.
8.  Save the PDF file using **[Document.Save(String)][54]** method.

The following code sample shows how to add an ellipse in a PDF file in C#.

{{< gist aspose-com-gists 340243ea16f22cd56afbabc050e5b955 "create-ellipse-in-pdf.cs" >}}

The following are the ellipses that we have created using the above code sample.



{{< figure align=center src="images/Create-Ellipse-in-PDF.png" alt="Create an Ellipse in PDF in C#">}}


## Get a Free License {#Get-a-Free-License}

You can [get a free temporary license][55] in order to use Aspose.PDF for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to create different objects of charts and graphs in PDF files using C#. You have seen how to add arcs, circles, rectangles, lines, curves, and ellipses in a PDF. Furthermore, you can explore more about .NET PDF API using the [documentation][56]. In case you would have any questions or queries, you can contact us via our [forum][57].

## See Also

*   [Add or Remove Annotations in PDF Files using C#][58]
*   [Extract Images from PDF using C#][59]
*   [Create PDF File from Images using C#][60]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #API-to-Create-Graphs-and-Charts-in-PDF
[4]: #Create-an-Arc-in-PDF
[5]: #Create-a-Circle-in-PDF
[6]: #Add-a-Curve-in-PDF
[7]: #Add-a-Line-in-PDF
[8]: #Create-a-Rectangle-in-PDF
[9]: #Create-an-Ellipse-in-PDF
[10]: https://products.aspose.com/pdf/net/
[11]: https://downloads.aspose.com/pdf/net/
[12]: http://nuget.org/packages/Aspose.PDF
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf/borderinfo
[16]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/arc
[17]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph/properties/shapes
[18]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/paragraphs
[19]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[20]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[21]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph
[22]: https://apireference.aspose.com/pdf/net/aspose.pdf/borderinfo
[23]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/circle
[24]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph/properties/shapes
[25]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/paragraphs
[26]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[27]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[28]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph
[29]: https://apireference.aspose.com/pdf/net/aspose.pdf/borderinfo
[30]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/curve
[31]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph/properties/shapes
[32]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/paragraphs
[33]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[34]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[35]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph
[36]: https://apireference.aspose.com/pdf/net/aspose.pdf/borderinfo
[37]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/line
[38]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph/properties/shapes
[39]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/paragraphs
[40]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[41]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[42]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph
[43]: https://apireference.aspose.com/pdf/net/aspose.pdf/borderinfo
[44]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/rectangle
[45]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph/properties/shapes
[46]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/paragraphs
[47]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[48]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[49]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph
[50]: https://apireference.aspose.com/pdf/net/aspose.pdf/borderinfo
[51]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/ellipse
[52]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph/properties/shapes
[53]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/paragraphs
[54]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[55]: https://purchase.aspose.com/temporary-license
[56]: https://docs.aspose.com/pdf/net/
[57]: https://forum.aspose.com/
[58]: https://blog.aspose.com/2021/01/04/add-or-remove-annotations-in-pdf-using-csharp/
[59]: https://blog.aspose.com/2021/06/15/extract-images-from-pdf-in-csharp/
[60]: https://blog.aspose.com/2021/04/20/create-pdf-from-images-using-csharp/




